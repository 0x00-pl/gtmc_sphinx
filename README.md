# gtmc_sphinx

## install
### Installing Sphinx
follow the guide in https://www.sphinx-doc.org/en/master/usage/installation.html .

### installing plugins
>  `python3 -m pip install -r requirements.txt`

## build

Use the Makefile to build the docs, like so:

>  `make <builder>`

where `<builder>` is one of the supported builders, e.g. `html`, `latex` or `linkcheck`.

## publish
using gitlab action for now.

## Contribute to GTMC
Sphinx Document: 
- https://www.sphinx-doc.org/en/master/tutorial/first-steps.html

reStructuredText syntax:
- https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html

markdown plugin (`myst-parser`):
- https://www.sphinx-doc.org/en/master/usage/markdown.html

myst-parser syntax extensions:
- https://myst-parser.readthedocs.io/en/latest/configuration.html#list-of-syntax-extensions
- https://myst-parser.readthedocs.io/en/latest/syntax/optional.html#syntax-extensions

markdown example on live-preview:
- https://myst-parser.readthedocs.io/en/latest/live-preview.html

markdown cross-references:
- https://myst-parser.readthedocs.io/en/latest/syntax/cross-referencing.html
