:tocdepth: 2

=================================
Lesson 1: Goals and Prerequisites
=================================

*****
Goals
*****

- Hands-on experience building a website.
- Create a website that helps promote your work or tells a story
  you're working on.
- Fundamental tools:
    - Markup (HTML)
    - Styling (CSS)
    - Versioning (Git)
    - Responsive design (Bootstrap)
    - Data management, templating, and publishing (Tarbell)

**********
Background
**********

*************
Prerequisites
*************

1. A laptop with OS X 10.7+ or Linux
2. A `command-line interface <https://en.wikipedia.org/wiki/Command-line_interface>`_ to interact with your computer
3. A `text editor <https://en.wikipedia.org/wiki/Text_editor>`_ to work with plain text files
4. Version 2.7 of the `Python <http://python.org/download/releases/2.7.6/>`_ programming language
5. The `pip <http://www.pip-installer.org/en/latest/installing.html>`_ package manager
6. `Git <http://git-scm.com/>`_ version control software
7. An account at `GitHub.com <http://www.github.com>`_
8. A `Google <http://google.com>`_ account and `client_secrets.json <http://tarbell.readthedocs.org/en/latest/install.html#configure-google-spreadsheet-access-optional>` file.
9. `Tarbell <http://tarbell.tribapps.com>`_ publishing software

.. note::

    Depending on your experience and operating system, you might already be ready
    to go with everything above. If so, move on to the next chapter. If not, 
    don't worry. And don't give up! It will be a bit of a 
    slog but the instructions below will point you in the right direction.


Bring your own laptop
---------------------

This will be no fun for anybody if you don't have an OS X or Linux-based laptop to
bring to the workshops.


---------------------
Command-line interface
---------------------

A command line interface, also known as a terminal, is a program that lets you
type in commands that control your computer.

- Apple OS X: Open the `"Terminal" application <http://blog.teamtreehouse.com/introduction-to-the-mac-os-x-command-line>`_. 
- Ubuntu Linux: Open the `"Terminal" application <http://askubuntu.com/questions/38162/what-is-a-terminal-and-how-do-i-open-and-use-it>`_.

.. note::

    Very little command line skills will be required for this tutorial. You'll need to run some
    commands to install the necessary software, and will use the command line to publish your
    project.


---------------------
Text editor
---------------------

You'll be editing simple `"plain text" files <https://en.wikipedia.org/wiki/Text_file>`_.

Just like you need a word processor for writing human language, you need a text editor
for working with plain text such as HTML markup, CSS, and Javascript.

We recommend `Sublime Text <http://www.sublimetext.com/3>` for all participants. It's fast,
simple, and sensible.


---------------------
Python
---------------------

To make sure your system has Python 2.7 installed, type the follow into your command line:

.. code-block:: bash

    python -V

You should see a reply like:

.. code-block:: bash

    Python 2.7.5


---------------------
pip package manager
---------------------

The `pip package manager <http://www.pip-installer.org/en/latest/index.html>`_
is needed to install Tarbell, our publishing tool. 

You'll probably need to install pip on your system.

On Mac OS X, run this command on your command line:

.. code-block:: bash

    sudo easy_install pip

To verify that you have pip installed, run:

.. code-block:: bash

    pip -V


---------------------
Git and Github
---------------------

`Git <http://git-scm.com/>`_ is a version control program for logging the changes 
you make to files over time. This is useful when you're working on your own, 
but quickly becomes essential when working with others.

You will use Git 

`GitHub <https://github.com/>`_ is a website that hosts git code repositories, both public and private. It comes
with many helpful tools for reviewing code and managing projects. It also has some 
`extra tricks <http://pages.github.com/>`_ that make it easy to publish web pages, which we will use later. 

GitHub offers helpful guides for installing Git in 
`Mac OS X <https://help.github.com/articles/set-up-git#platform-mac>`_ and
`Linux <https://help.github.com/articles/set-up-git#platform-linux>`_. You can verify
it's installed from your command line like so:

.. code-block:: bash

    # You don't have to type the "$" It's just a generic symbol 
    # geeks use to show they're working on the command line.
    $ git --version

Once that's done, you should create an account at GitHub, if you don't already have one.
It shouldn't cost you anything. `The free plan <https://github.com/pricing>`_ 
is all that's required to complete this lesson.

--------------------------------------
Google account and client secrets file
--------------------------------------

You'll need a Google account to manage the data and content on your site
with Google spreadsheets. If you have a gmail address, you already have a Google
account.

You'll need to follow `this guide to downloading a client_secrets.json file <http://tarbell.readthedocs.org/en/latest/install.html#configure-google-spreadsheet-access-optional>`
to your computer. This file acts like a password that allows Tarbell to communicate with Google spreadsheets.

---------------
Install Tarbell
---------------

Time to install Tarbell!

.. code-block:: bash

    sudo pip install tarbell==0.9b4

Time to configure Tarbell:

.. code-block:: bash

    tarbell configure

Follow the default prompts. You'll need to provide the location of your client secrets file
and visit a website to validate your access. It's a pain, but you only have to do it once.

For now, you should specify "no" / "n" when prompted to configure Amazon S3.


