# flymake-python-mypy

A flymake handler for python files with mypy.

## Usage

Install mypy:
```
pip install mypy-lang
```

Add following lines to emacs init file:

```
(require 'flymake-mypy)
(add-hook 'python-mode-hook 'flymake-python-mypy-load)
```

To use new type annotations in python 3.6 (PEP 526) like ```foo: int```, add this line:
```
(setq flymake-python-mypy-pep526 t)
```
