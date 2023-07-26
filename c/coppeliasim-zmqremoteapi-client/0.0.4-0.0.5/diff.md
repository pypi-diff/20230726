# Comparing `tmp/coppeliasim_zmqremoteapi_client-0.0.4.tar.gz` & `tmp/coppeliasim_zmqremoteapi_client-0.0.5.tar.gz`

## Comparing `coppeliasim_zmqremoteapi_client-0.0.4.tar` & `coppeliasim_zmqremoteapi_client-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/.flake8
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/opencv.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/pController.py
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/sendIkMovementSequence-mov.py
--rw-r--r--   0        0        0    34145 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/sendIkMovementSequence-pts.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/sendIkMovementSequence-simMoveToPose.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/sendMovementSequence-mov.py
--rw-r--r--   0        0        0     7781 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/sendMovementSequence-pts.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/sendMovementSequence-simMoveToConfig.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/sendSimultan2MovementSequences-mov.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/simpleTest-nonBlocking.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/simpleTest.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/synchronousImageTransmission.py
--rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/src/coppeliasim_zmqremoteapi_client/__init__.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/src/coppeliasim_zmqremoteapi_client/asyncio/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/zmqRemoteApi/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/.gitignore
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/LICENSE
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/README.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/.flake8
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/opencv.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/pController.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/sendIkMovementSequence-mov.py
+-rw-r--r--   0        0        0    34162 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/sendIkMovementSequence-pts.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/sendIkMovementSequence-simMoveToPose.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/sendMovementSequence-mov.py
+-rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/sendMovementSequence-pts.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/sendMovementSequence-simMoveToConfig.py
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/sendSimultan2MovementSequences-mov.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/simpleTest-nonBlocking.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/simpleTest.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/synchronousImageTransmission.py
+-rw-r--r--   0        0        0    14570 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/src/coppeliasim_zmqremoteapi_client/__init__.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/src/coppeliasim_zmqremoteapi_client/asyncio/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/zmqRemoteApi/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/.gitignore
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/README.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 coppeliasim_zmqremoteapi_client-0.0.5/PKG-INFO
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/opencv.py` & `coppeliasim_zmqremoteapi_client-0.0.5/opencv.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 # blocking example, see simpleTest-nonBlocking.py
 
 import time
 
 import numpy as np
 import cv2
 
-from zmqRemoteApi import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client import RemoteAPIClient
 
 
 print('Program started')
 
 client = RemoteAPIClient()
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 visionSensorHandle = sim.getObject('/VisionSensor')
 passiveVisionSensorHandle = sim.getObject('/PassiveVisionSensor')
 
 # When simulation is not running, ZMQ message handling could be a bit
 # slow, since the idle loop runs at 8 Hz by default. So let's make
 # sure that the idle loop runs at full speed for this program:
@@ -32,15 +32,15 @@
 sim.setInt32Param(sim.intparam_idle_fps, 0)
 
 # Run a simulation in stepping mode:
 client.setStepping(True)
 sim.startSimulation()
 
 while (t := sim.getSimulationTime()) < 3:
-    img, resX, resY = sim.getVisionSensorCharImage(visionSensorHandle)
+    img, [resX, resY] = sim.getVisionSensorImg(visionSensorHandle)
     img = np.frombuffer(img, dtype=np.uint8).reshape(resY, resX, 3)
 
     # In CoppeliaSim images are left to right (x-axis), and bottom to top (y-axis)
     # (consistent with the axes of vision sensors, pointing Z outwards, Y up)
     # and color format is RGB triplets, whereas OpenCV uses BGR:
     img = cv2.flip(cv2.cvtColor(img, cv2.COLOR_BGR2RGB), 0)
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/pController.py` & `coppeliasim_zmqremoteapi_client-0.0.5/pController.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 #
 # scenes/messaging/pControllerViaRemoteApi.ttt
 #
 # Do not launch simulation, but run this script
 
 import math
 
