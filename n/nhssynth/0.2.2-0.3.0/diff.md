# Comparing `tmp/nhssynth-0.2.2.tar.gz` & `tmp/nhssynth-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhssynth-0.2.2.tar", max compression
+gzip compressed data, was "nhssynth-0.3.0.tar", max compression
```

## Comparing `nhssynth-0.2.2.tar` & `nhssynth-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,43 @@
--rw-r--r--   0        0        0     1068 2023-03-31 11:03:40.629205 nhssynth-0.2.2/LICENSE
--rw-r--r--   0        0        0     6290 2023-04-05 14:58:26.929685 nhssynth-0.2.2/README.md
--rw-r--r--   0        0        0     1438 2023-04-13 19:25:28.430793 nhssynth-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.2.2/src/nhssynth/cli/__init__.py
--rw-r--r--   0        0        0     2690 2023-04-12 17:47:54.764686 nhssynth-0.2.2/src/nhssynth/cli/common_arguments.py
--rw-r--r--   0        0        0     8743 2023-04-13 12:22:56.987449 nhssynth-0.2.2/src/nhssynth/cli/config.py
--rw-r--r--   0        0        0     7024 2023-04-13 13:06:51.351173 nhssynth-0.2.2/src/nhssynth/cli/module_arguments.py
--rw-r--r--   0        0        0     6968 2023-04-13 17:46:22.769683 nhssynth-0.2.2/src/nhssynth/cli/module_setup.py
--rw-r--r--   0        0        0     1409 2023-04-13 13:03:16.862839 nhssynth-0.2.2/src/nhssynth/cli/run.py
--rw-r--r--   0        0        0       82 2023-04-04 13:59:35.254031 nhssynth-0.2.2/src/nhssynth/common/__init__.py
--rw-r--r--   0        0        0      292 2023-04-13 15:21:59.569403 nhssynth-0.2.2/src/nhssynth/common/common.py
--rw-r--r--   0        0        0     3339 2023-04-13 09:38:21.025865 nhssynth-0.2.2/src/nhssynth/common/constants.py
--rw-r--r--   0        0        0     2078 2023-04-04 13:59:35.254363 nhssynth-0.2.2/src/nhssynth/common/dicts.py
--rw-r--r--   0        0        0     2953 2023-04-12 15:31:20.079017 nhssynth-0.2.2/src/nhssynth/common/io.py
--rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.2.2/src/nhssynth/modules/__init__.py
--rw-r--r--   0        0        0       20 2023-03-06 16:05:17.363712 nhssynth-0.2.2/src/nhssynth/modules/dataloader/__init__.py
--rw-r--r--   0        0        0     4082 2023-04-12 15:32:23.986086 nhssynth-0.2.2/src/nhssynth/modules/dataloader/io.py
--rw-r--r--   0        0        0     5253 2023-04-12 15:46:13.535858 nhssynth-0.2.2/src/nhssynth/modules/dataloader/metadata.py
--rw-r--r--   0        0        0    20232 2023-04-13 16:21:20.147258 nhssynth-0.2.2/src/nhssynth/modules/dataloader/metatransformer.py
--rw-r--r--   0        0        0     1596 2023-04-13 12:33:38.185534 nhssynth-0.2.2/src/nhssynth/modules/dataloader/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.2.2/src/nhssynth/modules/evaluation/__init__.py
--rw-r--r--   0        0        0    14078 2023-04-13 17:25:24.470481 nhssynth-0.2.2/src/nhssynth/modules/evaluation/full_report.py
--rw-r--r--   0        0        0     2644 2023-04-13 10:57:28.285918 nhssynth-0.2.2/src/nhssynth/modules/evaluation/io.py
--rw-r--r--   0        0        0     3031 2023-04-11 16:04:10.935343 nhssynth-0.2.2/src/nhssynth/modules/evaluation/metrics.py
--rw-r--r--   0        0        0     1856 2023-04-13 15:24:02.908325 nhssynth-0.2.2/src/nhssynth/modules/evaluation/run.py
--rw-r--r--   0        0        0     8614 2023-04-13 16:21:55.328798 nhssynth-0.2.2/src/nhssynth/modules/model/DPVAE.py
--rw-r--r--   0        0        0       21 2023-03-07 10:57:59.963528 nhssynth-0.2.2/src/nhssynth/modules/model/__init__.py
--rw-r--r--   0        0        0     3092 2023-04-12 15:33:11.172294 nhssynth-0.2.2/src/nhssynth/modules/model/io.py
--rw-r--r--   0        0        0     3510 2023-04-13 16:21:44.533892 nhssynth-0.2.2/src/nhssynth/modules/model/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.2.2/src/nhssynth/modules/plotting/__init__.py
--rw-r--r--   0        0        0     2611 2023-04-13 11:19:38.014249 nhssynth-0.2.2/src/nhssynth/modules/plotting/io.py
--rw-r--r--   0        0        0     6421 2023-04-13 19:24:58.843577 nhssynth-0.2.2/src/nhssynth/modules/plotting/plots.py
--rw-r--r--   0        0        0      727 2023-04-13 12:33:18.866696 nhssynth-0.2.2/src/nhssynth/modules/plotting/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.2.2/src/nhssynth/modules/structure/__init__.py
--rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.2.2/src/nhssynth/modules/structure/run.py
--rw-r--r--   0        0        0     7605 1970-01-01 00:00:00.000000 nhssynth-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-31 11:03:40.629205 nhssynth-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7937 2023-04-26 19:31:33.655713 nhssynth-0.3.0/README.md
+-rw-r--r--   0        0        0     1473 2023-04-26 19:31:59.711829 nhssynth-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.3.0/src/nhssynth/cli/__init__.py
+-rw-r--r--   0        0        0     3437 2023-04-26 19:31:33.656962 nhssynth-0.3.0/src/nhssynth/cli/common_arguments.py
+-rw-r--r--   0        0        0     8878 2023-04-26 19:31:33.657342 nhssynth-0.3.0/src/nhssynth/cli/config.py
+-rw-r--r--   0        0        0     1826 2023-04-26 19:31:33.657526 nhssynth-0.3.0/src/nhssynth/cli/model_arguments.py
+-rw-r--r--   0        0        0     6768 2023-04-26 19:31:33.657824 nhssynth-0.3.0/src/nhssynth/cli/module_arguments.py
+-rw-r--r--   0        0        0     7416 2023-04-26 19:31:33.658068 nhssynth-0.3.0/src/nhssynth/cli/module_setup.py
+-rw-r--r--   0        0        0     1396 2023-04-26 19:31:33.658300 nhssynth-0.3.0/src/nhssynth/cli/run.py
+-rw-r--r--   0        0        0       82 2023-04-04 13:59:35.254031 nhssynth-0.3.0/src/nhssynth/common/__init__.py
+-rw-r--r--   0        0        0      354 2023-04-26 19:31:33.658538 nhssynth-0.3.0/src/nhssynth/common/common.py
+-rw-r--r--   0        0        0     3613 2023-04-26 19:31:33.658743 nhssynth-0.3.0/src/nhssynth/common/constants.py
+-rw-r--r--   0        0        0      376 2023-04-26 19:31:33.658992 nhssynth-0.3.0/src/nhssynth/common/debugging.py
+-rw-r--r--   0        0        0     2132 2023-04-18 15:14:18.123813 nhssynth-0.3.0/src/nhssynth/common/dicts.py
+-rw-r--r--   0        0        0     3119 2023-04-26 19:31:33.659233 nhssynth-0.3.0/src/nhssynth/common/io.py
+-rw-r--r--   0        0        0      582 2023-04-26 19:31:33.659388 nhssynth-0.3.0/src/nhssynth/common/strings.py
+-rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.3.0/src/nhssynth/modules/__init__.py
+-rw-r--r--   0        0        0       20 2023-03-06 16:05:17.363712 nhssynth-0.3.0/src/nhssynth/modules/dataloader/__init__.py
+-rw-r--r--   0        0        0     4082 2023-04-12 15:32:23.986086 nhssynth-0.3.0/src/nhssynth/modules/dataloader/io.py
+-rw-r--r--   0        0        0     5253 2023-04-12 15:46:13.535858 nhssynth-0.3.0/src/nhssynth/modules/dataloader/metadata.py
+-rw-r--r--   0        0        0    16743 2023-04-26 19:31:33.659686 nhssynth-0.3.0/src/nhssynth/modules/dataloader/metatransformer.py
+-rw-r--r--   0        0        0     1347 2023-04-26 19:31:33.659921 nhssynth-0.3.0/src/nhssynth/modules/dataloader/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.3.0/src/nhssynth/modules/evaluation/__init__.py
+-rw-r--r--   0        0        0    14071 2023-04-26 19:31:33.660200 nhssynth-0.3.0/src/nhssynth/modules/evaluation/full_report.py
+-rw-r--r--   0        0        0     2644 2023-04-13 10:57:28.285918 nhssynth-0.3.0/src/nhssynth/modules/evaluation/io.py
+-rw-r--r--   0        0        0     3031 2023-04-11 16:04:10.935343 nhssynth-0.3.0/src/nhssynth/modules/evaluation/metrics.py
+-rw-r--r--   0        0        0     1835 2023-04-26 19:31:33.660620 nhssynth-0.3.0/src/nhssynth/modules/evaluation/run.py
+-rw-r--r--   0        0        0       48 2023-04-26 19:31:33.660900 nhssynth-0.3.0/src/nhssynth/modules/model/__init__.py
+-rw-r--r--   0        0        0     4379 2023-04-26 19:31:33.661089 nhssynth-0.3.0/src/nhssynth/modules/model/common/DPMixin.py
+-rw-r--r--   0        0        0     6407 2023-04-26 19:31:33.661275 nhssynth-0.3.0/src/nhssynth/modules/model/common/Model.py
+-rw-r--r--   0        0        0     3447 2023-04-26 19:31:33.661529 nhssynth-0.3.0/src/nhssynth/modules/model/io.py
+-rw-r--r--   0        0        0     1648 2023-04-26 19:31:33.661707 nhssynth-0.3.0/src/nhssynth/modules/model/models/DPVAE.py
+-rw-r--r--   0        0        0     9881 2023-04-26 19:31:33.661896 nhssynth-0.3.0/src/nhssynth/modules/model/models/VAE.py
+-rw-r--r--   0        0        0      129 2023-04-26 19:31:33.662043 nhssynth-0.3.0/src/nhssynth/modules/model/models/__init__.py
+-rw-r--r--   0        0        0     2221 2023-04-26 19:31:33.662267 nhssynth-0.3.0/src/nhssynth/modules/model/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.3.0/src/nhssynth/modules/plotting/__init__.py
+-rw-r--r--   0        0        0     2611 2023-04-13 11:19:38.014249 nhssynth-0.3.0/src/nhssynth/modules/plotting/io.py
+-rw-r--r--   0        0        0     6421 2023-04-13 19:24:58.843577 nhssynth-0.3.0/src/nhssynth/modules/plotting/plots.py
+-rw-r--r--   0        0        0      727 2023-04-13 12:33:18.866696 nhssynth-0.3.0/src/nhssynth/modules/plotting/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.3.0/src/nhssynth/modules/structure/__init__.py
+-rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.3.0/src/nhssynth/modules/structure/run.py
+-rw-r--r--   0        0        0     9241 1970-01-01 00:00:00.000000 nhssynth-0.3.0/PKG-INFO
```

### Comparing `nhssynth-0.2.2/LICENSE` & `nhssynth-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.2/README.md` & `nhssynth-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -15,77 +15,96 @@
 <!-- PROJECT LOGO -->
 <div align="center">
   <a href="https://nhsx.github.io/NHSSynth">
     <img src="docs/assets/NHS.svg" alt="Logo" width="200" height="100">
   </a>
   <p align="center">
     <a href="https://nhsx.github.io/NHSSynth"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
+    <br /><br /><br />
   </p>
 </div>
 
 # NHS Synth
 
-## About the Project
+## About
 
