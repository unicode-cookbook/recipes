# Recipes for the Unicode Cookbook

[Steven Moran](https://scholar.google.com/citations?user=PpTOh08AAAAJ&hl=en) & [Michael Cysouw](http://cysouw.de/home/index.html)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview

This directory contains recipes (use cases) that supplement [The Unicode Cookbook for Linguists](https://github.com/unicode-cookbook/cookbook/blob/master/unicode-cookbook.pdf). Each recipe is in its own subdirectory:

- [Basics](https://github.com/unicode-cookbook/recipes/tree/master/Basics): basics of grapheme segmentation and text tokenization in the [Python](https://www.python.org/) and [R](https://www.r-project.org/) programming languages
- [ASJP](https://github.com/unicode-cookbook/recipes/tree/master/ASJP): tokenize ASJP wordlists with the R
- [Dogon](https://github.com/unicode-cookbook/recipes/tree/master/Dogon): tokenize the [Dogon comparative wordlist](http://dogonlanguages.org/values) and create an orthography profile in Python with [Pandas](https://pandas.pydata.org/)
- [Dutch](https://github.com/unicode-cookbook/recipes/tree/master/Dutch): create an orthography profile for tokenizing Dutch orthography with R
- [JIPA](https://github.com/unicode-cookbook/recipes/tree/master/JIPA): tokenize text in the [International Phonetic Alphabet (IPA)](https://www.internationalphoneticassociation.org/content/ipa-chart) with Python or R


## Installing Python `segments` package

To install the Python [segments package](https://pypi.python.org/pypi/segments) from the Python Package Index (PyPI) run:

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

## Installing R `qlcData` library

To install the qlcData library and accompanying data, install `qlcData`:

```
 install.packages("devtools")
 devtools::install_github("cysouw/qlcData", build_vignettes = T)
```

and then load the library:

```
 library(qlcData)
```

To access help, call:

```
help(qlcData)
```

To access the [vignette](https://cran.r-project.org/web/packages/qlcData/vignettes/orthography_processing.html), call:

```
vignette("orthography_processing")
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


