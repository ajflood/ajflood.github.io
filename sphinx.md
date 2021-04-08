# How I use sphinx for documentation

## Setup
- `mkdir docs`
- `cd docs`
- `sphinx-quickstart`
- 

## General use
- Doc string:
	```
	"""[summary]

	:param inputs: [description]
	:type inputs: [type]
	"""
	```

- Comments:
  ``` #: some comment ```

## Config stuff example
```
# Configuration file for the Sphinx documentation builder.
#
# This file only contains a selection of the most common options. For a full
# list see the documentation:
# https://www.sphinx-doc.org/en/master/usage/configuration.html

# -- Path setup --------------------------------------------------------------
import os
import sys
sys.path.insert(0, os.path.abspath('../'))

from sphinx.ext.autodoc import (
    ClassLevelDocumenter, InstanceAttributeDocumenter)
def iad_add_directive_header(self, sig):
    ClassLevelDocumenter.add_directive_header(self, sig)
InstanceAttributeDocumenter.add_directive_header = iad_add_directive_header

# -- Project information -----------------------------------------------------
project = 'XXX'
copyright = '2021, YYY'
author = 'YYY'

# The full version, including alpha/beta/rc tags
release = 'WY.WY'

master_doc = 'index'
latex_doc = 'galvodriver.tex'

# -- General configuration ---------------------------------------------------
extensions = [
    'sphinx.ext.autodoc',
    'sphinx.ext.viewcode',
    'sphinx.ext.githubpages',
]


# -- Options for LaTeX output ------------------------------------------------
latex_engine = 'pdflatex'
latex_elements = {
    'papersize': 'letterpaper',
    'pointsize': '12pt',
    'preamble': r'''
        \renewcommand{\cleardoublepage}{}
        \renewcommand{\printindex}{}''',
    'tableofcontents': r''' ''',

}
latex_domain_indices = False
texinfo_domain_indices = False
```

## Sample index file
```
.. Galvo Driver documentation master file, created by
   sphinx-quickstart on Thu Apr  8 09:14:11 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Galvo Driver's documentation!
========================================


.. autoclass:: GalvoDriver.galvo
   :members:
   :undoc-members:
```

## Sample build bash file
```
#!/bin/bash

project="galvodriver"

make latex
cd _build/latex
pdflatex $project.tex
pdflatex $project.tex
mv $project.pdf ../../
```