-The project currently consists of a Python package alongside research and investigative materials covering the effectiveness of the package and synthetic data more generally when applied to NHS use cases.
-
-[Project Description - Synthetic Data Exploration: Variational Autoencoders](https://nhsx.github.io/nhsx-internship-projects/synthetic-data-exploration-vae/)
-
-The codebase builds on previous NHSX Analytics Unit PhD internships contextualising and investigating the potential use of Variational Auto Encoders (VAEs) for synthetic data generation. These were undertaken by Dominic Danks and David Brind.
+This repository currently consists of a Python package alongside research and investigative materials covering the effectiveness of the package and synthetic data more generally when applied to NHS use cases. See the internal [project description](https://nhsx.github.io/nhsx-internship-projects/synthetic-data-exploration-vae/) for more information.
 
 _**Note:** No data, public or private are shared in this repository._
 
 ## Getting Started
 
 ### Project Structure
 
-- The main package and codebase is found in `src/nhssynth` (see Usage below for more information)
-- Accompanying materials are available in the `docs` folder:
-  - A [report](reports/report.pdf) summarising the previous iteration of this project
-  - A [model card](model_card.md) providing more information about the VAE with Differential Privacy
-- Numerous [exemplar configurations](../config) are found in `config`
-- Empty `data` and `experiments` folders are provided; these are the default locations for inputs and outputs when running the project using the provided [`cli`](../src/nhssynth/cli/) module
+- The main package and codebase is found in [`src/nhssynth`](src/nhssynth/) (see [Usage](#usage) below for more information)
+- Accompanying materials are available in the [`docs`](docs/) folder:
+  - The components used to create the GitHub Pages [documentation site](https://nhsx.github.io/NHSSynth/)
+  - A [report](docs/reports/report.pdf) summarising the previous iteration of this project
+  - A [model card](docs/model_card.md) providing more information about the VAE with Differential Privacy
+- Numerous exemplar configurations are found in [`config`](config/)
+- Empty [`data`](data/) and [`experiments`](experiments/) folders are provided; these are the default locations for inputs and outputs when running the project using the provided [CLI](../src/nhssynth/cli/) module
 - Pre-processing notebooks for specific datasets used to assess the approach and other non-core code can be found in [`auxiliary`](../auxiliary/)
 
 ### Installation
 
-As it stands, we recommend the following steps to reproduce our experiments and fully work with this project:
+For general usage, we recommend installing the package via `pip install nhssynth` in a supported python version environment. You can then `import` the package's [modules](src/nhssynth/modules/) and use them in your projects, or interact with the package directly via the [CLI](src/nhssynth/cli/), which is accessed using the `nhssynth` command (see [Usage](#usage) for more information).
+
+#### Secure Mode
+
+Note that in order to train a generator in *secure mode* (see the [documentation](https://nhsx.github.io/NHSSynth/secure_mode/) for details) you will need to install the PyTorch extension package [`csprng`](https://github.com/pytorch/csprng) separately. Currently this package's dependencies are not compatible with recent versions of PyTorch (the author's plan on rectifying this - watch this space), so you will need to install it manually; for this we recommend following the instructions below:
+
+```bash
+git clone git@github.com:pytorch/csprng.git
+cd csprng
+git branch release "v0.2.2-rc1"
+git checkout release
+python setup.py install
+```
+
+#### Advanced Usage
+
+If you intend on contributing or working with the codebase directly, or if you want to reproduce the results of this project, follow the steps below:
 
 1. Clone the repo
 2. Ensure one of the required versions of Python is installed
 3. Install [`poetry`](https://python-poetry.org/docs/#installation)
 4. Instantiate a virtual environment, e.g. via `python -m venv nhssynth`
 3. Activate the virtual environment, e.g. via `source nhssynth/bin/activate`
-4. Install project dependencies with `poetry install` (optionally install `jupyter` and `notebook` to work with some of the preprocessing files in [`auxiliary`](auxiliary/))
-5. Interact with the package in one of two ways:
-    - Via the [`cli`](src/nhssynth/cli/) module using `poetry run cli`
-    - Through building the package with `poetry build` and using it in an existing project (`import nhssynth`). However, if you intend on doing the latter it may be preferable to instead follow the second, simpler setup below.
+4. Install the project dependencies with `poetry install` (optionally install the dev dependencies `--with dev` to work with the [auxiliary notebooks](auxiliary/), or `--with docs` to work with the [documentation](docs/))
+5. You can then interact with the package in one of two ways:
+    - Via the [CLI](src/nhssynth/cli/) module using `nhssynth ...`
+    - Through building the package with `poetry build` and using it in an existing project (`import nhssynth`). You can then actively develop the package and test it.
 
-For more standard usage of the package:
+### Usage
 
-1. Run `pip install nhssynth` within a supported Python installation
-2. Use the modules exported by the package as you would any other. _Note that in this setup you will have to work more closely with the configuration and code to ensure you are handling inputs and outputs for each module appropriately. The cli handles a lot of this complexity, and interacting with the modules directly is considered advanced usage._
+This package comprises a set of modules that can be run individually, as part of a pipeline, or via a configuration file. These options are available via the `nhssynth` command:
 
-### Usage
+```
+nhssynth <module name> --<args>
+nhssynth pipeline --<args>
+nhssynth config -c <name> --<overrides>
+```
 
-This package comprises a pipeline that is runnable via `poetry run cli pipeline <args>` or `poetry run cli config <config filepath>`. You can run the modules that make up this pipeline independently via `poetry run cli <module name>`. To see the modules that are available and their corresponding arguments and function, run `poetry run cli --help` / `poetry run cli <module name> --help`.
+To see the modules that are available and their corresponding arguments, run `nhssynth --help` and `nhssynth <module name> --help` respectively.
+
+Configuration files can be used to run the pipeline or a chosen set of modules. They should be placed in the [`config`](config/) folder and their layout should match that of the examples provided. They can be run as in the latter case above by providing their filename (without the `.yaml` extension). You can also override any of the arguments provided in the configuration file by passing them as arguments in the command line.
+
+To ensure reproducibility, you should always specify a `--seed` value and provide the `--save-config` flag to dump the exact configuration specified / inferred for the run. This configuration file can then be used in the future to reproduce the exact same run or shared with others to run the same configuration on their dataset, etc.
 
 The figure below shows the structure and workflow of the package and its modules.
 
 ![](docs/modules.png)
 
 ### Roadmap
 
 See the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of proposed features (and known issues).
 
 ### Contributing
 
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+Any contributions you wish to make are **greatly appreciated**, we encourage you to first raise an issue to discuss with the maintainers. If you are interested in contributing, please follow these steps:
 
 1. Fork the project
 2. Create your branch (`git checkout -b <yourusername>/<featurename>`)
 3. Commit your changes (`git commit -m 'Add some amazing feature'`)
 4. Push to the branch (`git push origin <yourusername>/<featurename>`)
 5. Open a PR and we will try to get it merged!
 
@@ -95,14 +114,16 @@
 
 <div align="center">
 <a href="https://github.com/nhsx/nhssynth/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=nhsx/nhssynth" />
 </a>
 </div>
 
+This codebase builds on previous NHSX Analytics Unit PhD internships contextualising and investigating the potential use of Variational Auto Encoders (VAEs) for synthetic data generation. These were undertaken by Dominic Danks and David Brind.
+
 ### License
 
 Distributed under the MIT License. _See [LICENSE](./LICENSE) for more information._
 
 ### Contact
 
 This project is under active development by [@HarrisonWilde](https://github.com/HarrisonWilde), for any questions or security concerns [contact him](mailto:h.wilde@warwick.ac.uk) or [raise an issue](https://github.com/nhsx/NHSSynth/issues/new/choose). Alternatively, contact [NHS England TDAU](mailto:england.tdau@nhs.net).
```

#### html2text {}

```diff
@@ -9,71 +9,93 @@
   github.com/nhsx/nhssynth/blob/main/LICENSE) [![Code style: black](https://
   img.shields.io/badge/code%20style-black-000000?style=flat-square)](https://
     github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat-square)](https://pycqa.github.io/isort/)
                                     [Logo]
                              Explore_the_docs_Â»
 
-# NHS Synth ## About the Project The project currently consists of a Python
-package alongside research and investigative materials covering the
-effectiveness of the package and synthetic data more generally when applied to
-NHS use cases. [Project Description - Synthetic Data Exploration: Variational
-Autoencoders](https://nhsx.github.io/nhsx-internship-projects/synthetic-data-
-exploration-vae/) The codebase builds on previous NHSX Analytics Unit PhD
-internships contextualising and investigating the potential use of Variational
-Auto Encoders (VAEs) for synthetic data generation. These were undertaken by
-Dominic Danks and David Brind. _**Note:** No data, public or private are shared
-in this repository._ ## Getting Started ### Project Structure - The main
-package and codebase is found in `src/nhssynth` (see Usage below for more
-information) - Accompanying materials are available in the `docs` folder: - A
-[report](reports/report.pdf) summarising the previous iteration of this project
-- A [model card](model_card.md) providing more information about the VAE with
-Differential Privacy - Numerous [exemplar configurations](../config) are found
-in `config` - Empty `data` and `experiments` folders are provided; these are
-the default locations for inputs and outputs when running the project using the
-provided [`cli`](../src/nhssynth/cli/) module - Pre-processing notebooks for
-specific datasets used to assess the approach and other non-core code can be
-found in [`auxiliary`](../auxiliary/) ### Installation As it stands, we
-recommend the following steps to reproduce our experiments and fully work with
-this project: 1. Clone the repo 2. Ensure one of the required versions of
-Python is installed 3. Install [`poetry`](https://python-poetry.org/docs/
-#installation) 4. Instantiate a virtual environment, e.g. via `python -m venv
-nhssynth` 3. Activate the virtual environment, e.g. via `source nhssynth/bin/
-activate` 4. Install project dependencies with `poetry install` (optionally
-install `jupyter` and `notebook` to work with some of the preprocessing files
-in [`auxiliary`](auxiliary/)) 5. Interact with the package in one of two ways:
-- Via the [`cli`](src/nhssynth/cli/) module using `poetry run cli` - Through
+
+# NHS Synth ## About This repository currently consists of a Python package
+alongside research and investigative materials covering the effectiveness of
+the package and synthetic data more generally when applied to NHS use cases.
+See the internal [project description](https://nhsx.github.io/nhsx-internship-
+projects/synthetic-data-exploration-vae/) for more information. _**Note:** No
+data, public or private are shared in this repository._ ## Getting Started ###
+Project Structure - The main package and codebase is found in [`src/nhssynth`]
+(src/nhssynth/) (see [Usage](#usage) below for more information) - Accompanying
+materials are available in the [`docs`](docs/) folder: - The components used to
+create the GitHub Pages [documentation site](https://nhsx.github.io/NHSSynth/
+) - A [report](docs/reports/report.pdf) summarising the previous iteration of
+this project - A [model card](docs/model_card.md) providing more information
+about the VAE with Differential Privacy - Numerous exemplar configurations are
+found in [`config`](config/) - Empty [`data`](data/) and [`experiments`]
+(experiments/) folders are provided; these are the default locations for inputs
+and outputs when running the project using the provided [CLI](../src/nhssynth/
+cli/) module - Pre-processing notebooks for specific datasets used to assess
+the approach and other non-core code can be found in [`auxiliary`](../
+auxiliary/) ### Installation For general usage, we recommend installing the
+package via `pip install nhssynth` in a supported python version environment.
+You can then `import` the package's [modules](src/nhssynth/modules/) and use
+them in your projects, or interact with the package directly via the [CLI](src/
+nhssynth/cli/), which is accessed using the `nhssynth` command (see [Usage]
+(#usage) for more information). #### Secure Mode Note that in order to train a
+generator in *secure mode* (see the [documentation](https://nhsx.github.io/
+NHSSynth/secure_mode/) for details) you will need to install the PyTorch
+extension package [`csprng`](https://github.com/pytorch/csprng) separately.
+Currently this package's dependencies are not compatible with recent versions
+of PyTorch (the author's plan on rectifying this - watch this space), so you
+will need to install it manually; for this we recommend following the
+instructions below: ```bash git clone git@github.com:pytorch/csprng.git cd
+csprng git branch release "v0.2.2-rc1" git checkout release python setup.py
+install ``` #### Advanced Usage If you intend on contributing or working with
+the codebase directly, or if you want to reproduce the results of this project,
+follow the steps below: 1. Clone the repo 2. Ensure one of the required
+versions of Python is installed 3. Install [`poetry`](https://python-
+poetry.org/docs/#installation) 4. Instantiate a virtual environment, e.g. via
+`python -m venv nhssynth` 3. Activate the virtual environment, e.g. via `source
+nhssynth/bin/activate` 4. Install the project dependencies with `poetry
+install` (optionally install the dev dependencies `--with dev` to work with the
+[auxiliary notebooks](auxiliary/), or `--with docs` to work with the
+[documentation](docs/)) 5. You can then interact with the package in one of two
+ways: - Via the [CLI](src/nhssynth/cli/) module using `nhssynth ...` - Through
 building the package with `poetry build` and using it in an existing project
-(`import nhssynth`). However, if you intend on doing the latter it may be
-preferable to instead follow the second, simpler setup below. For more standard
-usage of the package: 1. Run `pip install nhssynth` within a supported Python
-installation 2. Use the modules exported by the package as you would any other.
-_Note that in this setup you will have to work more closely with the
-configuration and code to ensure you are handling inputs and outputs for each
-module appropriately. The cli handles a lot of this complexity, and interacting
-with the modules directly is considered advanced usage._ ### Usage This package
-comprises a pipeline that is runnable via `poetry run cli pipeline ` or `poetry
-run cli config `. You can run the modules that make up this pipeline
-independently via `poetry run cli `. To see the modules that are available and
-their corresponding arguments and function, run `poetry run cli --help` /
-`poetry run cli  --help`. The figure below shows the structure and workflow of
-the package and its modules. ![](docs/modules.png) ### Roadmap See the [open
-issues](https://github.com/nhsx/NHSSynth/issues) for a list of proposed
-features (and known issues). ### Contributing Contributions are what make the
-open source community such an amazing place to learn, inspire, and create. Any
-contributions you make are **greatly appreciated**. 1. Fork the project 2.
-Create your branch (`git checkout -b /`) 3. Commit your changes (`git commit -
-m 'Add some amazing feature'`) 4. Push to the branch (`git push origin /`) 5.
+(`import nhssynth`). You can then actively develop the package and test it. ###
+Usage This package comprises a set of modules that can be run individually, as
+part of a pipeline, or via a configuration file. These options are available
+via the `nhssynth` command: ``` nhssynth  -- nhssynth pipeline -- nhssynth
+config -c  -- ``` To see the modules that are available and their corresponding
+arguments, run `nhssynth --help` and `nhssynth  --help` respectively.
+Configuration files can be used to run the pipeline or a chosen set of modules.
+They should be placed in the [`config`](config/) folder and their layout should
+match that of the examples provided. They can be run as in the latter case
+above by providing their filename (without the `.yaml` extension). You can also
+override any of the arguments provided in the configuration file by passing
+them as arguments in the command line. To ensure reproducibility, you should
+always specify a `--seed` value and provide the `--save-config` flag to dump
+the exact configuration specified / inferred for the run. This configuration
+file can then be used in the future to reproduce the exact same run or shared
+with others to run the same configuration on their dataset, etc. The figure
+below shows the structure and workflow of the package and its modules. ![]
+(docs/modules.png) ### Roadmap See the [open issues](https://github.com/nhsx/
+NHSSynth/issues) for a list of proposed features (and known issues). ###
+Contributing Any contributions you wish to make are **greatly appreciated**, we
+encourage you to first raise an issue to discuss with the maintainers. If you
+are interested in contributing, please follow these steps: 1. Fork the project
+2. Create your branch (`git checkout -b /`) 3. Commit your changes (`git commit
+-m 'Add some amazing feature'`) 4. Push to the branch (`git push origin /`) 5.
 Open a PR and we will try to get it merged! _See [CONTRIBUTING.md](./
 CONTRIBUTING.md) for detailed guidance._ Thanks to everyone that has
 contributed so far!
                [https://contrib.rocks/image?repo=nhsx/nhssynth]
-### License Distributed under the MIT License. _See [LICENSE](./LICENSE) for
-more information._ ### Contact This project is under active development by
-[@HarrisonWilde](https://github.com/HarrisonWilde), for any questions or
-security concerns [contact him](mailto:h.wilde@warwick.ac.uk) or [raise an
-issue](https://github.com/nhsx/NHSSynth/issues/new/choose). Alternatively,
-contact [NHS England TDAU](mailto:england.tdau@nhs.net). To find out more about
-the [Analytics Unit](https://www.nhsx.nhs.uk/key-tools-and-info/nhsx-analytics-
-unit/) visit our [project website](https://nhsx.github.io/AnalyticsUnit/
-projects.html) or get in touch at [england.tdau@nhs.net](mailto:
+This codebase builds on previous NHSX Analytics Unit PhD internships
+contextualising and investigating the potential use of Variational Auto
+Encoders (VAEs) for synthetic data generation. These were undertaken by Dominic
+Danks and David Brind. ### License Distributed under the MIT License. _See
+[LICENSE](./LICENSE) for more information._ ### Contact This project is under
+active development by [@HarrisonWilde](https://github.com/HarrisonWilde), for
+any questions or security concerns [contact him](mailto:h.wilde@warwick.ac.uk)
+or [raise an issue](https://github.com/nhsx/NHSSynth/issues/new/choose).
+Alternatively, contact [NHS England TDAU](mailto:england.tdau@nhs.net). To find
+out more about the [Analytics Unit](https://www.nhsx.nhs.uk/key-tools-and-info/
+nhsx-analytics-unit/) visit our [project website](https://nhsx.github.io/
+AnalyticsUnit/projects.html) or get in touch at [england.tdau@nhs.net](mailto:
 england.tdau@nhs.net).
```

### Comparing `nhssynth-0.2.2/pyproject.toml` & `nhssynth-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhssynth"
-version = "0.2.2"
+version = "0.3.0"
 description = "Synthetic data generation pipeline leveraging a Differentially Private Variational Auto Encoder assessed using a variety of metrics"
 authors = ["HarrisonWilde <harrisondwilde@outlook.com>"]
 maintainers = ["NHSE TDAU <england.tdau@nhs.net>"]
 license = "MIT"
 readme = ["README.md"]
 repository = "https://github.com/nhsx/NHSSynth"
 keywords = ["synthetic data", "privacy", "fairness", "machine learning"]
@@ -14,24 +14,24 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/nhsx/NHSSynth/issues"
 "Docs" = "https://nhsx.github.io/NHSSynth"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
-torch = "^1.13.1"
+setuptools = "^67.6.1"
 tqdm = "^4.65.0"
-scikit-learn = "^1.2.1"
-rdt = "^1.3.0"
-opacus = "~0.14.0"
-sdv = "^1.0.0"
-pandas = "^1.5.3"
 gower = "^0.1.2"
 pyyaml = "^6.0"
-setuptools = "^67.6.1"
+sdmetrics = "^0.9.3"
+pandas = "^1.5.3"
+rdt = "^1.4.0"
+sdv = "^1.0.0"
+torch = "1.13.1"
+opacus = "^1.4.0"
 
 [tool.poetry.scripts]
 nhssynth = 'nhssynth.cli:run'
 
 [tool.poetry.group.docs]
 optional = true
 
@@ -40,14 +40,16 @@
 mkdocs-material = "^9.1.4"
 mkdocs-gen-files = "^0.4.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 pymdown-extensions = "^9.10"
 
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 notebook = "^6.5.4"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `nhssynth-0.2.2/src/nhssynth/cli/common_arguments.py` & `nhssynth-0.3.0/src/nhssynth/cli/common_arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,69 @@
+"""
+Functions to define the CLI's "common" arguments, i.e. those that can be applied to either:
+ - All module argument lists, e.g. --dataset, --seed, etc.
+ - A subset of module argument lists, e.g. --synthetic, --typed, etc.
+"""
 import argparse
 from typing import Final
 
 from nhssynth.common.constants import *
 
 
 def get_dataset_parser(overrides=False) -> argparse.ArgumentParser:
+    """Create a common parser for specifying the dataset"""
     dataset = argparse.ArgumentParser(add_help=False)
     dataset_grp = dataset.add_argument_group(title="options")
     dataset_grp.add_argument(
         "-d",
         "--dataset",
         required=(not overrides),
         type=str,
         help="the name of the dataset to experiment with, should be present in `<DATA_DIR>`",
     )
     return dataset
 
 
 def get_core_parser(overrides=False) -> argparse.ArgumentParser:
+    """Create a common parser for specifying the core args (except for dataset which is separate)"""
     core = argparse.ArgumentParser(add_help=False)
     core_grp = core.add_argument_group(title="options")
     core_grp.add_argument(
         "-e",
         "--experiment-name",
         type=str,
         default=TIME,
         help=f"name the experiment run to affect logging, config, and default-behaviour io",
     )
     core_grp.add_argument(
         "-s",
         "--seed",
         type=int,
-        help="specify a seed for reproducibility",
+        help="specify a seed for reproducibility, this is a recommended option for reproducibility",
     )
     core_grp.add_argument(
         "--save-config",
         action="store_true",
-        help="save the config provided via the cli",
+        help="save the config provided via the cli, this is a recommended option for reproducibility",
     )
     return core
 
 
-COMMON_TITLE: Final = "starting any of the following args with `_` defaults to a suffix on DATASET (e.g. `_metadata` -> `DATASET_metadata`);\nall filenames are relative to `experiments/<EXPERIMENT_NAME>/` unless otherwise stated"
+COMMON_TITLE: Final = "starting any of the following args with `_` defaults to a suffix on DATASET (e.g. `_metadata` -> `<DATASET>_metadata`);\nall filenames are relative to `experiments/<EXPERIMENT_NAME>/` unless otherwise stated"
 
 
 def suffix_parser_generator(name: str, help: str, required: bool = False) -> argparse.ArgumentParser:
+    """Generator function for creating common parsers for specifying a potential suffix filename
+
+    Args:
+        name: the name of the argument
+        help: the help message for the argument
+        required: whether the argument is required
+    """
+
     def get_parser(overrides: bool = False) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(add_help=False)
         parser_grp = parser.add_argument_group(title=COMMON_TITLE)
         parser_grp.add_argument(
             f"--{name}",
             required=required and not overrides,
             type=str,
```

### Comparing `nhssynth-0.2.2/src/nhssynth/cli/config.py` & `nhssynth-0.3.0/src/nhssynth/cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Read, write and process config files, including handling of module-specific config overrides."""
 import argparse
 import warnings
 from typing import Any, Callable
 
 import yaml
 from nhssynth.cli.module_setup import MODULE_MAP, PIPELINE, run_pipeline
 from nhssynth.common.dicts import *
@@ -109,18 +110,20 @@
         new_args, "dataset"
     ), "No dataset specified in the passed config file, provide one with the `--dataset` argument or add it to the config file"
     assert all(
         getattr(new_args, req_arg["arg"]) for req_arg in required_args
     ), f"Required arguments are missing from the passed config file: {[ra['module'] + ':' + ra['arg'] for ra in required_args if not getattr(new_args, ra['arg'])]}"
 
     # Run the appropriate execution function(s)
+    if not new_args.seed:
+        warnings.warn("No seed has been specified, meaning the results of this run may not be reproducible.")
     new_args.modules_to_run = modules_to_run
     new_args.module_handover = {}
     for module in new_args.modules_to_run:
-        MODULE_MAP[module].func(new_args)
+        MODULE_MAP[module](new_args)
 
     return new_args
 
 
 def get_modules_to_run(executor: Callable) -> list[str]:
     """
     Get the list of modules to run from the passed executor function.
@@ -157,18 +160,16 @@
     args_dict = vars(args)
 
     # Filter out the keys that are not relevant to the config file
     args_dict = filter_dict(
         args_dict, {"func", "experiment_name", "save_config", "save_config_path", "module_handover"}
     )
     for k in args_dict.copy().keys():
-        if k == "sdv_workflow" and not args_dict[k]:
-            args_dict.pop("synthesizer")
         # Remove empty metric lists from the config
-        elif "_metrics" in k and not args_dict[k]:
+        if "_metrics" in k and not args_dict[k]:
             args_dict.pop(k)
 
     modules_to_run = args_dict.pop("modules_to_run")
     if len(modules_to_run) == 1:
         run_type = modules_to_run[0]
     elif modules_to_run == PIPELINE:
         run_type = "pipeline"
```

### Comparing `nhssynth-0.2.2/src/nhssynth/cli/module_arguments.py` & `nhssynth-0.3.0/src/nhssynth/cli/module_arguments.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+"""Define arguments for each of the modules' CLI sub-parsers."""
 import argparse
 
+from nhssynth.cli.model_arguments import add_model_specific_args
 from nhssynth.common.constants import *
+from nhssynth.modules.model import MODELS
 
 
-class customAction(argparse.Action):
+class AllChoicesDefault(argparse.Action):
     """
-    Customized argparse action for defaulting to the full list of choices
+    Customized argparse action for defaulting to the full list of choices if only the flag is supplied.
 
+    Notes:
         1) If no `option_string` is supplied: set to default value (`self.default`)
         2) If `option_string` is supplied:
-            A) If `values` are supplied:
-                set to list of values
-            B) If no `values` are supplied:
-                set to `self.const`, if `self.const` is not set, set to `self.default`
+            a) If `values` are supplied, set to list of values
+            b) If no `values` are supplied, set to `self.const`, if `self.const` is not set, set to `self.default`
     """
 
     def __call__(self, parser, namespace, values=None, option_string=None):
         if values:
             setattr(namespace, self.dest, values)
         elif option_string:
             setattr(namespace, self.dest, self.const if self.const else self.default)
@@ -36,151 +38,132 @@
     group.add_argument(
         "--index-col",
         default=None,
         choices=[None, 0],
         help="indicate whether the csv file's 0th column is an index column, such that pandas can ignore it",
     )
     group.add_argument(
-        "--sdv-workflow",
-        action="store_true",
-        help="utilise the SDV synthesizer workflow for transformation and metadata, rather than a `HyperTransformer` from RDT",
-    )
-    group.add_argument(
         "--allow-null-transformers",
         action="store_true",
         help="allow null / None transformers, i.e. leave some columns as they are",
     )
     group.add_argument(
         "--collapse-yaml",
         action="store_true",
         help="use aliases and anchors in the output metadata yaml, this will make it much more compact",
     )
-    # TODO might be good to have something like this, needs some thought in how to only apply to appropriate transformers, without overriding metadata
-    # group.add_argument(
-    #     "--imputation-strategy",
-    #     default=None,
-    #     help="imputation strategy for missing values, pick one of None, `mean`, `mode`, or a number",
-    # )
     group.add_argument(
         "--synthesizer",
         type=str,
         default="TVAE",
-        choices=list(SDV_SYNTHESIZER_CHOICES.keys()),
+        choices=list(SDV_SYNTHESIZERS.keys()),
         help="pick a synthesizer to use (note this can also be specified in the model module, these must match)",
     )
 
 
 def add_structure_args(parser: argparse.ArgumentParser, group_title: str, overrides: bool = False) -> None:
     pass
 
 
 def add_model_args(parser: argparse.ArgumentParser, group_title: str, overrides: bool = False) -> None:
     """Adds arguments to an existing model module sub-parser instance."""
     group = parser.add_argument_group(title=group_title)
     group.add_argument(
-        "--model-file",
-        type=str,
-        default="_model",
-        help="specify the filename of the model to be saved in `experiments/<EXPERIMENT_NAME>/`, defaults to `<args.real_data>_model.pt`",
-    )
-    group.add_argument(
-        "--use-gpu",
-        action="store_true",
-        help="use the GPU for training",
-    )
-    group.add_argument(
-        "--non-private-training",
-        action="store_true",
-        help="train the model in a non-private way",
-    )
-    group.add_argument(
-        "--secure-rng",
-        action="store_true",
-        default=False,
-        help="Enable Secure RNG to have trustworthy privacy guarantees. Comes at a performance cost",
-    )
-    group.add_argument(
-        "--num-epochs",
-        type=int,
-        default=100,
-        help="number of epochs to train for",
-    )
-    group.add_argument(
-        "--tracked-metrics",
+        "--architecture",
         type=str,
         nargs="+",
-        default=TRACKED_METRIC_CHOICES,
-        help="metrics to track during training of the DPVAE model",
-        choices=TRACKED_METRIC_CHOICES,
+        default=["VAE"],
+        choices=list(MODELS.keys()),
+        help="the model architecture(s) to train",
     )
     group.add_argument(
-        "--latent-dim",
+        "--repeats",
         type=int,
-        default=256,
-        help="the latent dimension of the model",
+        default=1,
+        help="how many times to repeat the training process per model architecture (<SEED> is incremented each time)",
     )
     group.add_argument(
-        "--hidden-dim",
-        type=int,
-        default=256,
-        help="the hidden dimension of the model",
-    )
-    group.add_argument(
-        "--learning-rate",
-        type=float,
-        default=1e-3,
-        help="the learning rate for the model",
+        "--model-file",
+        type=str,
+        default="_model",
+        help="specify the filename of the model to be saved in `experiments/<EXPERIMENT_NAME>/`, defaults to `<DATASET>_model.pt`",
     )
     group.add_argument(
         "--batch-size",
         type=int,
         default=32,
         help="the batch size for the model",
     )
     group.add_argument(
+        "--num-epochs",
+        type=int,
+        default=100,
+        help="number of epochs to train for",
+    )
+    group.add_argument(
         "--patience",
         type=int,
         default=5,
         help="how many epochs the model is allowed to train for without improvement",
     )
     group.add_argument(
-        "--delta",
-        type=int,
-        default=10,
-        help="the difference in successive ELBO values that register as an 'improvement'",
+        "--tracked-metrics",
+        type=str,
+        nargs="+",
+        default=TRACKED_METRICS,
+        help="metrics to track during training of the model",
+        choices=TRACKED_METRICS,
     )
     group.add_argument(
+        "--use-gpu",
+        action="store_true",
+        help="use the GPU for training",
+    )
+    privacy_group = parser.add_argument_group(title="model privacy options")
+    privacy_group.add_argument(
+        "--non-private",
+        action="store_true",
+        help="train the model in a non-private way",
+    )
+    privacy_group.add_argument(
         "--target-epsilon",
         type=float,
         default=1.0,
         help="the target epsilon for differential privacy",
     )
-    group.add_argument(
+    privacy_group.add_argument(
         "--target-delta",
         type=float,
-        default=1e-5,
-        help="the target delta for differential privacy",
+        help="the target delta for differential privacy, defaults to `1 / len(dataset)` if not specified",
     )
-    group.add_argument(
+    privacy_group.add_argument(
         "--max-grad-norm",
-        type=int,
-        default=10,
+        type=float,
+        default=5.0,
         help="the clipping threshold for gradients (only relevant under differential privacy)",
     )
+    privacy_group.add_argument(
+        "--secure-mode",
+        action="store_true",
+        help="Enable secure RNG via the `csprng` package to make privacy guarantees more robust, comes at a cost of performance and reproducibility",
+    )
+    for model_name in MODELS.keys():
+        model_group = parser.add_argument_group(title=f"{model_name}-specific options")
+        add_model_specific_args(model_group, model_name, overrides=overrides)
 
 
 def generate_evaluation_arg(group, name):
     group.add_argument(
         f"--{'-'.join(name.split()).lower()}-metrics",
         type=str,
         default=None,
         nargs="*",
-        action=customAction,
-        const=list(SDV_METRIC_CHOICES[name].keys()),
-        choices=list(SDV_METRIC_CHOICES[name].keys()),
+        action=AllChoicesDefault,
+        const=list(SDV_METRICS[name].keys()),
+        choices=list(SDV_METRICS[name].keys()),
         help=f"run the {name.lower()} evaluation",
     )
 
 
 def add_evaluation_args(parser: argparse.ArgumentParser, group_title: str, overrides: bool = False) -> None:
     """Adds arguments to an existing evaluation module sub-parser instance."""
     group = parser.add_argument_group(title=group_title)
@@ -190,15 +173,15 @@
         help="run the diagnostic evaluation",
     )
     group.add_argument(
         "--quality",
         action="store_true",
         help="run the quality evaluation",
     )
-    for name in SDV_METRIC_CHOICES:
+    for name in SDV_METRICS:
         generate_evaluation_arg(group, name)
 
 
 def add_plotting_args(parser: argparse.ArgumentParser, group_title: str, overrides: bool = False) -> None:
     """Adds arguments to an existing plotting module sub-parser instance."""
     group = parser.add_argument_group(title=group_title)
     group.add_argument(
```

### Comparing `nhssynth-0.2.2/src/nhssynth/cli/module_setup.py` & `nhssynth-0.3.0/src/nhssynth/cli/module_setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,68 @@
+"""Specify all CLI-accessible modules and their configurations, the pipeline to run by default, and define special functions for the `config` and `pipeline` CLI options."""
 import argparse
-from typing import Any, Callable, Final
+from typing import Callable, Final, Optional
 
 from nhssynth.cli.common_arguments import COMMON_PARSERS
 from nhssynth.cli.module_arguments import *
 from nhssynth.modules import dataloader, evaluation, model, plotting, structure
 
 
 class ModuleConfig:
+    """
+    Represents a module's configuration, containing the following attributes:
+
+    Properties:
+        func: A callable that executes the module's functionality.
+        add_args: A callable that populates the module's sub-parser arguments.
+        description: A description of the module's functionality.
+        help: A help message for the module's command-line interface.
+        common_parsers: A list of common parsers to add to the module's sub-parser, appending the 'dataset' and 'core' parsers to those passed.
+    """
+
     def __init__(
         self,
-        func: Callable[..., Any],
-        add_args_func: Callable[..., Any],
+        func: Callable[..., argparse.Namespace],
+        add_args: Callable[..., None],
         description: str,
         help: str,
-        common_parsers: list[str] = None,
+        common_parsers: Optional[list[str]] = None,
     ) -> None:
-        """
-        Represents a module's configuration, containing the following attributes:
-
-        Args:
-            func: A callable that executes the module's functionality.
-            add_args_func: A callable that populates the module's sub-parser arguments.
-            description: A description of the module's functionality.
-            help: A help message for the module's command-line interface.
-            common_parsers: A list of common parsers to add to the module's sub-parser.
-        """
         self.func = func
-        self.add_args_func = add_args_func
+        self.add_args = add_args
         self.description = description
         self.help = help
         if common_parsers:
             assert set(common_parsers) <= COMMON_PARSERS.keys(), "Invalid common parser(s) specified."
             assert (
                 "dataset" not in common_parsers
             ), "The 'dataset' parser is automatically added to all modules, remove it from the ModuleConfig."
             assert (
                 "core" not in common_parsers
             ), "The 'core' parser is automatically added to all modules, remove it from the ModuleConfig."
             self.common_parsers = ["dataset", "core"] + common_parsers
         else:
             self.common_parsers = ["dataset", "core"]
 
+    def __call__(self, *args, **kwargs) -> argparse.Namespace:
+        self.func(*args, **kwargs)
+
 
 def run_pipeline(args: argparse.Namespace) -> None:
     """Runs the specified pipeline of modules with the passed configuration `args`."""
     print("Running full pipeline...")
     args.modules_to_run = PIPELINE
     for module_name in PIPELINE:
-        args = MODULE_MAP[module_name].func(args)
+        args = MODULE_MAP[module_name](args)
 
 
 def add_pipeline_args(parser: argparse.ArgumentParser) -> None:
     """Adds arguments to a `parser` for each module in the pipeline."""
     for module_name in PIPELINE:
-        MODULE_MAP[module_name].add_args_func(parser, f"{module_name} options")
+        MODULE_MAP[module_name].add_args(parser, f"{module_name} options")
 
 
 def add_config_args(parser: argparse.ArgumentParser) -> None:
     """Adds arguments to a `parser` relating to configuration file handling and module-specific config overrides."""
     parser.add_argument(
         "-c",
         "--input-config",
@@ -66,71 +71,73 @@
     )
     parser.add_argument(
         "-cp",
         "--custom-pipeline",
         action="store_true",
         help="infer a custom pipeline running order of modules from the config",
     )
-    for module_name in VALID_MODULES:
-        MODULE_MAP[module_name].add_args_func(parser, f"{module_name} option overrides", overrides=True)
+    for module_name in PIPELINE:
+        MODULE_MAP[module_name].add_args(parser, f"{module_name} option overrides", overrides=True)
+    for module_name in VALID_MODULES - set(PIPELINE):
+        MODULE_MAP[module_name].add_args(parser, f"{module_name} options overrides", overrides=True)
 
 
 ### EDIT BELOW HERE TO ADD MODULES / ALTER PIPELINE BEHAVIOUR
 
 PIPELINE: Final = [
     "dataloader",
     "model",
     "evaluation",
     "plotting",
 ]  # NOTE this determines the order of a pipeline run
 
 MODULE_MAP: Final = {
     "dataloader": ModuleConfig(
         func=dataloader.run,
-        add_args_func=add_dataloader_args,
+        add_args=add_dataloader_args,
         description="Run the Data Loader module, to prepare the chosen dataset for use in other modules.",
         help="prepare the dataset",
         common_parsers=["metadata", "typed", "prepared", "metatransformer"],
     ),
     "structure": ModuleConfig(
         func=structure.run,
-        add_args_func=add_structure_args,
+        add_args=add_structure_args,
         description="Run the Structural Discovery module, to learn a structural model for use in training and evaluation.",
         help="discover structure",
     ),
     "model": ModuleConfig(
         func=model.run,
-        add_args_func=add_model_args,
+        add_args=add_model_args,
         description="Run the Model Architecture module, to train a synthetic data generator.",
         help="train a model",
         common_parsers=["prepared", "metatransformer", "synthetic"],
     ),
     "evaluation": ModuleConfig(
         func=evaluation.run,
-        add_args_func=add_evaluation_args,
+        add_args=add_evaluation_args,
         description="Run the Evaluation module, to evaluate an experiment.",
         help="evaluate an experiment",
         common_parsers=["metadata", "typed", "synthetic", "report"],
     ),
     "plotting": ModuleConfig(
         func=plotting.run,
-        add_args_func=add_plotting_args,
+        add_args=add_plotting_args,
         description="Run the Plotting module, to generate plots for a given model and / or evaluation.",
         help="generate plots",
         common_parsers=["typed", "synthetic", "report"],
     ),
     "pipeline": ModuleConfig(
         func=run_pipeline,
-        add_args_func=add_pipeline_args,
+        add_args=add_pipeline_args,
         description="Run the full pipeline.",
         help="run the full pipeline",
     ),
     "config": ModuleConfig(
         func=None,
-        add_args_func=add_config_args,
+        add_args=add_config_args,
         description="Run module(s) according to configuration specified by a file in `config/`. Note that you can override parts of the configuration on the fly by using the usual CLI flags.",
         help="run module(s) in line with a passed configuration file",
     ),
 }
 
 ### EDIT ABOVE HERE TO ADD MODULES / ALTER PIPELINE BEHAVIOUR
 
@@ -156,26 +163,26 @@
 ) -> argparse.ArgumentParser:
     """
     Add a subparser to an argparse argument parser.
 
     Args:
         subparsers: The subparsers action to which the subparser will be added.
         name: The name of the subparser.
-        module_config: A ModuleConfig object containing information about the subparser, including a function to execute and a function to add arguments.
+        module_config: A [`ModuleConfig`][nhssynth.cli.module_setup.ModuleConfig] object containing information about the subparser, including a function to execute and a function to add arguments.
 
     Returns:
         The newly created subparser.
     """
     parent_parsers = get_parent_parsers(name, module_config.common_parsers)
     parser = subparsers.add_parser(
         name=name,
         description=module_config.description,
         help=module_config.help,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         parents=parent_parsers,
     )
     if name not in {"pipeline", "config"}:
-        module_config.add_args_func(parser, f"{name} options")
+        module_config.add_args(parser, f"{name} options")
     else:
-        module_config.add_args_func(parser)
+        module_config.add_args(parser)
     parser.set_defaults(func=module_config.func)
     return parser
```

### Comparing `nhssynth-0.2.2/src/nhssynth/cli/run.py` & `nhssynth-0.3.0/src/nhssynth/cli/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import argparse
+import warnings
 
 from nhssynth.cli.config import get_modules_to_run, read_config, write_config
 from nhssynth.cli.module_setup import MODULE_MAP, add_subparser
 
 
 def run() -> None:
-    """CLI for preparing, training and evaluating a synthetic data generator."""
-
     parser = argparse.ArgumentParser(
         prog="nhssynth",
         description="CLI for preparing, training and evaluating a synthetic data generator.",
     )
 
     # Below we instantiate one subparser for each module + one for running with a config file and one for
     # doing a full pipeline run with CLI-specified config
     subparsers = parser.add_subparsers()
     all_subparsers = {
         name: add_subparser(subparsers, name, option_config) for name, option_config in MODULE_MAP.items()
     }
 
     args = parser.parse_args()
 
-    # Use get to return None when no function has been set, i.e. user made no running choice
-    executor = vars(args).get("func")
+    executor = vars(args).get("func", None)
     if executor:
+        if not args.seed:
+            warnings.warn("No seed has been specified, meaning the results of this run may not be reproducible.")
         args.modules_to_run = get_modules_to_run(executor)
         args.module_handover = {}
         executor(args)
     elif hasattr(args, "input_config"):
         args = read_config(args, parser, all_subparsers)
     else:
         return parser.print_help()
```

### Comparing `nhssynth-0.2.2/src/nhssynth/common/constants.py` & `nhssynth-0.3.0/src/nhssynth/common/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,36 @@
+"""Define all of the common constants used throughout the project."""
 from time import strftime
 from typing import Final
 
+import torch.nn as nn
 from sdmetrics.single_table import *
 from sdv.single_table import *
 
 TIME: Final = strftime("%Y_%m_%d___%H_%M_%S")
 
-TRACKED_METRIC_CHOICES: Final = ["ELBO", "KLD", "ReconstructionLoss", "CategoricalLoss", "NumericalLoss", "Privacy"]
+TRACKED_METRICS: Final = [
+    "ELBO",
+    "KLD",
+    "ReconstructionLoss",
+    "CategoricalLoss",
+    "NumericalLoss",
+    "Privacy",
+]
+
+ACTIVATION_FUNCTIONS: Final = {
+    "elu": nn.ELU,
+    "relu": nn.ReLU,
+    "selu": nn.SELU,
+    "leaky_relu": nn.LeakyReLU,
+    "tanh": nn.Tanh,
+    "sigmoid": nn.Sigmoid,
+}
 
-SDV_SYNTHESIZER_CHOICES: Final = {
+SDV_SYNTHESIZERS: Final = {
     "TVAE": TVAESynthesizer,
     "CTGAN": CTGANSynthesizer,
     "CopulaGAN": CopulaGANSynthesizer,
     "Copula": GaussianCopulaSynthesizer,
 }
 
 SDV_DETECTION_METRIC_CHOICES: Final = {
@@ -85,15 +103,15 @@
 SDV_NUMERICAL_PRIVACY_METRIC_CHOICES: Final = {
     "NumericalLR": NumericalLR,
     "NumericalMLP": NumericalMLP,
     "NumericalSVR": NumericalSVR,
     "NumericalRadiusNearestNeighbor": NumericalRadiusNearestNeighbor,
 }
 
-SDV_METRIC_CHOICES: Final = {
+SDV_METRICS: Final = {
     "Detection": SDV_DETECTION_METRIC_CHOICES,
     "Binary": SDV_BINARY_METRIC_CHOICES,
     "Multiclass": SDV_MULTICLASS_METRIC_CHOICES,
     "Regression": SDV_REGRESSION_METRIC_CHOICES,
     "Column Shape": SDV_COLUMN_SHAPE_METRIC_CHOICES,
     "Column Similarity": SDV_COLUMN_SIMILARITY_METRIC_CHOICES,
     "Coverage": SDV_COVERAGE_METRIC_CHOICES,
```

### Comparing `nhssynth-0.2.2/src/nhssynth/common/dicts.py` & `nhssynth-0.3.0/src/nhssynth/common/dicts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Common functions for working with dictionaries."""
 from typing import Any
 
 
 def filter_dict(d: dict, filter_keys: set | list, include: bool = False) -> dict:
     """
     Given a dictionary, return a new dictionary either including or excluding keys in a given `filter` set.
```

### Comparing `nhssynth-0.2.2/src/nhssynth/common/io.py` & `nhssynth-0.3.0/src/nhssynth/common/io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Common building-block functions for handling module input and output."""
 import warnings
 from pathlib import Path
 
 
 def experiment_io(experiment_name: str, dir_experiments: str = "experiments") -> str:
     """
     Create an experiment's directory and return the path.
@@ -14,33 +15,31 @@
         The path to the experiment directory.
     """
     dir_experiment = Path(dir_experiments) / experiment_name
     dir_experiment.mkdir(parents=True, exist_ok=True)
     return dir_experiment
 
 
-def consistent_ending(fn: str, ending: str = ".pkl") -> str:
+def consistent_ending(fn: str, ending: str = ".pkl", suffix: str = "") -> str:
     """
     Ensures that the filename `fn` ends with `ending`. If not, removes any existing ending and appends `ending`.
 
     Args:
         fn: The filename to check.
         ending: The desired ending to check for. Default is ".pkl".
+        suffix: A suffix to append to the filename before the ending.
 
     Returns:
-        The filename with the correct ending.
+        The filename with the correct ending and potentially an inserted suffix.
     """
     path_fn = Path(fn)
-    if path_fn.suffix == ending:
-        return fn
-    else:
-        return str(path_fn.parent / path_fn.stem) + ending
+    return str(path_fn.parent / path_fn.stem) + suffix + ending
 
 
-def consistent_endings(args: list[str | tuple[str, str]]) -> list[str]:
+def consistent_endings(args: list[str | tuple[str, str] | tuple[str, str, str]]) -> list[str]:
     return list(consistent_ending(arg) if isinstance(arg, str) else consistent_ending(*arg) for arg in args)
 
 
 def potential_suffix(fn: str, fn_base: str) -> str:
     """
     Checks if `fn` is a suffix (starts with an underscore) to append to `fn_base`, or a filename in its own right.
```

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/dataloader/io.py` & `nhssynth-0.3.0/src/nhssynth/modules/dataloader/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/dataloader/metadata.py` & `nhssynth-0.3.0/src/nhssynth/modules/dataloader/metadata.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/dataloader/metatransformer.py` & `nhssynth-0.3.0/src/nhssynth/modules/dataloader/metatransformer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import warnings
 from typing import Any
 
 import numpy as np
 import pandas as pd
-from nhssynth.common.constants import SDV_SYNTHESIZER_CHOICES
+from nhssynth.common.constants import SDV_SYNTHESIZERS
 from nhssynth.common.dicts import filter_dict
 from nhssynth.modules.dataloader.metadata import get_sdtypes
-from rdt import HyperTransformer
 from rdt.transformers import *
 from sdv.metadata import SingleTableMetadata
 from sdv.single_table.base import BaseSingleTableSynthesizer
 
 
 # TODO should this be an @classmethod?
 def get_transformer(d: dict) -> BaseTransformer | None:
@@ -54,61 +53,55 @@
         ),
     }
 
 
 # TODO Can we come up with a way to instantiate this from the `model` module without needing to pickle and pass? Not high priority but would be nice to have
 class MetaTransformer:
     """
-    A metatransformer object that can wrap either a [`HyperTransformer`](https://docs.sdv.dev/rdt/usage/hypertransformer) from RDT or a
-    [`BaseSingleTableSynthesizer`](https://docs.sdv.dev/sdv/single-table-data/modeling/synthesizers) from SDV. The metatransformer is
-    responsible for transforming input data into a format that can be used by the model module, and transforming the module's output back
-    to the original format of the input data.
+    A metatransformer object that can wrap a [`BaseSingleTableSynthesizer`](https://docs.sdv.dev/sdv/single-table-data/modeling/synthesizers)
+    from SDV. The metatransformer is responsible for transforming input data into a format that can be used by the model module, and transforming
+    the module's output back to the original format of the input data.
 
     Args:
         metadata: A dictionary mapping column names to their metadata.
-        sdv_workflow: A flag indicating whether or not to use the SDV workflow.
         allow_null_transformers: A flag indicating whether or not to allow null transformers on some / all columns.
-        synthesizer: The `BaseSingleTableSynthesizer` class to use within the SDV workflow.
+        synthesizer: The `BaseSingleTableSynthesizer` class to use as the "host" for the MetaTransformer.
 
     Once instantiated via `mt = MetaTransformer(<parameters>)`, the following attributes will be available:
 
     Attributes:
-        sdv_workflow: A flag indicating whether or not to use the SDV workflow.
         allow_null_transformers: A flag indicating whether or not to allow null transformers on some / all columns.
-        Synthesizer: The `BaseSingleTableSynthesizer` class to use within the SDV workflow.
+        Synthesizer: The `BaseSingleTableSynthesizer` host class.
         dtypes: A dictionary mapping each column to its specified pandas dtype (will infer from pandas defaults if this is missing).
         sdtypes: A dictionary mapping each column to the appropriate SDV-specific data type.
         transformers: A dictionary mapping each column to their assigned (if any) transformer.
 
     After preparing some data with the MetaTransformer, i.e. `prepared_data = mt.apply(data)`, the following attributes and methods will be available:
 
     Attributes:
-        metatransformer (HyperTransformer | self.Synthesizer): An instanatiated `HyperTransformer` or `self.Synthesizer` object, ready to use on data.
+        metatransformer (self.Synthesizer): An instanatiated `self.Synthesizer` object, ready to use on data.
         assembled_metadata (dict[str, dict[str, Any]]): A dictionary containing the formatted and complete metadata for the MetaTransformer.
         onehots (list[list[int]]): The groups of indices of one-hotted columns (i.e. each inner list contains all levels of one categorical).
         singles (list[int]): The indices of non-one-hotted columns.
 
     **Methods:**
 
     - `get_assembled_metadata()`: Returns the assembled metadata.
     - `get_sdtypes()`: Returns the sdtypes from the assembled metadata in the correct format for SDMetrics.
     - `get_onehots_and_singles()`: Returns the values of the MetaTransformer's `onehots` and `singles` attributes.
     - `inverse_apply(synthetic_data)`: Apply the inverse of the MetaTransformer to the given data.
 
     Note that `mt.apply` is a helper function that runs `mt.apply_dtypes`, `mt.instaniate`, `mt.assemble`, `mt.prepare` and finally
-    `mt.count_onehots_and_singles` in sequence on a given raw dataset. Along the way it assigns the attributes listed above.
-
-    This workflow is highly encouraged to ensure that the MetaTransformer is properly instantiated for use with the model module.
+    `mt.count_onehots_and_singles` in sequence on a given raw dataset. Along the way it assigns the attributes listed above. *This workflow is highly
+    encouraged to ensure that the MetaTransformer is properly instantiated for use with the model module.*
     """
 
-    def __init__(self, metadata, sdv_workflow, allow_null_transformers, synthesizer) -> None:
-        self.sdv_workflow: bool = sdv_workflow
+    def __init__(self, metadata, allow_null_transformers, synthesizer) -> None:
         self.allow_null_transformers: bool = allow_null_transformers
-        self.Synthesizer: BaseSingleTableSynthesizer = SDV_SYNTHESIZER_CHOICES[synthesizer]
-        # TODO think about whether these belong here
+        self.Synthesizer: BaseSingleTableSynthesizer = SDV_SYNTHESIZERS[synthesizer]
         self.dtypes: dict[str, dict[str, Any]] = {cn: cd.get("dtype", {}) for cn, cd in metadata.items()}
         self.sdtypes: dict[str, dict[str, Any]] = {
             cn: filter_dict(cd, {"dtype", "transformer"}) for cn, cd in metadata.items()
         }
         self.transformers: dict[str, BaseTransformer | None] = {cn: get_transformer(cd) for cn, cd in metadata.items()}
 
     def apply_dtypes(self, data: pd.DataFrame) -> pd.DataFrame:
@@ -143,26 +136,26 @@
         """
         return {
             f"{cn}.component": OneHotEncoder()
             for cn, transformer in transformers.items()
             if transformer.get_name() == "ClusterBasedNormalizer"
         }
 
-    def _instantiate_synthesizer(self, data: pd.DataFrame) -> BaseSingleTableSynthesizer:
+    def instantiate(self, data: pd.DataFrame) -> BaseSingleTableSynthesizer:
         """
         Instantiates a `self.Synthesizer` object from the given metadata and data. Infers missing metadata (sdtypes and transformers).
 
         Args:
             data: The input DataFrame.
 
         Returns:
             A fully instantiated `self.Synthesizer` object and a transformer for the `*.component` columns.
 
         Raises:
-            UserWarning: If the metadata is incomplete and `self.allow_null_transformers` is `False`.
+            UserWarning: If the metadata is incomplete (and `self.allow_null_transformers` is `False`) in the case of missing transformer metadata.
         """
         if all(self.sdtypes.values()):
             metadata = SingleTableMetadata.load_from_dict({"columns": self.sdtypes})
         else:
             warnings.warn(
                 f"Incomplete metadata, detecting missing `sdtype`s for column(s): {[k for k, v in self.sdtypes.items() if not v]} automatically...",
                 UserWarning,
@@ -175,78 +168,30 @@
         if not all(self.transformers.values()) and not self.allow_null_transformers:
             warnings.warn(
                 f"Incomplete metadata, detecting missing `transformers`s for column(s): {[k for k, v in self.transformers.items() if not v]} automatically...",
                 UserWarning,
             )
         synthesizer = self.Synthesizer(metadata)
         synthesizer.auto_assign_transformers(data)
-        synthesizer.update_transformers(
-            self.transformers if self.allow_null_transformers else {k: v for k, v in self.transformers.items() if v}
-        )
-        # TODO this is a hacky way to get the component columns we want to apply OneHotEncoder to
-        component_transformer = self._instantiate_ohe_component_transformers(synthesizer.get_transformers())
-        return synthesizer, component_transformer
-
-    def _instantiate_hypertransformer(self, data: pd.DataFrame) -> HyperTransformer:
-        """
-        Instantiates a `HyperTransformer` object from the metadata and given data. Infers missing metadata (sdtypes and transformers).
-
-        Args:
-            data: The input DataFrame.
-
-        Returns:
-            A fully instantiated `HyperTransformer` object and a transformer for the `*.component` columns.
-
-        Raises:
-            UserWarning: If the metadata is incomplete.
-        """
-        ht = HyperTransformer()
-        if all(self.sdtypes.values()) and (all(self.transformers.values()) or self.allow_null_transformers):
-            ht.set_config(
-                config={
-                    "sdtypes": {k: v["sdtype"] for k, v in self.sdtypes.items()},
-                    "transformers": self.transformers,
-                }
-            )
-        else:
-            warnings.warn(
-                f"Incomplete metadata, detecting missing{(' `sdtype`s for column(s): ' + str([k for k, v in self.sdtypes.items() if not v])) if not all(self.sdtypes.values()) else ''}{(' `transformer`s for column(s): ' + str([k for k, v in self.transformers.items() if not v])) if not all(self.transformers.values()) and not self.allow_null_transformers else ''} automatically...",
-                UserWarning,
-            )
-            ht.detect_initial_config(data)
-            ht.update_sdtypes({k: v["sdtype"] for k, v in self.sdtypes.items() if v})
-            ht.update_transformers(
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            synthesizer.update_transformers(
                 self.transformers if self.allow_null_transformers else {k: v for k, v in self.transformers.items() if v}
             )
         # TODO this is a hacky way to get the component columns we want to apply OneHotEncoder to
-        component_transformer = self._instantiate_ohe_component_transformers(ht.get_config()["transformers"])
-        return ht, component_transformer
-
-    def instantiate(self, data: pd.DataFrame) -> BaseSingleTableSynthesizer | HyperTransformer:
-        """
-        Calls the appropriate instantiation method based on the value of `self.sdv_workflow`.
-
-        Args:
-            data: The input DataFrame.
-
-        Returns:
-            A fully instantiated `self.Synthesizer` or `HyperTransformer` object.
-        """
-        if self.sdv_workflow:
-            return self._instantiate_synthesizer(data)
-        else:
-            return self._instantiate_hypertransformer(data)
+        component_transformer = self._instantiate_ohe_component_transformers(synthesizer.get_transformers())
+        return synthesizer, component_transformer
 
     def _get_dtype(self, cn: str) -> str | np.dtype:
         """Returns the dtype for the given column name `cn`."""
         return self.dtypes[cn].name if not isinstance(self.dtypes[cn], str) else self.dtypes[cn]
 
     def assemble(self) -> dict[str, dict[str, Any]]:
         """
-        Rearranges the dtype, sdtype and transformer metadata into a consistent format regardless of the value of `self,sdv_workflow`
+        Rearranges the dtype, sdtype and transformer metadata into a consistent format ready for output.
 
         Returns:
             A dictionary mapping column names to column metadata.
                 The metadata for each column has the following keys:
                 - dtype: The pandas data type for the column
                 - sdtype: The SDV-specific data type for the column.
                 - transformer: A dictionary containing information about the transformer used for the column (if any). The dictionary has the following keys:
@@ -255,37 +200,23 @@
         Raises:
             ValueError: If the metatransformer has not yet been instantiated.
         """
         if not self.metatransformer:
             raise ValueError(
                 "The metatransformer has not yet been instantiated. Call `mt.apply(data)` first (or `mt.instantiate(data)`)."
             )
-        if self.sdv_workflow:
-            sdmetadata = self.metatransformer.metadata
-            transformers = self.metatransformer.get_transformers()
-            return {
-                cn: {
-                    **cd,
-                    "transformer": make_transformer_dict(transformers[cn]) if transformers[cn] else None,
-                    "dtype": self._get_dtype(cn),
-                }
-                for cn, cd in sdmetadata.columns.items()
-            }
-        else:
-            config = self.metatransformer.get_config()
-            return {
-                cn: {
-                    "sdtype": cd,
-                    "transformer": make_transformer_dict(config["transformers"][cn])
-                    if config["transformers"][cn]
-                    else None,
-                    "dtype": self._get_dtype(cn),
-                }
-                for cn, cd in config["sdtypes"].items()
+        transformers = self.metatransformer.get_transformers()
+        return {
+            cn: {
+                **cd,
+                "transformer": make_transformer_dict(transformers[cn]) if transformers[cn] else None,
+                "dtype": self._get_dtype(cn),
             }
+            for cn, cd in self.metatransformer.metadata.columns.items()
+        }
 
     def prepare(self, data: pd.DataFrame) -> pd.DataFrame:
         """
         Prepares the data by processing it via the metatransformer.
 
         Args:
             data: The data to fit and apply the transformer to.
@@ -296,18 +227,15 @@
         Raises:
             ValueError: If the metatransformer has not yet been instantiated.
         """
         if not self.metatransformer:
             raise ValueError(
                 "The metatransformer has not yet been instantiated. Call `mt.apply(data)` first (or `mt.instantiate(data)`)."
             )
-        if self.sdv_workflow:
-            prepared_data = self.metatransformer.preprocess(data)
-        else:
-            prepared_data = self.metatransformer.fit_transform(data)
+        prepared_data = self.metatransformer.preprocess(data)
         # TODO this is kind of a hacky way to solve the component column problem
         for cn, transformer in self.component_transformer.items():
             prepared_data = transformer.fit_transform(prepared_data, cn)
         return prepared_data
 
     def count_onehots_and_singles(self, data: pd.DataFrame) -> tuple[list[list[int]], list[int]]:
         """
@@ -330,14 +258,16 @@
             if cd["transformer"].get("name") == "OneHotEncoder":
                 onehot_idxs.append(data.columns.get_indexer(data.filter(like=cn + ".value").columns).tolist())
             elif cd["transformer"].get("name") == "ClusterBasedNormalizer":
                 onehot_idxs.append(data.columns.get_indexer(data.filter(like=cn + ".component.value").columns).tolist())
                 single_idxs.append(data.columns.get_loc(cn + ".normalized"))
             elif cd["transformer"].get("name") != "RegexGenerator":
                 single_idxs.append(data.columns.get_loc(cn))
+        if not onehot_idxs:
+            onehot_idxs.append([])
         return onehot_idxs, single_idxs
 
     def apply(self, data: pd.DataFrame) -> pd.DataFrame:
         """
         Applies the various steps of the MetaTransformer to a passed DataFrame.
 
         Args:
@@ -420,11 +350,8 @@
         """
         if not hasattr(self, "metatransformer"):
             raise ValueError(
                 "The metatransformer has not yet been instantiated. Call `mt.apply(data)` first (or `mt.instantiate(data)`)."
             )
         for transformer in self.component_transformer.values():
             data = transformer.reverse_transform(data)
-        if self.sdv_workflow:
-            return self.metatransformer._data_processor.reverse_transform(data)
-        else:
-            return self.metatransformer.reverse_transform(data)
+        return self.metatransformer._data_processor.reverse_transform(data)
```

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/dataloader/run.py` & `nhssynth-0.3.0/src/nhssynth/modules/dataloader/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,25 @@
 from nhssynth.common import *
 from nhssynth.modules.dataloader.io import *
 from nhssynth.modules.dataloader.metadata import load_metadata
 from nhssynth.modules.dataloader.metatransformer import MetaTransformer
 
 
 def run(args: argparse.Namespace) -> argparse.Namespace:
-    """
-    Runs the main workflow of the dataloader module, transforms the dataset and writes the output and transformer used to disk.
-
-    Args:
-        args: An argparse Namespace containing the command line arguments.
-    """
     print("Running dataloader module...")
 
     set_seed(args.seed)
     dir_experiment = experiment_io(args.experiment_name)
 
     dir_input, fn_dataset, fn_metadata = check_input_paths(args.dataset, args.metadata, args.data_dir)
 
     dataset = pd.read_csv(dir_input / fn_dataset, index_col=args.index_col)
     metadata = load_metadata(dir_input / fn_metadata, dataset)
 
-    mt = MetaTransformer(metadata, args.sdv_workflow, args.allow_null_transformers, args.synthesizer)
+    mt = MetaTransformer(metadata, args.allow_null_transformers, args.synthesizer)
     typed_dataset, prepared_dataset = mt.apply(dataset)
 
     write_data_outputs(typed_dataset, prepared_dataset, mt, fn_dataset, fn_metadata, dir_experiment, args)
 
     if "model" in args.modules_to_run:
         args.module_handover.update(
             {
```

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/evaluation/full_report.py` & `nhssynth-0.3.0/src/nhssynth/modules/evaluation/full_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         print("")
         validate_single_table_inputs(real_data, synthetic_data, metadata)
         self._property_breakdown = {}
         for prop, metrics in tqdm(
             self._metrics.items(), desc="Creating report", position=0, disable=(not verbose), leave=True
         ):
             num_prop_errors = 0
-            if "NewRowSynthesis" in SDV_METRIC_CHOICES[prop]:
+            if "NewRowSynthesis" in SDV_METRICS[prop]:
                 if "NewRowSynthesis" not in self._metric_args:
                     self._metric_args["NewRowSynthesis"] = {}
                 self._metric_args["NewRowSynthesis"]["synthetic_sample_size"] = min(
                     min(len(real_data), len(synthetic_data)),
                     self._metric_args["NewRowSynthesis"].get("synthetic_sample_size", len(real_data)),
                 )
             for metric in tqdm(metrics, desc=prop + " metrics", position=1, disable=(not verbose), leave=False):
```

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/evaluation/io.py` & `nhssynth-0.3.0/src/nhssynth/modules/evaluation/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/evaluation/metrics.py` & `nhssynth-0.3.0/src/nhssynth/modules/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/evaluation/run.py` & `nhssynth-0.3.0/src/nhssynth/modules/evaluation/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 
 from nhssynth.common import *
-from nhssynth.common.constants import SDV_METRIC_CHOICES
+from nhssynth.common.constants import SDV_METRICS
 from nhssynth.modules.evaluation.full_report import FullReport
 from nhssynth.modules.evaluation.io import load_required_data
 from sdmetrics.reports.single_table import DiagnosticReport, QualityReport
 
 
 def run(args: argparse.Namespace) -> argparse.Namespace:
     print("Running evaluation module...")
@@ -29,16 +29,16 @@
             report.get_visualization(property_name)
             for property_name in report.get_properties()["Property"].unique().tolist()
         ]
         for fig in figs:
             fig.show()
 
     sdv_metrics = {
-        k: [SDV_METRIC_CHOICES[k][v] for v in getattr(args, "_".join(k.split()).lower() + "_metrics")]
-        for k in SDV_METRIC_CHOICES.keys()
+        k: [SDV_METRICS[k][v] for v in getattr(args, "_".join(k.split()).lower() + "_metrics")]
+        for k in SDV_METRICS.keys()
         if getattr(args, "_".join(k.split()).lower() + "_metrics")
     }
     if sdv_metrics:
         report = FullReport(sdv_metrics)
         report.generate(real_data, synthetic_data, metadata)
         report.save(dir_experiment / (fn_dataset[:-4] + args.report + ".pkl"))
```

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/model/io.py` & `nhssynth-0.3.0/src/nhssynth/modules/model/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import pickle
 from pathlib import Path
+from typing import Optional
 
 import pandas as pd
 from nhssynth.common.io import *
 from nhssynth.modules.dataloader.metatransformer import MetaTransformer
 
 
 def check_input_paths(
@@ -25,28 +26,42 @@
     fn_dataset, fn_prepared, fn_metatransformer = consistent_endings([fn_dataset, fn_prepared, fn_metatransformer])
     fn_prepared, fn_metatransformer = potential_suffixes([fn_prepared, fn_metatransformer], fn_dataset)
     warn_if_path_supplied([fn_dataset, fn_prepared, fn_metatransformer], dir_experiment)
     check_exists([fn_prepared, fn_metatransformer], dir_experiment)
     return fn_dataset, fn_prepared, fn_metatransformer
 
 
-def check_output_paths(fn_dataset: Path, fn_synthetic: str, fn_model: str, dir_experiment: Path) -> tuple[str, str]:
+def check_output_paths(
+    fn_dataset: Path,
+    fn_synthetic: str,
+    fn_model: str,
+    dir_experiment: Path,
+    model: str,
+    seed: Optional[int] = None,
+) -> tuple[str, str]:
     """
     Sets up the input and output paths for the model files.
 
     Args:
         fn_dataset: The base name of the dataset.
         fn_synthetic: The name of the synthetic data file.
         fn_model: The name of the model file.
         dir_experiment: The path to the experiment output directory.
+        model: The name of the model used.
+        seed: The seed used to generate the synthetic data.
 
     Returns:
         The path to output the model.
     """
-    fn_synthetic, fn_model = consistent_endings([fn_synthetic, (fn_model, ".pt")])
+    fn_synthetic, fn_model = consistent_endings(
+        [
+            (fn_synthetic, ".pkl", f"_{model}" + (f"_{str(seed)}" if seed else "")),
+            (fn_model, ".pt", f"_{model}" + (f"_{str(seed)}" if seed else "")),
+        ]
+    )
     fn_synthetic, fn_model = potential_suffixes([fn_synthetic, fn_model], fn_dataset)
     warn_if_path_supplied([fn_synthetic, fn_model], dir_experiment)
     return fn_synthetic, fn_model
 
 
 def load_required_data(
     args: argparse.Namespace, dir_experiment: Path
```

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/plotting/io.py` & `nhssynth-0.3.0/src/nhssynth/modules/plotting/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/plotting/plots.py` & `nhssynth-0.3.0/src/nhssynth/modules/plotting/plots.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.2/src/nhssynth/modules/plotting/run.py` & `nhssynth-0.3.0/src/nhssynth/modules/plotting/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.2/PKG-INFO` & `nhssynth-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhssynth
-Version: 0.2.2
+Version: 0.3.0
 Summary: Synthetic data generation pipeline leveraging a Differentially Private Variational Auto Encoder assessed using a variety of metrics
 Home-page: https://github.com/nhsx/NHSSynth
 License: MIT
 Keywords: synthetic data,privacy,fairness,machine learning
 Author: HarrisonWilde
 Author-email: harrisondwilde@outlook.com
 Maintainer: NHSE TDAU
@@ -12,22 +12,22 @@
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: gower (>=0.1.2,<0.2.0)
-Requires-Dist: opacus (>=0.14.0,<0.15.0)
+Requires-Dist: opacus (>=1.4.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: rdt (>=1.3.0,<2.0.0)
-Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
+Requires-Dist: rdt (>=1.4.0,<2.0.0)
+Requires-Dist: sdmetrics (>=0.9.3,<0.10.0)
 Requires-Dist: sdv (>=1.0.0,<2.0.0)
 Requires-Dist: setuptools (>=67.6.1,<68.0.0)
-Requires-Dist: torch (>=1.13.1,<2.0.0)
+Requires-Dist: torch (==1.13.1)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/nhsx/NHSSynth/issues
 Project-URL: Docs, https://nhsx.github.io/NHSSynth
 Project-URL: Repository, https://github.com/nhsx/NHSSynth
 Description-Content-Type: text/markdown
 
 <!-- PROJECT SHIELDS -->
@@ -47,77 +47,96 @@
 <!-- PROJECT LOGO -->
 <div align="center">
   <a href="https://nhsx.github.io/NHSSynth">
     <img src="docs/assets/NHS.svg" alt="Logo" width="200" height="100">
   </a>
   <p align="center">
     <a href="https://nhsx.github.io/NHSSynth"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
+    <br /><br /><br />
   </p>
 </div>
 
 # NHS Synth
 
-## About the Project
+## About
 
-The project currently consists of a Python package alongside research and investigative materials covering the effectiveness of the package and synthetic data more generally when applied to NHS use cases.
-
-[Project Description - Synthetic Data Exploration: Variational Autoencoders](https://nhsx.github.io/nhsx-internship-projects/synthetic-data-exploration-vae/)
-
-The codebase builds on previous NHSX Analytics Unit PhD internships contextualising and investigating the potential use of Variational Auto Encoders (VAEs) for synthetic data generation. These were undertaken by Dominic Danks and David Brind.
+This repository currently consists of a Python package alongside research and investigative materials covering the effectiveness of the package and synthetic data more generally when applied to NHS use cases. See the internal [project description](https://nhsx.github.io/nhsx-internship-projects/synthetic-data-exploration-vae/) for more information.
 
 _**Note:** No data, public or private are shared in this repository._
 
 ## Getting Started
 
 ### Project Structure
 
-- The main package and codebase is found in `src/nhssynth` (see Usage below for more information)
-- Accompanying materials are available in the `docs` folder:
-  - A [report](reports/report.pdf) summarising the previous iteration of this project
-  - A [model card](model_card.md) providing more information about the VAE with Differential Privacy
-- Numerous [exemplar configurations](../config) are found in `config`
-- Empty `data` and `experiments` folders are provided; these are the default locations for inputs and outputs when running the project using the provided [`cli`](../src/nhssynth/cli/) module
+- The main package and codebase is found in [`src/nhssynth`](src/nhssynth/) (see [Usage](#usage) below for more information)
+- Accompanying materials are available in the [`docs`](docs/) folder:
+  - The components used to create the GitHub Pages [documentation site](https://nhsx.github.io/NHSSynth/)
+  - A [report](docs/reports/report.pdf) summarising the previous iteration of this project
+  - A [model card](docs/model_card.md) providing more information about the VAE with Differential Privacy
+- Numerous exemplar configurations are found in [`config`](config/)
+- Empty [`data`](data/) and [`experiments`](experiments/) folders are provided; these are the default locations for inputs and outputs when running the project using the provided [CLI](../src/nhssynth/cli/) module
 - Pre-processing notebooks for specific datasets used to assess the approach and other non-core code can be found in [`auxiliary`](../auxiliary/)
 
 ### Installation
 
-As it stands, we recommend the following steps to reproduce our experiments and fully work with this project:
+For general usage, we recommend installing the package via `pip install nhssynth` in a supported python version environment. You can then `import` the package's [modules](src/nhssynth/modules/) and use them in your projects, or interact with the package directly via the [CLI](src/nhssynth/cli/), which is accessed using the `nhssynth` command (see [Usage](#usage) for more information).
+
+#### Secure Mode
+
+Note that in order to train a generator in *secure mode* (see the [documentation](https://nhsx.github.io/NHSSynth/secure_mode/) for details) you will need to install the PyTorch extension package [`csprng`](https://github.com/pytorch/csprng) separately. Currently this package's dependencies are not compatible with recent versions of PyTorch (the author's plan on rectifying this - watch this space), so you will need to install it manually; for this we recommend following the instructions below:
+
+```bash
+git clone git@github.com:pytorch/csprng.git
+cd csprng
+git branch release "v0.2.2-rc1"
+git checkout release
+python setup.py install
+```
+
+#### Advanced Usage
+
+If you intend on contributing or working with the codebase directly, or if you want to reproduce the results of this project, follow the steps below:
 
 1. Clone the repo
 2. Ensure one of the required versions of Python is installed
 3. Install [`poetry`](https://python-poetry.org/docs/#installation)
 4. Instantiate a virtual environment, e.g. via `python -m venv nhssynth`
 3. Activate the virtual environment, e.g. via `source nhssynth/bin/activate`
-4. Install project dependencies with `poetry install` (optionally install `jupyter` and `notebook` to work with some of the preprocessing files in [`auxiliary`](auxiliary/))
-5. Interact with the package in one of two ways:
-    - Via the [`cli`](src/nhssynth/cli/) module using `poetry run cli`
-    - Through building the package with `poetry build` and using it in an existing project (`import nhssynth`). However, if you intend on doing the latter it may be preferable to instead follow the second, simpler setup below.
+4. Install the project dependencies with `poetry install` (optionally install the dev dependencies `--with dev` to work with the [auxiliary notebooks](auxiliary/), or `--with docs` to work with the [documentation](docs/))
+5. You can then interact with the package in one of two ways:
+    - Via the [CLI](src/nhssynth/cli/) module using `nhssynth ...`
+    - Through building the package with `poetry build` and using it in an existing project (`import nhssynth`). You can then actively develop the package and test it.
 
-For more standard usage of the package:
+### Usage
 
-1. Run `pip install nhssynth` within a supported Python installation
-2. Use the modules exported by the package as you would any other. _Note that in this setup you will have to work more closely with the configuration and code to ensure you are handling inputs and outputs for each module appropriately. The cli handles a lot of this complexity, and interacting with the modules directly is considered advanced usage._
+This package comprises a set of modules that can be run individually, as part of a pipeline, or via a configuration file. These options are available via the `nhssynth` command:
 
-### Usage
+```
+nhssynth <module name> --<args>
+nhssynth pipeline --<args>
+nhssynth config -c <name> --<overrides>
+```
 
-This package comprises a pipeline that is runnable via `poetry run cli pipeline <args>` or `poetry run cli config <config filepath>`. You can run the modules that make up this pipeline independently via `poetry run cli <module name>`. To see the modules that are available and their corresponding arguments and function, run `poetry run cli --help` / `poetry run cli <module name> --help`.
+To see the modules that are available and their corresponding arguments, run `nhssynth --help` and `nhssynth <module name> --help` respectively.
+
+Configuration files can be used to run the pipeline or a chosen set of modules. They should be placed in the [`config`](config/) folder and their layout should match that of the examples provided. They can be run as in the latter case above by providing their filename (without the `.yaml` extension). You can also override any of the arguments provided in the configuration file by passing them as arguments in the command line.
+
+To ensure reproducibility, you should always specify a `--seed` value and provide the `--save-config` flag to dump the exact configuration specified / inferred for the run. This configuration file can then be used in the future to reproduce the exact same run or shared with others to run the same configuration on their dataset, etc.
 
 The figure below shows the structure and workflow of the package and its modules.
 
 ![](docs/modules.png)
 
 ### Roadmap
 
 See the [open issues](https://github.com/nhsx/NHSSynth/issues) for a list of proposed features (and known issues).
 
 ### Contributing
 
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+Any contributions you wish to make are **greatly appreciated**, we encourage you to first raise an issue to discuss with the maintainers. If you are interested in contributing, please follow these steps:
 
 1. Fork the project
 2. Create your branch (`git checkout -b <yourusername>/<featurename>`)
 3. Commit your changes (`git commit -m 'Add some amazing feature'`)
 4. Push to the branch (`git push origin <yourusername>/<featurename>`)
 5. Open a PR and we will try to get it merged!
 
@@ -127,14 +146,16 @@
 
 <div align="center">
 <a href="https://github.com/nhsx/nhssynth/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=nhsx/nhssynth" />
 </a>
 </div>
 
+This codebase builds on previous NHSX Analytics Unit PhD internships contextualising and investigating the potential use of Variational Auto Encoders (VAEs) for synthetic data generation. These were undertaken by Dominic Danks and David Brind.
+
 ### License
 
 Distributed under the MIT License. _See [LICENSE](./LICENSE) for more information._
 
 ### Contact
 
 This project is under active development by [@HarrisonWilde](https://github.com/HarrisonWilde), for any questions or security concerns [contact him](mailto:h.wilde@warwick.ac.uk) or [raise an issue](https://github.com/nhsx/NHSSynth/issues/new/choose). Alternatively, contact [NHS England TDAU](mailto:england.tdau@nhs.net).
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: nhssynth Version: 0.2.2 Summary: Synthetic data
+Metadata-Version: 2.1 Name: nhssynth Version: 0.3.0 Summary: Synthetic data
 generation pipeline leveraging a Differentially Private Variational Auto
 Encoder assessed using a variety of metrics Home-page: https://github.com/nhsx/
 NHSSynth License: MIT Keywords: synthetic data,privacy,fairness,machine
 learning Author: HarrisonWilde Author-email: harrisondwilde@outlook.com
 Maintainer: NHSE TDAU Maintainer-email: england.tdau@nhs.net Requires-Python:
 >=3.9,<3.11 Classifier: Development Status :: 3 - Alpha Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Dist: gower (>=0.1.2,<0.2.0) Requires-Dist:
-opacus (>=0.14.0,<0.15.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist:
-pyyaml (>=6.0,<7.0) Requires-Dist: rdt (>=1.3.0,<2.0.0) Requires-Dist: scikit-
-learn (>=1.2.1,<2.0.0) Requires-Dist: sdv (>=1.0.0,<2.0.0) Requires-Dist:
-setuptools (>=67.6.1,<68.0.0) Requires-Dist: torch (>=1.13.1,<2.0.0) Requires-
-Dist: tqdm (>=4.65.0,<5.0.0) Project-URL: Bug Tracker, https://github.com/nhsx/
+opacus (>=1.4.0,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist:
+pyyaml (>=6.0,<7.0) Requires-Dist: rdt (>=1.4.0,<2.0.0) Requires-Dist:
+sdmetrics (>=0.9.3,<0.10.0) Requires-Dist: sdv (>=1.0.0,<2.0.0) Requires-Dist:
+setuptools (>=67.6.1,<68.0.0) Requires-Dist: torch (==1.13.1) Requires-Dist:
+tqdm (>=4.65.0,<5.0.0) Project-URL: Bug Tracker, https://github.com/nhsx/
 NHSSynth/issues Project-URL: Docs, https://nhsx.github.io/NHSSynth Project-URL:
 Repository, https://github.com/nhsx/NHSSynth Description-Content-Type: text/
 markdown
  [![PyPI - Latest Release](https://img.shields.io/pypi/v/nhssynth?style=flat-
     square)](https://pypi.org/project/nhssynth/) [![PyPI - Wheel](https://
    img.shields.io/pypi/wheel/nhssynth?style=flat-square)](https://pypi.org/
    project/nhssynth/) [![PyPI - Package Status](https://img.shields.io/pypi/
@@ -27,71 +27,93 @@
   github.com/nhsx/nhssynth/blob/main/LICENSE) [![Code style: black](https://
   img.shields.io/badge/code%20style-black-000000?style=flat-square)](https://
     github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat-square)](https://pycqa.github.io/isort/)
                                     [Logo]
                              Explore_the_docs_Â»
 
-# NHS Synth ## About the Project The project currently consists of a Python
-package alongside research and investigative materials covering the
-effectiveness of the package and synthetic data more generally when applied to
-NHS use cases. [Project Description - Synthetic Data Exploration: Variational
-Autoencoders](https://nhsx.github.io/nhsx-internship-projects/synthetic-data-
-exploration-vae/) The codebase builds on previous NHSX Analytics Unit PhD
-internships contextualising and investigating the potential use of Variational
-Auto Encoders (VAEs) for synthetic data generation. These were undertaken by
-Dominic Danks and David Brind. _**Note:** No data, public or private are shared
-in this repository._ ## Getting Started ### Project Structure - The main
-package and codebase is found in `src/nhssynth` (see Usage below for more
-information) - Accompanying materials are available in the `docs` folder: - A
-[report](reports/report.pdf) summarising the previous iteration of this project
-- A [model card](model_card.md) providing more information about the VAE with
-Differential Privacy - Numerous [exemplar configurations](../config) are found
-in `config` - Empty `data` and `experiments` folders are provided; these are
-the default locations for inputs and outputs when running the project using the
-provided [`cli`](../src/nhssynth/cli/) module - Pre-processing notebooks for
-specific datasets used to assess the approach and other non-core code can be
-found in [`auxiliary`](../auxiliary/) ### Installation As it stands, we
-recommend the following steps to reproduce our experiments and fully work with
-this project: 1. Clone the repo 2. Ensure one of the required versions of
-Python is installed 3. Install [`poetry`](https://python-poetry.org/docs/
-#installation) 4. Instantiate a virtual environment, e.g. via `python -m venv
-nhssynth` 3. Activate the virtual environment, e.g. via `source nhssynth/bin/
-activate` 4. Install project dependencies with `poetry install` (optionally
-install `jupyter` and `notebook` to work with some of the preprocessing files
-in [`auxiliary`](auxiliary/)) 5. Interact with the package in one of two ways:
-- Via the [`cli`](src/nhssynth/cli/) module using `poetry run cli` - Through
+
+# NHS Synth ## About This repository currently consists of a Python package
+alongside research and investigative materials covering the effectiveness of
+the package and synthetic data more generally when applied to NHS use cases.
+See the internal [project description](https://nhsx.github.io/nhsx-internship-
+projects/synthetic-data-exploration-vae/) for more information. _**Note:** No
+data, public or private are shared in this repository._ ## Getting Started ###
+Project Structure - The main package and codebase is found in [`src/nhssynth`]
+(src/nhssynth/) (see [Usage](#usage) below for more information) - Accompanying
+materials are available in the [`docs`](docs/) folder: - The components used to
+create the GitHub Pages [documentation site](https://nhsx.github.io/NHSSynth/
+) - A [report](docs/reports/report.pdf) summarising the previous iteration of
+this project - A [model card](docs/model_card.md) providing more information
+about the VAE with Differential Privacy - Numerous exemplar configurations are
+found in [`config`](config/) - Empty [`data`](data/) and [`experiments`]
+(experiments/) folders are provided; these are the default locations for inputs
+and outputs when running the project using the provided [CLI](../src/nhssynth/
+cli/) module - Pre-processing notebooks for specific datasets used to assess
+the approach and other non-core code can be found in [`auxiliary`](../
+auxiliary/) ### Installation For general usage, we recommend installing the
+package via `pip install nhssynth` in a supported python version environment.
+You can then `import` the package's [modules](src/nhssynth/modules/) and use
+them in your projects, or interact with the package directly via the [CLI](src/
+nhssynth/cli/), which is accessed using the `nhssynth` command (see [Usage]
+(#usage) for more information). #### Secure Mode Note that in order to train a
+generator in *secure mode* (see the [documentation](https://nhsx.github.io/
+NHSSynth/secure_mode/) for details) you will need to install the PyTorch
+extension package [`csprng`](https://github.com/pytorch/csprng) separately.
+Currently this package's dependencies are not compatible with recent versions
+of PyTorch (the author's plan on rectifying this - watch this space), so you
+will need to install it manually; for this we recommend following the
+instructions below: ```bash git clone git@github.com:pytorch/csprng.git cd
+csprng git branch release "v0.2.2-rc1" git checkout release python setup.py
+install ``` #### Advanced Usage If you intend on contributing or working with
+the codebase directly, or if you want to reproduce the results of this project,
+follow the steps below: 1. Clone the repo 2. Ensure one of the required
+versions of Python is installed 3. Install [`poetry`](https://python-
+poetry.org/docs/#installation) 4. Instantiate a virtual environment, e.g. via
+`python -m venv nhssynth` 3. Activate the virtual environment, e.g. via `source
+nhssynth/bin/activate` 4. Install the project dependencies with `poetry
+install` (optionally install the dev dependencies `--with dev` to work with the
+[auxiliary notebooks](auxiliary/), or `--with docs` to work with the
+[documentation](docs/)) 5. You can then interact with the package in one of two
+ways: - Via the [CLI](src/nhssynth/cli/) module using `nhssynth ...` - Through
 building the package with `poetry build` and using it in an existing project
-(`import nhssynth`). However, if you intend on doing the latter it may be
-preferable to instead follow the second, simpler setup below. For more standard
-usage of the package: 1. Run `pip install nhssynth` within a supported Python
-installation 2. Use the modules exported by the package as you would any other.
-_Note that in this setup you will have to work more closely with the
-configuration and code to ensure you are handling inputs and outputs for each
-module appropriately. The cli handles a lot of this complexity, and interacting
-with the modules directly is considered advanced usage._ ### Usage This package
-comprises a pipeline that is runnable via `poetry run cli pipeline ` or `poetry
-run cli config `. You can run the modules that make up this pipeline
-independently via `poetry run cli `. To see the modules that are available and
-their corresponding arguments and function, run `poetry run cli --help` /
-`poetry run cli  --help`. The figure below shows the structure and workflow of
-the package and its modules. ![](docs/modules.png) ### Roadmap See the [open
-issues](https://github.com/nhsx/NHSSynth/issues) for a list of proposed
-features (and known issues). ### Contributing Contributions are what make the
-open source community such an amazing place to learn, inspire, and create. Any
-contributions you make are **greatly appreciated**. 1. Fork the project 2.
-Create your branch (`git checkout -b /`) 3. Commit your changes (`git commit -
-m 'Add some amazing feature'`) 4. Push to the branch (`git push origin /`) 5.
+(`import nhssynth`). You can then actively develop the package and test it. ###
+Usage This package comprises a set of modules that can be run individually, as
+part of a pipeline, or via a configuration file. These options are available
+via the `nhssynth` command: ``` nhssynth  -- nhssynth pipeline -- nhssynth
+config -c  -- ``` To see the modules that are available and their corresponding
+arguments, run `nhssynth --help` and `nhssynth  --help` respectively.
+Configuration files can be used to run the pipeline or a chosen set of modules.
+They should be placed in the [`config`](config/) folder and their layout should
+match that of the examples provided. They can be run as in the latter case
+above by providing their filename (without the `.yaml` extension). You can also
+override any of the arguments provided in the configuration file by passing
+them as arguments in the command line. To ensure reproducibility, you should
+always specify a `--seed` value and provide the `--save-config` flag to dump
+the exact configuration specified / inferred for the run. This configuration
+file can then be used in the future to reproduce the exact same run or shared
+with others to run the same configuration on their dataset, etc. The figure
+below shows the structure and workflow of the package and its modules. ![]
+(docs/modules.png) ### Roadmap See the [open issues](https://github.com/nhsx/
+NHSSynth/issues) for a list of proposed features (and known issues). ###
+Contributing Any contributions you wish to make are **greatly appreciated**, we
+encourage you to first raise an issue to discuss with the maintainers. If you
+are interested in contributing, please follow these steps: 1. Fork the project
+2. Create your branch (`git checkout -b /`) 3. Commit your changes (`git commit
+-m 'Add some amazing feature'`) 4. Push to the branch (`git push origin /`) 5.
 Open a PR and we will try to get it merged! _See [CONTRIBUTING.md](./
 CONTRIBUTING.md) for detailed guidance._ Thanks to everyone that has
 contributed so far!
                [https://contrib.rocks/image?repo=nhsx/nhssynth]
-### License Distributed under the MIT License. _See [LICENSE](./LICENSE) for
-more information._ ### Contact This project is under active development by
-[@HarrisonWilde](https://github.com/HarrisonWilde), for any questions or
-security concerns [contact him](mailto:h.wilde@warwick.ac.uk) or [raise an
-issue](https://github.com/nhsx/NHSSynth/issues/new/choose). Alternatively,
-contact [NHS England TDAU](mailto:england.tdau@nhs.net). To find out more about
-the [Analytics Unit](https://www.nhsx.nhs.uk/key-tools-and-info/nhsx-analytics-
-unit/) visit our [project website](https://nhsx.github.io/AnalyticsUnit/
-projects.html) or get in touch at [england.tdau@nhs.net](mailto:
+This codebase builds on previous NHSX Analytics Unit PhD internships
+contextualising and investigating the potential use of Variational Auto
+Encoders (VAEs) for synthetic data generation. These were undertaken by Dominic
+Danks and David Brind. ### License Distributed under the MIT License. _See
+[LICENSE](./LICENSE) for more information._ ### Contact This project is under
+active development by [@HarrisonWilde](https://github.com/HarrisonWilde), for
+any questions or security concerns [contact him](mailto:h.wilde@warwick.ac.uk)
+or [raise an issue](https://github.com/nhsx/NHSSynth/issues/new/choose).
+Alternatively, contact [NHS England TDAU](mailto:england.tdau@nhs.net). To find
+out more about the [Analytics Unit](https://www.nhsx.nhs.uk/key-tools-and-info/
+nhsx-analytics-unit/) visit our [project website](https://nhsx.github.io/
+AnalyticsUnit/projects.html) or get in touch at [england.tdau@nhs.net](mailto:
 england.tdau@nhs.net).
```

