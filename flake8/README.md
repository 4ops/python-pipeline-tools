# Components

## flake8

Flake8 is a wrapper around these tools:
* PyFlakes
* pycodestyle
* Ned Batchelder's McCabe script

Project link: <https://gitlab.com/pycqa/flake8>

## flake8-mypy

A plugin for Flake8 integrating mypy. The idea is to enable limited type checking as a linter inside editors and other tools that already support Flake8 warning syntax and config.

Project link: <https://github.com/ambv/flake8-mypy>

# Usage

GitLab CI config example:

```YAML
stages:
  - test

python:syntax:
  stage: test
  image: 4ops/flake8:latest
  script: flake8 --verbose .
```
