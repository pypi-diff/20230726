# Comparing `tmp/fajrGPT-1.4.5.tar.gz` & `tmp/fajrGPT-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.4.5.tar", last modified: Tue Jul 25 13:04:51 2023, max compression
+gzip compressed data, was "fajrGPT-1.4.6.tar", last modified: Wed Jul 26 10:48:41 2023, max compression
```

## Comparing `fajrGPT-1.4.5.tar` & `fajrGPT-1.4.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-25 13:04:51.058085 fajrGPT-1.4.5/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.5/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-25 13:04:51.057912 fajrGPT-1.4.5/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.5/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-25 13:04:51.056354 fajrGPT-1.4.5/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.5/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.5/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    18434 2023-07-25 10:13:28.000000 fajrGPT-1.4.5/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-25 13:04:51.057708 fajrGPT-1.4.5/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-25 13:04:51.058126 fajrGPT-1.4.5/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-25 13:04:41.000000 fajrGPT-1.4.5/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-26 10:48:41.474101 fajrGPT-1.4.6/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.6/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-26 10:48:41.473473 fajrGPT-1.4.6/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.6/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-26 10:48:41.472072 fajrGPT-1.4.6/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.6/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.6/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    19125 2023-07-26 10:47:03.000000 fajrGPT-1.4.6/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-26 10:48:41.473280 fajrGPT-1.4.6/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-26 10:48:41.474165 fajrGPT-1.4.6/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-26 10:47:18.000000 fajrGPT-1.4.6/setup.py
```

### Comparing `fajrGPT-1.4.5/LICENSE` & `fajrGPT-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.5/PKG-INFO` & `fajrGPT-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.5
+Version: 1.4.6
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.5/README.md` & `fajrGPT-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.5/fajrGPT/quran_metadata.py` & `fajrGPT-1.4.6/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.5/fajrGPT/wake.py` & `fajrGPT-1.4.6/fajrGPT/wake.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 @click.command()
 @click.option('--url', required=True, help='YouTube URL containing desired audio data.')
 @click.option('--time', required=True, help='Countdown time in format [number][h/m/s], i.e. 1h would create a 1 hour timer.')
 @click.option('--output', required=True, help='Name of the output file.')
 @click.option('--names-flag', required=False, help='Whether or not to include a randomly selected name of Allah in the preamble.', default=True)
 @click.option('--transition-time', required=False, help='Time in seconds for the transition between the output audio and the Quran verses.', default=600)
 @click.option('--surah', required=False, help='Specific Surah from the Quran. Should be given as integer.')
+# TODO: add option for including english translation of each surah if the user selects the surah option. Perhaps use a natural language generation model to generate the translation from the english translation of the Quran verses.
 
 def main(url, time, output, names_flag, transition_time=600, surah=None):
     # Check surah option
     if surah:
         # make the output file name the same as the surah
         output = 'quran-' + '{:03d}'.format(int(surah))
         flag = download_surah(surah, output)
@@ -100,14 +101,21 @@
 
     return True    
 
 def play_quran_verses_audio(verses,transition_time=0.5):
     # convert verses to urls
     urls = [quran_verse_to_mp3_url(verse) for verse in verses]
 
+    # TODO: find mp3 url for the english translation of each verse and append it to the urls list depending on an option the user selects
+    # if include_english_translation:
+    ## if insert_translation_after_verse:
+    ### urls.append(english_translation_url)
+    ## elif insert_translation_within_verse:
+    ### urls.insert(1,english_translation_url)
+
     # download the verse audio
     file_paths = [download_file_and_sleep(url,0.5) for url in urls]
 
     # concatenate the audio files into one
     combined_audio_file_name = combine_audio_from_files(file_paths)
 
     # delete the temporary files
@@ -231,15 +239,16 @@
 
         # Get the transliteration of the name of Allah
         name_of_allah_transliteration = allah_transliterations[index]
 
         # Get the explanation of the name of Allah using a GPT-3 model prompt
         prompt = f"""
 
-        For the name of Allah below, please do the following: First break down the word into its root letters, giving their approximate equivalent in the english language. Then, using the root letters, try to guess the meaning of the name. Finally, give a brief explanation of the significane of this particular name of Allah as it relates to the Quran.
+        For the name of Allah below, please do the following: First break down the word into its root letters and also identify the corresponding Arabic letter for each phonetic sound, giving their approximate equivalent in the english language.
+        Then, using the root letters, try to guess the meaning of the name. Finally, give a brief explanation of the significane of this particular name of Allah as it relates to the Quran.
         
         Name of Allah: {name_of_allah_arabic}\nExplanation: 
         
         """
 
         # Get the explanation of the name of Allah
         explanation = query_gpt(prompt)
@@ -265,15 +274,15 @@
     # initialize the verse_texts output and explanations output
     verse_texts = []
     explanations = []
 
     # Get the explanations
     for i, verse_info in enumerate(zip(verses_Quran_Module, verses)):
         verse_QM, verse = verse_info
-        verse_text = Project_Quran().Get_Ayah_English(verse_QM).split('"')[1][0:-1]
+        verse_text = Project_Quran().Get_Ayah_English(verse_QM).split('"')[1][0:-1].replace("&quot;",'"')
         chapter_number = verse.split(':')[0]
         if i == 0:
             prompt2 = f"""
             I want you to act as Sheikh Hamza Yusuf. You are an influential Islamic scholar, who has a profound understanding of the Qur'an, Hadith, and various branches of Islamic Jurisprudence. 
             You are deeply conversant with the various cultural, historical, and philosophical contexts of Islamic thought. You are committed to promoting peace, understanding, and the intellectual tradition of Islam. 
             I know that you are just an AI, but I don't want you to say that at the beginning, just emulate this description to the best of your ability. My first request is as follows:
```

### Comparing `fajrGPT-1.4.5/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.4.6/fajrGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.5
+Version: 1.4.6
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.5/setup.py` & `fajrGPT-1.4.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.4.5",
+    version="1.4.6",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

