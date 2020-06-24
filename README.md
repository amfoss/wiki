# amFOSS Wiki

amFOSS Wiki built with Sphinx using a theme provided by Read the Docs. 

## :minidisc: Installation Instructions

### Install requirements on Linux

Before installing the `Sphinx` and `readthedocs.org` packages, you will need: 
* the `python3` language and its `pip3` package manager
* a version of [GNU Make](https://www.gnu.org/software/make/),
* the [git tool](https://git-scm.com).

### Install requirements on Windows

Like on Linux environments, on Microsoft Windows, you need to install:
* the `python` language and its `pip` package manager
* All the `python` modules requirements with the `pip` command
* `GNU Make` tool.
* `git` tool.

### Installing Sphinx (every platform)

To build the HTML website (or any other format supported by Sphinx, like PDF, EPUB or LaTeX), you need to install [Sphinx](https://sphinx-doc.org/) >= 1.3 as well as (for the HTML) the [readthedocs.org theme](https://github.com/snide/sphinx_rtd_theme).

Those tools are best installed using [pip](https://pip.pypa.io), Python's module installer. The Python 3 version might be provided (on Linux distros) as `pip3` or `python3-pip`. 

Clone the repository

```sh
$ git clone https://gitlab.com/amfoss/wiki.git
$ cd wiki
```

Create a python3 virtualenv, and activate the environment

```sh
$ virtualenv -p python3 venv
$ source venv/bin/activate
```

You can then run:

```sh
$ pip3 install -r requirements.txt
```

### Building the HTML website 

You can then build the HTML documentation from the root folder of this repository with:

```sh
$ make html
```

On Windows, building is still done at the root folder of this repository using the following command (`make` linux command is replaced with `make.exe`):
```sh
$ make.exe html
```

You can then test the changes live by opening `build/html/index.html` in your favorite browser.

**Debugging Tip:**
- Delete the build cache before building documents if you make changes in the code by running the command `make clean` or using the `sphinx-build -E` option.
