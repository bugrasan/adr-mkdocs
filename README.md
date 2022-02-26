# README

## Installation
pre-reqs:
- python

### Windows
- install `winget` as [described](https://docs.microsoft.com/en-us/windows/package-manager/winget/)
	- install python from elevated shell (with Administrator rights)
		```powershell
		winget install python.python3
		```
- in Windows Terminal:
	```powershell
	# check proper installation of python
	python --version
	# install virtualenv
	pip install virtualenv
	git clone <this-repo>
	cd <repo>
	virtualenv .

	# activate the virtualenv
	Scripts/activate
	# install all requirements (mkdocs, themes, plugins)
	pip install -r requirements.txt
	# test ADR
	mkdocs serve
	```

### Linux
```bash
# if `virtualenv` isn't already installed then install it first
pip install virtualenv

git clone <this-repo>
cd <repo>
virtualenv .
# assuming using bash as shell
source bin/activate

# install mkdocs, themes, plugins
pip install -r requirements.txt


# optional: install original adr-tools as bash scripts
#git clone https://github.com/adr/adr-tools.git
#export PATH=$PATH:$(pwd)\adr-tools\src\
```


## Documentations
- [mkdocs](https://www.mkdocs.org/)
- [mkdocs-material](https://squidfunk.github.io/mkdocs-material/)
- [mkdocs-awesome-pages-plugin](https://pythonawesome.com/mkdocs-plugin-that-simplifies-configuring-page-titles-and-their-order/)
- [mkdocs-with-pdf](https://pypi.org/project/mkdocs-with-pdf/)
- [mkdocs-print-site-plugin](https://timvink.github.io/mkdocs-print-site-plugin/index.html)
- [adr-tools-python](https://pypi.org/project/adr-tools-python/)
- [adr-tools](https://github.com/npryce/adr-tools) - original bash scripts


### adr-tools help
```bash
# init ADR repository, default folder is 'docs/adr'
adr-init <directory>
# new arch decision, name is description (and can contain blanks)
adr-new <name>
# list all decisions
adr-list
```


## PDF
```bash
# this plugins seems to be outdated
#pip install -e git+https://github.com/jwaschkau/mkpdfs-mkdocs-plugin.git#egg=mkpdfs-mkdocs
#pip install --upgrade weasyprint==52.5

# this works fine
# **IMPORTANT** but not on windows!!
pip install mkdocs-with-pdf
# TODO - find a solution for windows

# generate export page
pip3 install mkdocs-print-site-plugin

```

## References 

- https://github.com/elastisys/compliantkubernetes/blob/main/mkdocs.yml
	- https://elastisys.io/compliantkubernetes/adr/0000-use-markdown-architectural-decision-records/