-from zmqRemoteApi import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client import RemoteAPIClient
 
 print('Program started')
 
 maxForce = 100
 
 client = RemoteAPIClient()
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 
 def moveToAngle(targetAngle):
     global jointAngle
     while abs(jointAngle - targetAngle) > 0.1 * math.pi / 180:
         vel = computeTargetVelocity(jointAngle, targetAngle)
         sim.setJointTargetVelocity(jointHandle, vel)
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/sendIkMovementSequence-mov.py` & `coppeliasim_zmqremoteapi_client-0.0.5/sendIkMovementSequence-mov.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Make sure to have CoppeliaSim running, with followig scene loaded:
 #
 # scenes/messaging/ikMovementViaRemoteApi.ttt
 #
 # Do not launch simulation, then run this script
 
-from zmqRemoteApi import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client import RemoteAPIClient
 
 print('Program started')
 
 client = RemoteAPIClient()
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 executedMovId = 'notReady'
 targetArm = '/LBR4p'
 stringSignalName = targetArm + '_executedMovId'
 objHandle = sim.getObject(targetArm)
 scriptHandle = sim.getScript(sim.scripttype_childscript,objHandle)
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/sendIkMovementSequence-pts.py` & `coppeliasim_zmqremoteapi_client-0.0.5/sendIkMovementSequence-pts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Make sure to have CoppeliaSim running, with followig scene loaded:
 #
 # scenes/messaging/ikMovementViaRemoteApi.ttt
 #
 # Do not launch simulation, then run this script
 
-from zmqRemoteApi import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client import RemoteAPIClient
 
 print('Program started')
 
 client = RemoteAPIClient()
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 executedMovId = 'notReady'
 
 targetArm = '/LBR4p'
 stringSignalName = targetArm + '_executedMovId'
 objHandle = sim.getObject(targetArm)
 scriptHandle = sim.getScript(sim.scripttype_childscript,objHandle)
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/sendIkMovementSequence-simMoveToPose.py` & `coppeliasim_zmqremoteapi_client-0.0.5/sendIkMovementSequence-simMoveToPose.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Make sure to have CoppeliaSim running, with followig scene loaded:
 #
 # scenes/messaging/ikMovementViaRemoteApi.ttt
 #
 # Do not launch simulation, then run this script
 
-from zmqRemoteApi import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client import RemoteAPIClient
 
 print('Program started')
 
 client = RemoteAPIClient()
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 tipHandle = sim.getObject('/LBR4p/tip')
 targetHandle = sim.getObject('/LBR4p/target')
 
 # Set-up some movement variables:
 maxVel = 0.1
 maxAccel = 0.01
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/sendMovementSequence-mov.py` & `coppeliasim_zmqremoteapi_client-0.0.5/sendMovementSequence-mov.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #
 # scenes/messaging/movementViaRemoteApi.ttt
 #
 # Do not launch simulation, then run this script
 
 import math
 
-from zmqRemoteApi import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client import RemoteAPIClient
 
 print('Program started')
 
 client = RemoteAPIClient()
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 executedMovId = 'notReady'
 
 targetArm = '/blueArm'
 # targetArm = '/redArm'
 
 stringSignalName = targetArm + '_executedMovId'
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/sendMovementSequence-pts.py` & `coppeliasim_zmqremoteapi_client-0.0.5/sendMovementSequence-pts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Make sure to have CoppeliaSim running, with followig scene loaded:
 #
 # scenes/messaging/movementViaRemoteApi.ttt
 #
 # Do not launch simulation, then run this script
 
-from zmqRemoteApi import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client import RemoteAPIClient
 
 print('Program started')
 
 client = RemoteAPIClient()
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 executedMovId = 'notReady'
 
 targetArm = '/blueArm'
 # targetArm = '/redArm'
 
 stringSignalName = targetArm + '_executedMovId'
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/sendMovementSequence-simMoveToConfig.py` & `coppeliasim_zmqremoteapi_client-0.0.5/sendMovementSequence-simMoveToConfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 #
 # scenes/messaging/movementViaRemoteApi.ttt
 #
 # Do not launch simulation, then run this script
 
 import math
 
