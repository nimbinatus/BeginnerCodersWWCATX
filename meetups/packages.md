[Back to the index](/BeginnerCodersWWCATX)

# Using pip, easy_install, and packages

_A Primer for Women Who Code ATX_

## Packages

First, a _module_ in Python is a collection of functions (or methods, if you
want to get fancy), variable definitions, and classes. As noted in the
[Python Packaging docs](https://packaging.python.org/glossary/), it's a "basic
unit of code reusability" for Python. _Packages_ are collections of Python
modules and other files that collectively make up a released bit of software.
You can think of them as Python building blocks.

## Pip and easy_install

When getting started with pip, you're actually going to install it with
easy_install. Pip is a package itself. If you have Python 2.7.9 or greater or
Python 3.4 or greater, you already have pip. Congratulations!

If you have an older version of Python (and you can't upgrade... you should try
to upgrade first if you can), you'll need to install it. To get it, you can
invoke easy_install, one of the setup tools bundled with Python, from your
command line like this:

    easy_install pip

You may have to use `sudo` to install pip (`sudo easy_install pip`), but pip
should be the only package you ever use `sudo` to install with Python. See the
next section for the reason why.

You can also install it with your local package manager most of the time, or you
can download it and install it. Follow the directions at
[https://pip.pypi.org/en/latest/installing/](https://pip.pypi.org/en/latest/installing/)
if you're unsure.

### What's the difference between pip and easy_install?

There's a few differences, actually. First, understand that pip is the standard,
and no one really uses easy_install any longer. Pip showed up four years or so
after easy_install, so there are some things that it was designed for that
people saw as flaws with easy_install.

Easy_install takes an _egg_, or a boxed up version of a package that can be
either unzipped and installed or run directly in the interpreter, as input. Pip,
on the other hand, takes a _wheel_, or a zipped package with metadata attached,
as input. Both of them use setuptools under the hood in one form or another to
take those inputs and install them.

Pip has one great thing going for it: the ability to install from a requirements
file. Using a requirements file allows developers to ensure a program will run
on different systems because they can tell the system exactly what the program
needs to run on. Sometimes new releases of different packages can cause breaking
changes--changes that prevent a system from running,--which can cause havoc in
production systems.

The big things to know is that eggs are slowly being replaced completely by
wheels and that wheels are the current standard. If you want to learn more about
wheels, check out
[PEP (Python Enhancement Proposal) 427](https://www.python.org/dev/peps/pep-0427/).

If you want to see a full rundown of the differences, check out
[this list](https://packaging.python.org/pip_easy_install/).

### Pitfalls of sudo

Never ever use sudo with pip. You will corrupt your Python installation on your
machine. It's much better to use virtual environments (for example, with the
packages virtualenv or virtualenvwrapper. I prefer the latter.), which is a
later topic.

Need to install something but don't have admin access? You can install it
locally just for you. run

    pip install --user <package-name>

## What can be found with pip?

You have a couple options to look up packages with pip.

### Command line

Using the command line is probably the way most programmers look up packages
available with the pip command. Simply use the following syntax:

    pip search <keyword>

Replace `<keyword>` with the package name, and you're off searching through the
index.

### Web

You can also go explore the packages available to you through pip on the
[Python Package Index](https://pypi.python.org/), which is often just
abbreviated as PyPI.

## Resources

-   [Python Packaging User Guide](https://packaging.python.org/)
-   [Python Package Index](https://pypi.python.org/)
-   [Pip documentation](https://pip.pypa.io/en/stable/)
