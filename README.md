# Python Package

An empty python package.

[![Built with Cookiecutter Python Package](https://img.shields.io/badge/built%20with-Cookiecutter%20Python%20Package-ff69b4.svg?logo=cookiecutter)](https://github.com/91nunocosta/python-package-cookiecutter)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
![Code Coverage](coverage.svg)

## Contributing

### How to prepare the development environment

1. Clone the repository.

   ```bash
   git clone git@github.com:91nunocosta/python-package.git
   ```

2. Open the project directory.

   ```bash
   cd python-package
   ```

3. Install [_poetry_](https://python-poetry.org/) _package and dependency manager_.
Follow the [poetry installation guide](https://python-poetry.org/docs/#installation).
Chose the method that is more convenient to you, for example:

   ```bash
   curl -sSL\
        https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py \
      | python -
   ```

4. Create a new virtual environment (managed by _poetry_) with the project dependencies.

   ```bash
   poetry install
   ```

5. Enter the virtual environment.

   ```bash
   poetry shell
   ```

### How to check code quality

1. Prepare the development environment, as described in
[**How to prepare the development environment**](#how-to-prepare-the-development-environment).

2. Lint and test code

     ```bash
     pre-commit run --all-files
     ```

3. Test package artifact

    ```bash
    tox
    ```