-from zmqRemoteApi import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client import RemoteAPIClient
 
 def movCallback(config,vel,accel,handles):
     for i in range(len(handles)):
         if sim.getJointMode(handles[i])[0]==sim.jointmode_force and sim.isDynamicallyEnabled(handles[i]):
             sim.setJointTargetPosition(handles[i],config[i])
         else:
             sim.setJointPosition(handles[i],config[i])
 
 print('Program started')
 
 client = RemoteAPIClient()
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 targetArm = '/blueArm'
 # targetArm = '/redArm'
 
 jointHandles=[]
 for i in range(6):
     jointHandles.append(sim.getObject(targetArm+'/joint',{'index':i}))
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/sendSimultan2MovementSequences-mov.py` & `coppeliasim_zmqremoteapi_client-0.0.5/sendSimultan2MovementSequences-mov.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 #
 # scenes/messaging/movementViaRemoteApi.ttt
 #
 # Do not launch simulation, then run this script
 
 import math
 
-from zmqRemoteApi import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client import RemoteAPIClient
 
 print('Program started')
 
 executedMovId1 = 'notReady'
 executedMovId2 = 'notReady'
 
 client = RemoteAPIClient()
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 targetArm1 = '/blueArm'
 targetArm2 = '/redArm'
 
 stringSignalName1 = targetArm1 + '_executedMovId'
 stringSignalName2 = targetArm2 + '_executedMovId'
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/simpleTest-nonBlocking.py` & `coppeliasim_zmqremoteapi_client-0.0.5/simpleTest-nonBlocking.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 #
 # Some CoppeliaSim commands will run in non-blocking mode
 # For a simpler, blocking mode only example, see simpleTest.py
 
 import asyncio
 import sys
 
-from zmqRemoteApi.asyncio import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client.asyncio import RemoteAPIClient
 
 
 async def mainFunc():
     print('Program started')
 
     async with RemoteAPIClient() as client:
-        sim = await client.getObject('sim')
+        sim = await client.require('sim')
 
         # When simulation is not running, ZMQ message handling could be a bit
         # slow, since the idle loop runs at 8 Hz by default. So let's make
         # sure that the idle loop runs at full speed for this program:
         defaultIdlsFps = await sim.getInt32Param(sim.intparam_idle_fps)
         await sim.setInt32Param(sim.intparam_idle_fps, 0)
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/simpleTest.py` & `coppeliasim_zmqremoteapi_client-0.0.5/simpleTest.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 #
 # All CoppeliaSim commands will run in blocking mode (block
 # until a reply from CoppeliaSim is received). For a non-
 # blocking example, see simpleTest-nonBlocking.py
 
 import time
 
-from zmqRemoteApi import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client import RemoteAPIClient
 
 
 print('Program started')
 
 client = RemoteAPIClient()
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 # When simulation is not running, ZMQ message handling could be a bit
 # slow, since the idle loop runs at 8 Hz by default. So let's make
 # sure that the idle loop runs at full speed for this program:
 defaultIdleFps = sim.getInt32Param(sim.intparam_idle_fps)
 sim.setInt32Param(sim.intparam_idle_fps, 0)
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/synchronousImageTransmission.py` & `coppeliasim_zmqremoteapi_client-0.0.5/synchronousImageTransmission.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 # scenes/messaging/synchronousImageTransmissionViaRemoteApi.ttt
 #
 # Do not launch simulation, but run this script
 #
 
 import time
 
-from zmqRemoteApi import RemoteAPIClient
+from coppeliasim_zmqremoteapi_client import RemoteAPIClient
 
 
 print('Program started')
 
 client = RemoteAPIClient()
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 visionSensorHandle = sim.getObject('/VisionSensor')
 passiveVisionSensorHandle = sim.getObject('/PassiveVisionSensor')
 
 client.setStepping(True)
 sim.startSimulation()
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/src/coppeliasim_zmqremoteapi_client/__init__.py` & `coppeliasim_zmqremoteapi_client-0.0.5/src/coppeliasim_zmqremoteapi_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,18 @@
             ret.wait=self._wait
             ret.waitForSignal=self._waitForSignal
             ret.moveToConfig=self._moveToConfig
             ret.moveToPose=self._moveToPose
             self.sim=ret
         return ret
 
+    def require(self, name):
+        self.call('zmqRemoteApi.require', [name])
+        return self.getObject(name)
+
     def setStepping(self, enable=True):
         ret = None
         if self.threadLocLevel > 0:
             self.threadLocLevel = 0
             ret = self.call('setStepping', [False,self.uuid])
         if enable == True:
             self.threadLocLevel = 1
