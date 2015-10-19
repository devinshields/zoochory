# zoochory
A runnable tutorial on how to create and deploy a python module to the Python Package Index (and how to make it pip-installable).

[Zoochory](https://en.wikipedia.org/wiki/Seed_dispersal#By_animals) is a fancy name seeds piggybacking on animals, catching a ride to their new home.


Getting Started
---------------

* create an account at [python.org](https://www.python.org/) and at [pypi](https://pypi.python.org/pypi).

* [RTFM](https://packaging.python.org/en/latest/distributing/#packaging-and-distributing-projects) for Packaging and Distributing Projects from the [Python Packaging User Guide](https://packaging.python.org/en/latest/).

* make a new virtual environment

```
virtualenv venv
source venv/bin/activate
```

* [install twine (and track dependencies)](https://packaging.python.org/en/latest/distributing/#requirements-for-packaging-and-distributing)

```
pip install twine
pip freeze > requirements.txt
```

* take a look at [this complete sample project](https://github.com/pypa/sampleproject) from the pypi team

* update setuptools and install wheel

```
pip install -U pip setuptools
pip install wheel
pip freeze > requirements.txt
```

* learn about the [setup.py](https://packaging.python.org/en/latest/distributing/#setup-py)
   * "The primary feature of setup.py is that it contains a global setup() function"

* learn about the other special purpose files in an installable package
  * [setup.cfg](https://packaging.python.org/en/latest/distributing/#setup-cfg)
  * [README.rst](https://packaging.python.org/en/latest/distributing/#readme-rst)
  * [MANIFEST.in](https://packaging.python.org/en/latest/distributing/#manifest-in)

* download the example files so we can start tweaking them

```
wget https://raw.githubusercontent.com/pypa/sampleproject/master/setup.py
wget https://raw.githubusercontent.com/pypa/sampleproject/master/setup.cfg
wget https://raw.githubusercontent.com/pypa/sampleproject/master/README.rst
wget https://raw.githubusercontent.com/pypa/sampleproject/master/MANIFEST.in
```




