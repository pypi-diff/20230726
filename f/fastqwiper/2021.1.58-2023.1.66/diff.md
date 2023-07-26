# Comparing `tmp/fastqwiper-2021.1.58-py3-none-any.whl.zip` & `tmp/fastqwiper-2023.1.66-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9518 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     1898 b- defN 21-May-13 17:06 fastq_wiper/__init__.py
--rw-rw-rw-  2.0 fat     2078 b- defN 21-May-13 17:06 fastq_wiper/color_log_formatter.py
--rw-rw-rw-  2.0 fat     7467 b- defN 21-May-13 17:06 fastq_wiper/wiper.py
--rw-rw-rw-  2.0 fat     1065 b- defN 21-May-13 17:12 fastqwiper-2021.1.58.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     8480 b- defN 21-May-13 17:12 fastqwiper-2021.1.58.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 21-May-13 17:12 fastqwiper-2021.1.58.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       61 b- defN 21-May-13 17:12 fastqwiper-2021.1.58.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       12 b- defN 21-May-13 17:12 fastqwiper-2021.1.58.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      771 b- defN 21-May-13 17:12 fastqwiper-2021.1.58.dist-info/RECORD
-9 files, 21924 bytes uncompressed, 8176 bytes compressed:  62.7%
+Zip file size: 9548 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     1898 b- defN 23-Jul-26 15:21 fastq_wiper/__init__.py
+-rw-rw-rw-  2.0 fat     2078 b- defN 23-Jul-26 15:21 fastq_wiper/color_log_formatter.py
+-rw-rw-rw-  2.0 fat     7467 b- defN 23-Jul-26 15:21 fastq_wiper/wiper.py
+-rw-rw-rw-  2.0 fat     1065 b- defN 23-Jul-26 15:34 fastqwiper-2023.1.66.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     8661 b- defN 23-Jul-26 15:34 fastqwiper-2023.1.66.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 15:34 fastqwiper-2023.1.66.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       60 b- defN 23-Jul-26 15:34 fastqwiper-2023.1.66.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-26 15:34 fastqwiper-2023.1.66.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      771 b- defN 23-Jul-26 15:34 fastqwiper-2023.1.66.dist-info/RECORD
+9 files, 22104 bytes uncompressed, 8206 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: fastq_wiper/color_log_formatter.py
 Comment: 
 
 Filename: fastq_wiper/wiper.py
 Comment: 
 
-Filename: fastqwiper-2021.1.58.dist-info/LICENSE
+Filename: fastqwiper-2023.1.66.dist-info/LICENSE
 Comment: 
 
-Filename: fastqwiper-2021.1.58.dist-info/METADATA
+Filename: fastqwiper-2023.1.66.dist-info/METADATA
 Comment: 
 
-Filename: fastqwiper-2021.1.58.dist-info/WHEEL
+Filename: fastqwiper-2023.1.66.dist-info/WHEEL
 Comment: 
 
-Filename: fastqwiper-2021.1.58.dist-info/entry_points.txt
+Filename: fastqwiper-2023.1.66.dist-info/entry_points.txt
 Comment: 
 
-Filename: fastqwiper-2021.1.58.dist-info/top_level.txt
+Filename: fastqwiper-2023.1.66.dist-info/top_level.txt
 Comment: 
 
