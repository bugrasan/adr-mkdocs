# README

## Installation

Pre-reqs:
- python
- pip
- virtualenv

```bash

# if `virtualenv` isn't already installed then install it first
# install mkdocs, themes, and plugins
virtualenv adr-company
cd adr-company
source bin/activate

# install mkdocs, themes, plugins
pip install mkdocs
pip install mkdocs-material
pip install mkdocs-awesome-pages-plugin

# install adr-tools
pip install adr-tools-python
#adr-init  docs/adr
#adr-new <decision>
#adr-list

# optional original adr-tools as bash scripts
#git clone https://github.com/adr/adr-tools.git
#export PATH=$PATH:

```

## Documentations

- [mkdocs](https://www.mkdocs.org/)
- [mkdocs-material](https://squidfunk.github.io/mkdocs-material/)
- [mkdocs-awesome-pages-plugin](https://pythonawesome.com/mkdocs-plugin-that-simplifies-configuring-page-titles-and-their-order/)
- [mkdocs-with-pdf](https://pypi.org/project/mkdocs-with-pdf/)
- [mkdocs-print-site-plugin](https://timvink.github.io/mkdocs-print-site-plugin/index.html)
- [adr-tools-python](https://pypi.org/project/adr-tools-python/)
- [adr-tools](https://github.com/npryce/adr-tools) - original bash scripts


## PDF
```bash
# this plugins seems to be outdated
#pip install -e git+https://github.com/jwaschkau/mkpdfs-mkdocs-plugin.git#egg=mkpdfs-mkdocs
#pip install --upgrade weasyprint==52.5

# this works fine
pip install mkdocs-with-pdf

# generate export page
pip3 install mkdocs-print-site-plugin


```

## References 

- https://github.com/elastisys/compliantkubernetes/blob/main/mkdocs.yml
	- https://elastisys.io/compliantkubernetes/adr/0000-use-markdown-architectural-decision-records/

