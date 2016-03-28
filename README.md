pyenv-alias
===========

pyenv-alias is a [pyenv](https://github.com/yyuu/pyenv) plugin which allows you
to specify a 'version name alias' when installing python.

Out of the box, pyenv does not allow you to install multiple copies of the same
python version. This can be limiting in situations where you want to have
different instances of python with, for example, different compile-time
configurations.

## Installation

```
git clone https://github.com/s1341/pyenv-alias.git $(pyenv root)/plugins/pyenv-alias
```

## Usage

Specify the version alias name using the `VERSION_ALIAS` environment variable
when performing a `pyenv install`

For example, building a version of python 2.7.6 with the shared `.so`:

```
VERSION_ALIAS="2.7.6_shared" PYTHON_CONFIGURE_OPTS="--enable-shared" pyenv install 2.7.6
```
