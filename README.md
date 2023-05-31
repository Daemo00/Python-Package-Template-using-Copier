# Python Package Template using Copier

Template for generating Python Packages using _Copier_ (https://github.com/copier-org/copier).

Installs and uses _pre-commit_ (https://pre-commit.com) in generated Package.

## Installation

Suggested way of installing the dependencies is _pipx_ (https://pypa.github.io/pipx):
```shell
# Install pipx
python3 -m pip install --user pipx
python3 -m pipx ensurepath
# Install dependencies
pipx install copier pre-commit
```

## Usage

Create a new Package `MyPackage` with:
```shell
copier copy https://github.com/Daemo00/Python-Package-Template-using-Copier MyPackage
```

Update an existing Package in `MyPackage` directory with:

```shell
cd MyPackage
copier update .
pre-commit run --all-files
git commit --all --message "Template Update"  # Check the changes and commit
```
