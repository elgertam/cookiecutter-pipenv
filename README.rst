================================================
Cookiecutter Python Package Template with Pipenv
================================================

|travis|

.. |travis| image:: https://travis-ci.com/elgertam/cookiecutter-pipenv.svg?branch=master
    :target: https://travis-ci.com/elgertam/cookiecutter-pipenv


Cookiecutter_ template for a Python package with Pipenv_.

* GitHub repo: https://github.com/elgertam/cookiecutter-pipenv/
* Documentation: https://cookiecutter-pipenv.readthedocs.io/
* Free software: BSD license

Why Pipenv?
-----------

Packaging in Python can be a pain, but it doesn't need to be. The new Pipenv project
has rapidly improved packaging in Python by tackling two related problems: automatic
package dependency management and virtualenv management. Pipenv uses the new Pipfile_
format that is the endorsed replacement for `requirements.txt`. Pipenv is the future of
Python package management, and is even recommended to newcomers in the Python tutorial_.

Features
--------

* Testing setup with ``unittest`` and ``python setup.py test`` or ``py.test``
* Travis-CI_: Ready for Travis Continuous Integration testing
* Tox_ testing: Setup to easily test for Python 2.7, 3.5, 3.6, 3.7
* Sphinx_ docs: Documentation ready for generation with, for example, ReadTheDocs_
* Bumpversion_: Pre-configured version bumping with a single command
* Auto-release to PyPI_ when you push a new tag to master (optional)
* Command line interface using Click (optional)

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _Pipenv: https://docs.pipenv.org/
.. _Pipfile: https://github.com/pypa/pipfile
.. _tutorial: https://packaging.python.org/tutorials/managing-dependencies/#managing-dependencies

Quickstart
----------

Install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher)::

    pip install -U cookiecutter

Install the latest Pipenv::

    pip install -U pipenv

Generate a Python project that uses Pipenv::

    cookiecutter gh:elgertam/cookiecutter-pipenv

Once your project has been created, change directories::

    cd <project-name>

Then:

* Create a repo and put it there (e.g. ``git init``).
* Install the dev requirements into a virtualenv (``pipenv install --dev``).
* Add the repo to your Travis-CI_ account.
* Register_ your project with PyPI.
* Run the Travis CLI command `travis encrypt --add deploy.password` to encrypt your PyPI password in Travis config
  and activate automated deployment on PyPI when you push a new tag to master branch.
* Add the repo to your ReadTheDocs_ account + turn on the ReadTheDocs service hook.
* Release your package by pushing a new tag to master.
* Activate your project on `pyup.io`_.

.. _Register: https://packaging.python.org/distributing/#register-your-project

Fork This / Create Your Own
~~~~~~~~~~~~~~~~~~~~~~~~~~~

This project itself is a fork of Audrey Roy Greenfeld's exceptional
cookiecutter-pypackage_. If you have differences in your preferred setup, I
encourage you to fork this to create your own version. Or create your own;
it doesn't strictly have to be a fork.

.. _cookiecutter-pypackage: https://github.com/audreyr/cookiecutter-pypackage

Or Submit a Pull Request
~~~~~~~~~~~~~~~~~~~~~~~~

I will consider pull requests as they come in, if they enhance the overall packaging experience.

.. _Travis-CI: http://travis-ci.org/
.. _Tox: http://testrun.org/tox/
.. _Sphinx: http://sphinx-doc.org/
.. _ReadTheDocs: https://readthedocs.io/
.. _`pyup.io`: https://pyup.io/
.. _Bumpversion: https://github.com/peritus/bumpversion
.. _PyPi: https://pypi.org/