-Filename: fastqwiper-2021.1.58.dist-info/RECORD
+Filename: fastqwiper-2023.1.66.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fastqwiper-2021.1.58.dist-info/LICENSE` & `fastqwiper-2023.1.66.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastqwiper-2021.1.58.dist-info/METADATA` & `fastqwiper-2023.1.66.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,181 +1,179 @@
-Metadata-Version: 2.1
-Name: fastqwiper
-Version: 2021.1.58
-Summary: A package to wipe out uncompliant reads from FASTQ files
-Home-page: https://github.com/mazzalab/fastqwiper
-Author: Tommaso Mazza
-Author-email: bioinformatics@css-mendel.it
-License: MIT
-Project-URL: Source, https://github.com/mazzalab/fastqwiper
-Project-URL: Tracker, https://github.com/mazzalab/fastqwiper/issues
-Project-URL: Developmental plan, https://github.com/mazzalab/fastqwiper/projects
-Keywords: genomics,ngs,fastq,bioinformatics
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: <3.9
-Description-Content-Type: text/markdown
-Requires-Dist: setuptools
-Requires-Dist: colorama (==0.4.4)
-Requires-Dist: click (==7.1.2)
-
-# FastqWiper
-[![Build status](https://ci.appveyor.com/api/projects/status/y09medho67x2nrgn?svg=true)](https://ci.appveyor.com/project/mazzalab/fastqwiper)
-[![GitHub issues](https://img.shields.io/github/issues-raw/mazzalab/fastqwiper)](https://github.com/mazzalab/fastqwiper/issues)
-
-`FastqWiper` is a Python application that wipes out badly formatted reads from readable FASTQ files. 
-
-More complex workflows, as **recover** corrupted `fastq.gz`, **dropping** or **fixing** pesky lines, **removing** 
-unpaired reads, and **fixing** reads interleaving, can be executed using Snakemake and the preconfigured 
-[pipeline files](https://github.com/mazzalab/fastqwiper/tree/main/pipeline) provided here.
-
-* Compatibility: Python <3.9
-* OS: Windows (excluding pipelines), Linux, Mac OS
-* Contributions: [bioinformatics@css-mendel.it](bioinformatics@css-mendel.it)
-* Pypi: https://pypi.org/project/fastqwiper
-* Conda: https://anaconda.org/bfxcss/fastqwiper
-* Docker Hub: available soon
-* Bug report: [https://github.com/mazzalab/fastqwiper/issues](https://github.com/mazzalab/fastqwiper/issues)
-
-
-## Installation
-`FastqWiper` alone can be installed using both Conda and PyPi and runs smoothly on all OS specified above.
-
-### Anaconda or Miniconda
-[![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/version.svg)](https://anaconda.org/bfxcss/fastqwiper) [![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/latest_release_date.svg)](https://anaconda.org/bfxcss/fastqwiper) [![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/platforms.svg)](https://anaconda.org/bfxcss/fastqwiper) [![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/downloads.svg)](https://anaconda.org/bfxcss/fastqwiper)
-
-Create and activate an empty Conda environment, if not already available.<br/>
-```
-$ conda create -n FastqWiper python=3.8
-$ conda activate FastqWiper
-```
-
-then<br/>
-`$ conda install -y -c bfxcss -c conda-forge fastqwiper`
-
-### Pypi
-[![PyPI version](https://badge.fury.io/py/fastqwiper.svg)](https://pypi.org/project/fastqwiper/)
-
-`pip install fastqwiper`
-
-### Usage
-`fastqwiper` `<options>`
-```
-options:
-  --fastq_in TEXT          The input FASTQ file to be cleaned  [required]
-  --fastq_out TEXT         The wiped FASTQ file                [required]
-  --log_frequency INTEGER  The number of processed reads that you want to print a status message after
-```
-It  accepts in input and outputs **readable** `*.fastq` or `*.fastq.gz` files.
-
-
-## Snakemake
-To enable the use of preconfigured [pipelines](https://github.com/mazzalab/fastqwiper/tree/main/pipeline), you need to 
-install **Snakemake**. The recommended way to install Snakemake is via Conda, because it enables **Snakemake** to 
-[handle software dependencies of your workflow](https://snakemake.readthedocs.io/en/stable/snakefiles/deployment.html#integrated-package-management).
-However, the default conda solver is slow and often hangs. Therefore, we recommend 
-installing [Mamba](https://github.com/mamba-org/mamba) as a drop-in replacement via
-
-`$ conda install -c conda-forge mamba`
-
-and then creating and activating a clean environment as above:
-
-```
-$ mamba create -c conda-forge -c bioconda -n FastqWiper snakemake
-$ conda activate FastqWiper
-$ conda install colorama click
-$ conda install mamba -c conda-forge
-```
-
-
-### Usage
-Clone the FastqWiper repository:
-
-`git clone https://github.com/mazzalab/fastqwiper.git`.
-
-It contains, in particular, a folder `data` containing the fastq files to be processed, a folder `pipeline` containing 
-the released pipelines and a folder `fastq_wiper` with the source files of FastqWiper. <br/>
-Input files to be processed should be copied into the **data** folder. All software packages not fetched from `Conda` 
-and used by the pipelines should be copied, even if it is not strictly mandatory, in the root directory of the cloned
-repository. 
-
-Currently, to run the FastqWiper pipelines, the following packages are not included in `Conda` but are 
-required:
-
-### required packages:
-[gzrt](https://github.com/arenn/gzrt) (install [instructions](https://github.com/arenn/gzrt/blob/master/README.build))
-
-[BBTools](https://jgi.doe.gov/data-and-tools/bbtools/) (install [instructions](https://jgi.doe.gov/data-and-tools/bbtools/bb-tools-user-guide/installation-guide/))
-
-```
-$ cd fastqwiper
-$ git clone https://github.com/arenn/gzrt.git
-$ cd gzrt
-$ make
-$ cd ..
-$ cd fastqwiper
-$ tar -xvzf BBMap_(version).tar.gz
-```
-
-### Commands:
-#### Paired-end files
-- **Personalize a pipeline**. Using `fix_wipe_pairs_reads.smk` requires you to edit 
-  line 3 of the file with the name of the fastq files stored in `data` folder that you want to process. 
-  If the files were:
-```
-excerpt_S1_R1_001.fastq.gz
-excerpt_S1_R2_001.fastq.gz
-sample_S1_R1_001.fastq.gz
-sample_S1_R2_001.fastq.gz
-```
-the SAMPLE vector should be: `SAMPLES = ["sample", "excerpt"]`
-
-- **Get a dry run** of a pipeline (e.g., `fix_wipe_pairs_reads.smk`):<br />
-`snakemake -s pipeline/fix_wipe_pairs_reads.smk --use-conda --cores 2 -np`
-
-- **Generate the planned DAG**:<br />
-`snakemake -s pipeline/fix_wipe_pairs_reads.smk --dag | dot -Tpdf > dag.pdf`<br />
-<img src="https://github.com/mazzalab/fastqwiper/blob/main/pipeline/fix_wipe_pairs_reads.png?raw=true" width="400">
-
-- **Run the pipeline** (n.b., during the first execution, Snakemake will download and install some required remote 
-  packages and may take longer). The number of computing cores can be tuned accordingly:<br />
-`snakemake -s pipeline/fix_wipe_pairs_reads.smk --use-conda --cores 2`
-
-Fixed files will be copied in the `data` folder and will be suffixed with the string `_fixed_wiped_paired_interleaving`.
-We remind that the `fix_wipe_pairs_reads.smk` pipeline performs the following actions:
-- execute `gzrt` on corrupted fastq.gz files (i.e., that cannot be unzipped because of errors) and recover readable reads;
-- execute `fastqwiper` on recovered reads to make them compliant with the FASTQ format (source: [Wipipedia](https://en.wikipedia.org/wiki/FASTQ_format))
-- execute `Trimmomatic` on wiped reads to remove residual unpaired reads
-- execute `BBmap (repair.sh)` on paired reads to fix the correct interleaving and sort fastq files.  
-
-#### Single-end files
-Using `fix_wipe_pairs_reads.smk` requires you to make the same edits as above. This pipeline will not execute 
-`trimmomatic` and BBmap's `repair.sh`.
-
-- **Get a dry run** of a pipeline (e.g., `fix_wipe_single_reads.smk`):<br />
-`snakemake -s pipeline/fix_wipe_single_reads.smk --use-conda --cores 2 -np`
-
-- **Generate the planned DAG**:<br />
-`snakemake -s pipeline/fix_wipe_single_reads.smk --dag | dot -Tpdf > dag.pdf`<br />
-<img src="https://github.com/mazzalab/fastqwiper/blob/main/pipeline/fix_wipe_single_reads.png?raw=true" width="200">
-
-- **Run the pipeline** (n.b., during the first execution, Snakemake will download and install some required remote 
-  packages and may take longer). The number of computing cores can be tuned accordingly:<br />
-`snakemake -s pipeline/fix_wipe_single_reads.smk --use-conda --cores 2`
-
-# Author
-**Tommaso Mazza**  
-[![Tweeting](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/irongraft)
-
-Laboratory of Bioinformatics<br/>
-Fondazione IRCCS Casa Sollievo della Sofferenza<br/>
-Viale Regina Margherita 261 - 00198 Roma IT<br/>
-Tel: +39 06 44160526 - Fax: +39 06 44160548<br/>
-E-mail: t.mazza@css-mendel.it <br/>
-Web page: http://www.css-mendel.it <br/>
-Web page: http://bioinformatics.css-mendel.it <br/>
-
-
+Metadata-Version: 2.1
+Name: fastqwiper
+Version: 2023.1.66
+Summary: A package to wipe out uncompliant reads from FASTQ files
+Home-page: https://github.com/mazzalab/fastqwiper
+Author: Tommaso Mazza
+Author-email: bioinformatics@css-mendel.it
+License: MIT
+Project-URL: Source, https://github.com/mazzalab/fastqwiper
+Project-URL: Tracker, https://github.com/mazzalab/fastqwiper/issues
+Project-URL: Developmental plan, https://github.com/mazzalab/fastqwiper/projects
+Keywords: genomics,ngs,fastq,bioinformatics
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: ==3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: colorama (==0.4.6)
+Requires-Dist: click (==8.1.3)
+
+# FastqWiper
+[![Build status](https://ci.appveyor.com/api/projects/status/y09medho67x2nrgn?svg=true)](https://ci.appveyor.com/project/mazzalab/fastqwiper)
+[![GitHub issues](https://img.shields.io/github/issues-raw/mazzalab/fastqwiper)](https://github.com/mazzalab/fastqwiper/issues)
+
+`FastqWiper` is a Python application that wipes out badly formatted reads from readable FASTQ files. 
+
+More complex workflows, as **recover** corrupted `fastq.gz`, **dropping** or **fixing** pesky lines, **removing** 
+unpaired reads, and **fixing** reads interleaving, can be executed using Snakemake and the preconfigured 
+[pipeline files](https://github.com/mazzalab/fastqwiper/tree/main/pipeline) provided here.
+
+* Compatibility: Python 3.8
+* OS: Windows (excluding pipelines), Linux, Mac OS
+* Contributions: [bioinformatics@css-mendel.it](bioinformatics@css-mendel.it)
+* Pypi: https://pypi.org/project/fastqwiper
+* Conda: https://anaconda.org/bfxcss/fastqwiper
+* Docker Hub: available soon
+* Bug report: [https://github.com/mazzalab/fastqwiper/issues](https://github.com/mazzalab/fastqwiper/issues)
+
+
+## Installation
+`FastqWiper` alone can be installed using both Conda and PyPi and runs smoothly on all OS specified above.
+
+### Anaconda or Miniconda
+[![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/version.svg)](https://anaconda.org/bfxcss/fastqwiper) [![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/latest_release_date.svg)](https://anaconda.org/bfxcss/fastqwiper) [![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/platforms.svg)](https://anaconda.org/bfxcss/fastqwiper) [![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/downloads.svg)](https://anaconda.org/bfxcss/fastqwiper)
+
+Create and activate an empty Conda environment, if not already available.<br/>
+```
+$ conda create -n FastqWiper python=3.8
+$ conda activate FastqWiper
+```
+
+then<br/>
+`$ conda install -y -c bfxcss -c conda-forge fastqwiper`
+
+### Pypi
+[![PyPI version](https://badge.fury.io/py/fastqwiper.svg)](https://pypi.org/project/fastqwiper/)
+
+`pip install fastqwiper`
+
+### Usage
+`fastqwiper` `<options>`
+```
+options:
+  --fastq_in TEXT          The input FASTQ file to be cleaned  [required]
+  --fastq_out TEXT         The wiped FASTQ file                [required]
+  --log_frequency INTEGER  The number of processed reads that you want to print a status message after
+```
+It  accepts in input and outputs **readable** `*.fastq` or `*.fastq.gz` files.
+
+
+## Snakemake
+To enable the use of preconfigured [pipelines](https://github.com/mazzalab/fastqwiper/tree/main/pipeline), you need to 
+install **Snakemake**. The recommended way to install Snakemake is via Conda, because it enables **Snakemake** to 
+[handle software dependencies of your workflow](https://snakemake.readthedocs.io/en/stable/snakefiles/deployment.html#integrated-package-management).
+However, the default conda solver is slow and often hangs. Therefore, we recommend 
+installing [Mamba](https://github.com/mamba-org/mamba) as a drop-in replacement via
+
+`$ conda install -c conda-forge mamba`
+
+and then creating and activating a clean environment as above:
+
+```
+$ mamba create -c conda-forge -c bioconda -n FastqWiper snakemake
+$ conda activate FastqWiper
+$ conda install colorama click
+$ conda install mamba -c conda-forge
+```
+
+
+### Usage
+Clone the FastqWiper repository:
+
+`git clone https://github.com/mazzalab/fastqwiper.git`.
+
+It contains, in particular, a folder `data` containing the fastq files to be processed, a folder `pipeline` containing 
+the released pipelines and a folder `fastq_wiper` with the source files of FastqWiper. <br/>
+Input files to be processed should be copied into the **data** folder. All software packages not fetched from `Conda` 
+and used by the pipelines should be copied, even if it is not strictly mandatory, in the root directory of the cloned
+repository. 
+
+Currently, to run the FastqWiper pipelines, the following packages are not included in `Conda` but are 
+required:
+
+### required packages:
+[gzrt](https://github.com/arenn/gzrt) (install [instructions](https://github.com/arenn/gzrt/blob/master/README.build))
+
+[BBTools](https://jgi.doe.gov/data-and-tools/bbtools/) (install [instructions](https://jgi.doe.gov/data-and-tools/bbtools/bb-tools-user-guide/installation-guide/))
+
+```
+$ cd fastqwiper
+$ git clone https://github.com/arenn/gzrt.git
+$ cd gzrt
+$ make
+$ cd ..
+$ cd fastqwiper
+$ tar -xvzf BBMap_(version).tar.gz
+```
+
+### Commands:
+#### Paired-end files
+- **Personalize a pipeline**. Using `fix_wipe_pairs_reads.smk` requires you to edit 
+  line 3 of the file with the name of the fastq files stored in `data` folder that you want to process. 
+  If the files were:
+```
+excerpt_S1_R1_001.fastq.gz
+excerpt_S1_R2_001.fastq.gz
+sample_S1_R1_001.fastq.gz
+sample_S1_R2_001.fastq.gz
+```
+the SAMPLE vector should be: `SAMPLES = ["sample", "excerpt"]`
+
+- **Get a dry run** of a pipeline (e.g., `fix_wipe_pairs_reads.smk`):<br />
+`snakemake -s pipeline/fix_wipe_pairs_reads.smk --use-conda --cores 2 -np`
+
+- **Generate the planned DAG**:<br />
+`snakemake -s pipeline/fix_wipe_pairs_reads.smk --dag | dot -Tpdf > dag.pdf`<br />
+<img src="https://github.com/mazzalab/fastqwiper/blob/main/pipeline/fix_wipe_pairs_reads.png?raw=true" width="400">
+
+- **Run the pipeline** (n.b., during the first execution, Snakemake will download and install some required remote 
+  packages and may take longer). The number of computing cores can be tuned accordingly:<br />
+`snakemake -s pipeline/fix_wipe_pairs_reads.smk --use-conda --cores 2`
+
+Fixed files will be copied in the `data` folder and will be suffixed with the string `_fixed_wiped_paired_interleaving`.
+We remind that the `fix_wipe_pairs_reads.smk` pipeline performs the following actions:
+- execute `gzrt` on corrupted fastq.gz files (i.e., that cannot be unzipped because of errors) and recover readable reads;
+- execute `fastqwiper` on recovered reads to make them compliant with the FASTQ format (source: [Wipipedia](https://en.wikipedia.org/wiki/FASTQ_format))
+- execute `Trimmomatic` on wiped reads to remove residual unpaired reads
+- execute `BBmap (repair.sh)` on paired reads to fix the correct interleaving and sort fastq files.  
+
+#### Single-end files
+Using `fix_wipe_pairs_reads.smk` requires you to make the same edits as above. This pipeline will not execute 
+`trimmomatic` and BBmap's `repair.sh`.
+
+- **Get a dry run** of a pipeline (e.g., `fix_wipe_single_reads.smk`):<br />
+`snakemake -s pipeline/fix_wipe_single_reads.smk --use-conda --cores 2 -np`
+
+- **Generate the planned DAG**:<br />
+`snakemake -s pipeline/fix_wipe_single_reads.smk --dag | dot -Tpdf > dag.pdf`<br />
+<img src="https://github.com/mazzalab/fastqwiper/blob/main/pipeline/fix_wipe_single_reads.png?raw=true" width="200">
+
+- **Run the pipeline** (n.b., during the first execution, Snakemake will download and install some required remote 
+  packages and may take longer). The number of computing cores can be tuned accordingly:<br />
+`snakemake -s pipeline/fix_wipe_single_reads.smk --use-conda --cores 2`
+
+# Author
+**Tommaso Mazza**  
+[![Tweeting](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/irongraft)
+
+Laboratory of Bioinformatics<br/>
+Fondazione IRCCS Casa Sollievo della Sofferenza<br/>
+Viale Regina Margherita 261 - 00198 Roma IT<br/>
+Tel: +39 06 44160526 - Fax: +39 06 44160548<br/>
+E-mail: t.mazza@css-mendel.it <br/>
+Web page: http://www.css-mendel.it <br/>
+Web page: http://bioinformatics.css-mendel.it <br/>
```

