# EcoFOCI CodeLab

The [EcoFOCI CodeLab](https://shaunwbell.github.io/ioos_code_lab) is a collection of tutorials and examples of how to access and
utilize the many EcoFOCI Data sets and resources available. This site is geared towards scientists and collaborators with internal access to EcoFOCI resources. Most notebook examples are written in Python.

See the rendered version at https://shaunwbell.github.io/ecofoci_code_lab

To suggest a notebook or ask questions please open an issue at: https://github.com/ioos/ioos_code_lab/issues

This is a fork of the IOOS CodeLab (thanks to that project for the initial codebase) and the IOOS project can be obtained at: https://github.com/ioos/ioos_code_lab - the citation link included in this repo still refers to the original project.

## Run on Pangeo Binder - ??? disabld for now

## Citation

ioos_code_lab initial citation:  
[![DOI](https://zenodo.org/badge/399546690.svg)](https://zenodo.org/badge/latestdoi/399546690)

---

## Build the JupyterBook locally

### Resources:

- Jupyter-book command line interface: https://jupyterbook.org/basics/build.html

### Requirements:

- Git: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
- Jupyter{Book}: https://jupyterbook.org/intro.html
- Web Browser

### Installation

Install jupyter-book:

```
conda install jupyter-book
```

Clone the [ecofoci_code_lab](https://github.com/shaunwbell/ecofoci_code_lab) repository.

```
git clone https://github.com/shaunwbell/ecofoci_code_lab.git
```

Once you have cloned the repository, you have all the required notebooks cloned onto your system
(in the `/jupyterbook/content` directory).

### Build the JupyterBook

Run the following command to build the JupyterBook.

```
jupyter-book build jupyterbook/
```

The command should be run relative to the `jupyterbook/` directory.

If you are in the `jupyterbook/` directory, you can build the book using

```
juyter-book build .
```

### View the built JupyterBook

Your book's HTML pages are here:

```
jupyterbook\_build\html\
```

You can look at your book by opening this file in a browser:

```
jupyterbook\_build\html\index.html
```

Or, use the full link displayed in the terminal to view the website.

### Clean up the book's generated files

To entirely remove the folders in the `_build/` directory:

```
jupyter-book clean jupyterbook/ --all
```
