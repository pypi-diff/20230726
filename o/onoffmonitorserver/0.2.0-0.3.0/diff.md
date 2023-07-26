# Comparing `tmp/onoffmonitorserver-0.2.0-py3-none-any.whl.zip` & `tmp/onoffmonitorserver-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,21 @@
-Zip file size: 7258 bytes, number of entries: 17
+Zip file size: 9925 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 17:32 onoffmonitorserver/__init__.py
 -rw-r--r--  2.0 unx      137 b- defN 23-Jul-22 16:30 onoffmonitorserver/admin.py
 -rw-r--r--  2.0 unx      204 b- defN 23-Jul-06 17:32 onoffmonitorserver/apps.py
 -rw-r--r--  2.0 unx      365 b- defN 23-Jul-06 17:32 onoffmonitorserver/filters.py
--rw-r--r--  2.0 unx     1689 b- defN 23-Jul-25 09:48 onoffmonitorserver/models.py
+-rw-r--r--  2.0 unx     1889 b- defN 23-Jul-26 15:42 onoffmonitorserver/models.py
 -rw-r--r--  2.0 unx      333 b- defN 23-Jul-06 17:32 onoffmonitorserver/permissions.py
--rw-r--r--  2.0 unx     1120 b- defN 23-Jul-25 09:37 onoffmonitorserver/serializers.py
+-rw-r--r--  2.0 unx     1135 b- defN 23-Jul-26 15:40 onoffmonitorserver/serializers.py
 -rw-r--r--  2.0 unx       60 b- defN 23-Jul-06 17:32 onoffmonitorserver/tests.py
 -rw-r--r--  2.0 unx      292 b- defN 23-Jul-22 16:30 onoffmonitorserver/urls.py
--rw-r--r--  2.0 unx     2184 b- defN 23-Jul-25 09:37 onoffmonitorserver/views.py
+-rw-r--r--  2.0 unx     2310 b- defN 23-Jul-26 15:40 onoffmonitorserver/views.py
 -rw-r--r--  2.0 unx     2205 b- defN 23-Jul-22 16:30 onoffmonitorserver/migrations/0001_initial.py
 -rw-r--r--  2.0 unx      594 b- defN 23-Jul-25 09:51 onoffmonitorserver/migrations/0002_alter_device_gpio_pin_device_gpio_input_and_more.py
+-rw-r--r--  2.0 unx      707 b- defN 23-Jul-26 15:42 onoffmonitorserver/migrations/0003_monitor_gpio_mode_alter_device_gpio_input.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 17:32 onoffmonitorserver/migrations/__init__.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jul-25 09:54 onoffmonitorserver-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 09:54 onoffmonitorserver-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-25 09:54 onoffmonitorserver-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1527 b- defN 23-Jul-25 09:54 onoffmonitorserver-0.2.0.dist-info/RECORD
-17 files, 11882 bytes uncompressed, 4684 bytes compressed:  60.6%
+-rw-r--r--  2.0 unx     1687 b- defN 23-Jul-26 16:13 onoffmonitorserver-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jul-26 16:13 onoffmonitorserver-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 16:13 onoffmonitorserver-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-26 16:13 onoffmonitorserver-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1761 b- defN 23-Jul-26 16:13 onoffmonitorserver-0.3.0.dist-info/RECORD
+19 files, 16826 bytes uncompressed, 6957 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -30,23 +30,29 @@
 
 Filename: onoffmonitorserver/migrations/0001_initial.py
 Comment: 
 
 Filename: onoffmonitorserver/migrations/0002_alter_device_gpio_pin_device_gpio_input_and_more.py
 Comment: 
 
+Filename: onoffmonitorserver/migrations/0003_monitor_gpio_mode_alter_device_gpio_input.py
+Comment: 
+
 Filename: onoffmonitorserver/migrations/__init__.py
 Comment: 
 
-Filename: onoffmonitorserver-0.2.0.dist-info/METADATA
+Filename: onoffmonitorserver-0.3.0.dist-info/LICENSE
+Comment: 
+
+Filename: onoffmonitorserver-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: onoffmonitorserver-0.2.0.dist-info/WHEEL
+Filename: onoffmonitorserver-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: onoffmonitorserver-0.2.0.dist-info/top_level.txt
+Filename: onoffmonitorserver-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: onoffmonitorserver-0.2.0.dist-info/RECORD
+Filename: onoffmonitorserver-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## onoffmonitorserver/models.py

```diff
@@ -6,17 +6,23 @@
 from django.utils import timezone
 
 
 class Monitor(models.Model):
     """
     Model for storing data about a monitor (such as "garage")
     """
+    GPIO_MODE_CHOICES = (
+        (0, 'BOARD'),
+        (1, 'BCM'),
+    )
     user = models.ForeignKey(settings.AUTH_USER_MODEL,
                              on_delete=models.CASCADE)
     name = models.CharField(max_length=100)
+    gpio_mode = models.PositiveSmallIntegerField(
+        choices=GPIO_MODE_CHOICES, default=0, verbose_name='GPIO pin mode')
 
     def __str__(self):
         return f'{self.name} ({self.user})'
 
 
 class Device(models.Model):
     """
```

## onoffmonitorserver/serializers.py

