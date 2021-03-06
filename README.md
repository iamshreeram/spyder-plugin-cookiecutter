# Spyder Plugin Cookiecutter

[![CircleCI](https://circleci.com/gh/spyder-ide/spyder-plugin-cookiecutter.svg?style=svg)](https://circleci.com/gh/spyder-ide/spyder-plugin-cookiecutter)

Powered by [Cookiecutter](https://github.com/audreyr/cookiecutter), Spyder Plugin Cookiecutter is a template for jumpstarting [Spyder IDE](https://github.com/spyder-ide/spyder) plugins quickly.

> This is under development, you can use it, but some features are missing

> We recommend using conda and anaconda when developing a Spyder-IDE plugin.

## Features

- For Spyder >=3.1
- Spyder Plugin Structure (plugin.py, gui.py)
- A functional basic plugin [under development]

### Repo structure
- Licence, Manifiest, Contibutors, .gitatributes
- Readme with bagdes and some instructions.

### Packaging

- requierements.txt
- conda recipe [under development]
- setup.py

### Continuous Integration

- appveyor [under development]
- travis [under development]
- circle-ci [under development]

### Code Checking

- coverage [under development]
- ciocheck [under development]
- scrutinizer [under development]
- quantified code [under development]

### Repo Managing

- versionner


## Usage

First, get Cookiecutter:

```
$ conda install "cookiecutter>=1.4.0"
```

If you want to use versioneer: (also you need to install git)

```
$ conda install versioneer
```

Now run against the repo:

```
$ cookiecutter gh:spyder-ide/spyder-plugin-cookiecutter
```

You'll be prompted for some values. and after that the repo will be generated

Normally you don't need to change `project_name` and `repo_name`.

Example:

```
author [Spyder Project Contributors]:
email [admin@spyder-ide.org]:
github_username [spyder-ide]:
plugin_name [Demo Plugin]: Reports
repo_name [spyder-reports]:
project_name [spyder_reports]:
description [Plugin for Spyder IDE.]: Spyder Plugin for Markdown reports for Pweave and Stitc
version [0.1.0]:
create_config_page [n]:
use_ciocheck [y]:
support_python_2 [n]:
use_versioneer [y]:
```

## Testing

For testing you need to install pytest and pytest-cookies

```
$ pip install pytest pytest-cookies
```

And run pytest:

```
$ pytest
```
