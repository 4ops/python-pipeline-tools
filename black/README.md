# Components

## black

*Black* is the uncompromising Python code formatter.  By using it, you
agree to cede control over minutiae of hand-formatting.  In return,
*Black* gives you speed, determinism, and freedom from `pycodestyle`
nagging about formatting.  You will save time and mental energy for
more important matters.

Project link: <https://black.readthedocs.io/en/stable/>

# Usage

GitLab CI config example:

```YAML
stages:
  - test

python:code-formatting:
  stage: test
  image: 4ops/black:latest
  script: black --check .
```