```diff
@@ -3,16 +3,16 @@
 from . import models
 
 
 class MonitorSerializer(ModelSerializer):
     user = HiddenField(default=CurrentUserDefault())
 
     class Meta:
-        model = models.Device
-        fields = ['id', 'name', 'user']
+        model = models.Monitor
+        fields = ['id', 'name', 'gpio_mode', 'user']
 
 
 class DeviceSerializer(ModelSerializer):
     user = HiddenField(default=CurrentUserDefault())
 
     def validate(self, attrs):
         print(attrs)
@@ -23,14 +23,15 @@
     class Meta:
         model = models.Device
         fields = ['id', 'name', 'user', 'monitor', 'gpio_input', 'gpio_led']
 
 
 class StatusSerializer(ModelSerializer):
     user = CurrentUserDefault()
+
     def validate(self, attrs):
         if attrs['device'].user != self.user(self):
             raise ValidationError('Device owner must be the current user')
         return super().validate(attrs)
 
     class Meta:
         model = models.Status
```

## onoffmonitorserver/views.py

```diff
@@ -21,15 +21,20 @@
     serializer_class = MonitorSerializer
     permission_classes = [IsAuthenticated, IsDeviceOwner]
     authentication_classes = [SessionAuthentication, TokenAuthentication]
     filter_backends = [DeviceOwnerFilter]
 
     @action(methods=['GET'], detail=True, url_path='conf')
     def device_list(self, request, pk: int):
-        return Response(models.Device.objects.filter(monitor_id=pk).values('id', 'gpio_input', 'gpio_led'))
+        return Response({
+            'gpio_mode': self.get_object().gpio_mode,
+            'devices':
+                models.Device.objects.filter(monitor_id=pk).values(
+                    'id', 'gpio_input', 'gpio_led')
+        })
 
 
 class DeviceViewSet(ModelViewSet):
     """
     ViewSet for managing Device objects
     """
     queryset = models.Device.objects.all()
```

## Comparing `onoffmonitorserver-0.2.0.dist-info/RECORD` & `onoffmonitorserver-0.3.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 onoffmonitorserver/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 onoffmonitorserver/admin.py,sha256=zIKRnR95dyCRkXPMlExPPPX4s3Zk_oClWKxyfxAR1Es,137
 onoffmonitorserver/apps.py,sha256=kPufj7Z9UAxHGq2v6ir3QxPm-vf1R1tKG6o4-CJA_X4,204
 onoffmonitorserver/filters.py,sha256=d1OFS5Mtip2nLS7lvdwtJPrG-ZmfORQjQ8HEl6C4VIo,365
-onoffmonitorserver/models.py,sha256=c_VUi6Obq0QSrA9pu5jpugNz5rQjq1OdPFhuAHNE74k,1689
+onoffmonitorserver/models.py,sha256=_gQvtGv67cTKjEtArumgIwltRWnEPiPsK4TMZXjjRtk,1889
 onoffmonitorserver/permissions.py,sha256=y-dURrhXm4hJorZ8QBsg51ak-cZ1EaDg-KicePa-R24,333
-onoffmonitorserver/serializers.py,sha256=VDB46hx8Thc08QjHVjjONKLyU4JnaK1KW8clNjDEM44,1120
+onoffmonitorserver/serializers.py,sha256=oWHHFOLNdX87p_UX1ExDJ9mZukemQ7ri1gdjKYBqCZY,1135
 onoffmonitorserver/tests.py,sha256=mrbGGRNg5jwbTJtWWa7zSKdDyeB4vmgZCRc2nk6VY-g,60
 onoffmonitorserver/urls.py,sha256=aO7I65KuJTpYyBnWMy7OZEbr4JDfyrpgTnEc5TdAu90,292
-onoffmonitorserver/views.py,sha256=Q6pk_vBQ7OchmDNHylxwY9SwIbsVAqqE8IJBsbH4ua4,2184
+onoffmonitorserver/views.py,sha256=-WwkG8iIoGGIlCGgpw3tf8sQESISJH3j6fvU2LCHFA0,2310
 onoffmonitorserver/migrations/0001_initial.py,sha256=vSqXj4PR2ARTDmmJuJUofWdLH481q30NtR2EFoZCDJs,2205
 onoffmonitorserver/migrations/0002_alter_device_gpio_pin_device_gpio_input_and_more.py,sha256=0nRXSD_okyfTe5kFFXVGyMlOEvI9GfPIcvZGR2X4c9Q,594
+onoffmonitorserver/migrations/0003_monitor_gpio_mode_alter_device_gpio_input.py,sha256=_Hy0QUMn5pse8pk8D0NO8meeMdQTk6yfubJJxWjxzWo,707
 onoffmonitorserver/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-onoffmonitorserver-0.2.0.dist-info/METADATA,sha256=NfQgANXpUu5kklU7pnqy0Rv2PfB3j8PBOPUIftJ1B4M,1061
-onoffmonitorserver-0.2.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-onoffmonitorserver-0.2.0.dist-info/top_level.txt,sha256=To5bX54jTRb2wvSPY4AX9oenfUC4REFMMcWmUuBJdZ4,19
-onoffmonitorserver-0.2.0.dist-info/RECORD,,
+onoffmonitorserver-0.3.0.dist-info/LICENSE,sha256=EauXk7lwd6z-a8bJgvo3A7hc81tjj_NBScbdp-ON9mA,1687
+onoffmonitorserver-0.3.0.dist-info/METADATA,sha256=3oqpVraEYsRcxHjJ8r_YHIL0f3CVMy38kZilUN1jlmk,3036
+onoffmonitorserver-0.3.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+onoffmonitorserver-0.3.0.dist-info/top_level.txt,sha256=To5bX54jTRb2wvSPY4AX9oenfUC4REFMMcWmUuBJdZ4,19
+onoffmonitorserver-0.3.0.dist-info/RECORD,,
```

