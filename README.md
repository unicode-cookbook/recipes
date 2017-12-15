# Recipes for the Unicode Cookbook

Steven Moran &lt;bambooforest@gmail.com&gt; & Michael Cysouw &lt;cysouw@mac.com&gt;

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview

This directory contains recipes (use cases) that supplement the [Unicode Cookbook for Linguists](https://github.com/unicode-cookbook/cookbook). Each recipe is in its own subdirectory:

- ASJP: tokenize ASJP wordlists with the R programming language
- Basics: basics of text tokenization and grapheme segmentation in the Python programming language
- Dogon: tokenize the Dogon comparative wordlist and create an orthography profile in Python with Pandas
- Dutch: create an orthography profile for tokenizing Dutch orthography with R
- JIPA: tokenize text in IPA with Python or R


## Installing Python `segments` package

To install the [Python `segments` package](https://pypi.python.org/pypi/segments) from the Python Package Index (PyPI) run:

```
 pip install segments
``` 

on the command line. This will give you access to both the CLI and programmatic functionality in Python scripts, when you import the `segments` library.

You can also install the `segments` package with from the [Github repository](https://github.com/cldf/segments):

```
 git clone https://github.com/cldf/segments.git
 cd segments
 python setup.py develop
```

## Installing R `qlcTokenize` library

To install the qlcTokenize library and accompanying data, install `qlcData`:

```
 install.packages("devtools")
 devtools::install_github("cysouw/qlcData", build_vignettes = T)
```

and then load the library:

```
 library(qlcData)
```

## Recipes

Each recipe contains a short use case with accompanying code. The directory structure is typically as follows:

```
|-- Recipe name
|    |-- recipe files
|    |-- data
|    |    └── orthography profiles
|    |-- sources
|    |    └── input data
|    |-- sandbox
|    |    └── where the output is written
```


