# Python template
My base copier template for python projects

## How to use
Run copier, for example, like this:

```bash
copier gh:acid9reen/python_template <target_directory>
```

## Project structure
```
├───src
│   └───{{package_name}}
│       ├───__init__.py
│       └───py.typed
├───tests
│   └───__init__.py
├───.gitignore
├───.pre-commit-config.yaml
├───README.md
└───pyproject.toml
```

Project have 'src' layout for main package. Also notice 'py.typed' file, existence of it says that project is typed.

## What's included?
* Python package and tools configuration via pyproject.toml
* [Mypy](https://github.com/python/mypy) static typing
* [PyTest](https://github.com/pytest-dev/pytest) as testing framework
* A bunch of pre-commit hooks:
    * [Ruff linter](https://github.com/charliermarsh/ruff) + autoformat (including flake8-bugbear and flake8-quotes functionality)
    * [Reorder python imports](https://github.com/asottile/reorder_python_imports)
    * [Add trailing comma](https://github.com/asottile/add-trailing-comma)
    * [Pre commit hooks](https://github.com/pre-commit/pre-commit-hooks):
        * check-yaml
        * end-of-file-fixer
        * trailing-whitespace
        * debug-statements