@@ -337,11 +341,11 @@
 
         self._setThreadAutomaticSwitch(lb)
         return outMatrix,timeLeft
 
 
 if __name__ == '__console__':
     client = RemoteAPIClient()
-    sim = client.getObject('sim')
+    sim = client.require('sim')
 
 
 __all__ = ['RemoteAPIClient']
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/src/coppeliasim_zmqremoteapi_client/asyncio/__init__.py` & `coppeliasim_zmqremoteapi_client-0.0.5/src/coppeliasim_zmqremoteapi_client/asyncio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,18 @@
                 setattr(ret, k, lambda *a, func=f'{name}.{k}': self.call(func, a))
             elif len(v) == 1 and 'const' in v:
                 setattr(ret, k, v['const'])
             else:
                 setattr(ret, k, self.getObject(f'{name}.{k}', _info=v))
         return ret
 
+    async def require(self, name):
+        await self.call('zmqRemoteApi.require', [name])
+        return await self.getObject(name)
+
     async def setStepping(self, enable=True):
         return await self.call('setStepping', [enable,self.uuid])
 
     async def step(self, *, wait=True):
         await self.getStepCount(False)
         await self.call('step', [self.uuid])
         await self.getStepCount(wait)
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/LICENSE` & `coppeliasim_zmqremoteapi_client-0.0.5/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 -----------------------------------------------------------------------
-The WS plugin is courtesy of Federico Ferri.
+The python zmqRemoteApi client is courtesy of Federico Ferri.
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/README.md` & `coppeliasim_zmqremoteapi_client-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # create a client to connect to zmqRemoteApi server:
 # (creation arguments can specify different host/port,
 # defaults are host='localhost', port=23000)
 client = RemoteAPIClient()
 
 # get a remote object:
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 # call API function:
 h = sim.getObject('/Floor')
 print(h)
 ```
 
 There is also an `asyncio` version of the client. Normal `asyncio` principles apply, and all methods are async:
@@ -31,15 +31,15 @@
 ```python
 from coppeliasim_zmqremoteapi_client.asyncio import *
 
 client = RemoteAPIClient()
 
 async def main():
     async with RemoteAPIClient() as client:
-        sim = await client.getObject('sim')
+        sim = await client.require('sim')
         h = await sim.getObject('/Floor')
         print(h)
 
 asyncio.run(main())
 ```
 
 on Windows, if it doesn't work properly, before calling `asyncio.run(...)` call:
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/pyproject.toml` & `coppeliasim_zmqremoteapi_client-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "coppeliasim_zmqremoteapi_client"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="Federico Ferri (Coppelia Robotics)", email="federico@coppeliarobotics.com" },
 ]
 description = "Client for the CoppeliaSim's zmqRemoteApi"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `coppeliasim_zmqremoteapi_client-0.0.4/PKG-INFO` & `coppeliasim_zmqremoteapi_client-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coppeliasim_zmqremoteapi_client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Client for the CoppeliaSim's zmqRemoteApi
 Project-URL: Homepage, https://github.com/CoppeliaRobotics/zmqRemoteApi
 Project-URL: Bug Tracker, https://github.com/CoppeliaRobotics/zmqRemoteApi/issues
 Author-email: "Federico Ferri (Coppelia Robotics)" <federico@coppeliarobotics.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
 
 # create a client to connect to zmqRemoteApi server:
 # (creation arguments can specify different host/port,
 # defaults are host='localhost', port=23000)
 client = RemoteAPIClient()
 
 # get a remote object:
-sim = client.getObject('sim')
+sim = client.require('sim')
 
 # call API function:
 h = sim.getObject('/Floor')
 print(h)
 ```
 
 There is also an `asyncio` version of the client. Normal `asyncio` principles apply, and all methods are async:
@@ -47,15 +47,15 @@
 ```python
 from coppeliasim_zmqremoteapi_client.asyncio import *
 
 client = RemoteAPIClient()
 
 async def main():
     async with RemoteAPIClient() as client:
-        sim = await client.getObject('sim')
+        sim = await client.require('sim')
         h = await sim.getObject('/Floor')
         print(h)
 
 asyncio.run(main())
 ```
 
 on Windows, if it doesn't work properly, before calling `asyncio.run(...)` call:
```

