# Linter for jinja2 #

This repository contains a simple j2 linter which is useful for checking jinja2 template syntax. 

## Requirements ##

Python

Ansible

## How to use ##
```
cp j2lint.py /usr/local/bin/
j2lint.py my-template.j2
```

It accepts multiple arguments so shell expansion and/or combining with find is no issue:

```
j2lint.py *.j2
find src -type f -name "*.j2" -exec j2lint.py '{}' +
```