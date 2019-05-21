# Cookiecutter Python Package Template with Pipenv

[![travis](https://travis-ci.com/elgertam/cookiecutter-pipenv.svg?branch=master)](https://travis-ci.com/elgertam/cookiecutter-pipenv)

[Cookiecutter](https://github.com/audreyr/cookiecutter) template for a Python package with [Pipenv](https://docs.pipenv.org/).

- GitHub repo: <https://github.com/elgertam/cookiecutter-pipenv/>
- Documentation: <https://cookiecutter-pipenv.readthedocs.io/>
- Free software: BSD license

## Why Pipenv

Packaging in Python can be a pain, but it doesn\'t need to be. The new Pipenv project has rapidly improved packaging in Python by tackling two related problems: automatic package dependency management and virtualenv management. Pipenv uses the new [Pipfile](https://github.com/pypa/pipfile) format that is a replacement for [requirements.txt]{.title-ref}. Pipenv is an improvement over the `requirements.txt` format, and is used in the Python [tutorial](https://packaging.python.org/tutorials/managing-dependencies/#managing-dependencies).

## Features

- Testing setup with `unittest` and `python setup.py test` or `py.test`
- [Travis-CI](http://travis-ci.org/): Ready for Travis Continuous Integration testing
- [Tox](http://testrun.org/tox/) testing: Setup to easily test for Python 2.7, 3.5, 3.6, 3.7
- [Sphinx](http://sphinx-doc.org/) docs: Documentation ready for generation with, for example, [ReadTheDocs](https://readthedocs.io/)
- [Bumpversion](https://github.com/peritus/bumpversion): Pre-configured version bumping with a single command
- Auto-release to [PyPI](https://pypi.org/) when you push a new tag to master (optional)
- Command line interface using Click (optional)

## Quickstart

Install the latest Cookiecutter if you haven\'t installed it yet (this requires Cookiecutter 1.4.0 or higher):

    pip install -U cookiecutter

Install the latest Pipenv:

    pip install -U pipenv

Generate a Python project that uses Pipenv:

    cookiecutter gh:elgertam/cookiecutter-pipenv

Once your project has been created, change directories:

    cd <project-name>

Then:

- Create a repo and put it there (e.g. `git init`).
- Install the dev requirements into a virtualenv (`pipenv install --dev`).
- Add the repo to your [Travis-CI](http://travis-ci.org/) account.
- [Register](https://packaging.python.org/distributing/#register-your-project) your project with PyPI.
- Run the Travis CLI command [travis encrypt \--add deploy.password]{.title-ref} to encrypt your PyPI password in Travis config and activate automated deployment on PyPI when you push a new tag to master branch.
- Add the repo to your [ReadTheDocs](https://readthedocs.io/) account + turn on the ReadTheDocs service hook.
- Release your package by pushing a new tag to master.
- Activate your project on [pyup.io](https://pyup.io/).

### Fork This / Create Your Own

This project itself is a fork of Audrey Roy Greenfeld\'s exceptional [cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage). If you have differences in your preferred setup, I encourage you to forkthis to create your own version. Or create your own; it doesn\'t strictly have to be a fork.

### Or Submit a Pull Request

I will consider pull requests as they come in, if they enhance the overall packaging experience.
