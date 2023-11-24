---
layout: default
title: Python Virtual Environment
parent: Python Development
---


## Python Virtual Environment

Python envoronment includes, the python.exe itself and installed
packages (scipy, numpy, and others)

By default, the python is installed to your system. Every time you
need to run a script, the system looks for the "globally" installed
version of Python and packages.

In case of software development, the globally installed python is a
bad option.

1. Sometimes you need to use different versions of packages for
   different projects
2. All the developers must use the same versions (even outdated) of
   packages
3. Different packages are required for different projects. So it is
   better to keep only those, used in current project.

## venv

*venv* is the python package, that allows to create a virtual
environment. It creates a separate folder with specific verion of
python and all the packages.

User can activate a specific environment at any time.

It is a good practice to keep a virtual environment inside directory
with other project related files (source code, tests, documentation,
etc.).

It is also improtant to include the environment to *.gitignore* list.
The environment uses a lot of space, and must be stored locally.

## python installation

Make sure at least one version of python is installed on your PC.
The latest version can be downloaded from the
[official webiste](python.org)

Anaconda is not considered as a separate installation.

## how to initialize venv

1. Open system terminal (cmd.exe)
2. Navigate to a directory where new python and packages will be
   installed. Make sure, the directory exists

```cmd
cd ./src/my-new-code
```

1. create a new environment in *venv* directory. Here the first *venv*
   is the name of python package you call, the second *venv* is the
   name of directory, where the environment will be created.

```cmd
python -m venv venv
```

## gitignore

## install required packages

## save list of packages

## activate

## deactivate