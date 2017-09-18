---
title: 搭建 Python 虚拟环境 virtualenv 和 virtualenvwrapper
comments: true;
categories:
- python

---

```
pip3 install virtualenv
pip3 install virtualenvwrapper

```

```
vi ~/.bash_profile
export WORKON_HOME=$HOME/code/.virtualenvs
export PROJECT_HOME=$HOME/code
export VIRTUALENVWRAPPER_PYTHON=/usr/local/bin/python3
export VIRTUALENVWRAPPER_VIRTUALENV=/usr/local/bin/virtualenv
export VIRTUALENVWRAPPER_VIRTUALENV_ARGS='--no-site-packages'

source /usr/local/bin/virtualenvwrapper.sh
```

```
source ~/.bash_profile
mkvirtualenv test
workon test
deactivate
rmvirtualenv

```

虚拟环境路径
![虚拟环境路径](/img/virtualpath.png)

python3 manage.py shell 练习 
