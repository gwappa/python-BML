Intro: the terminal emulator
=============================

Before starting to program: you probably cannot avoid using your **terminal emulator**.
It may sound awful, but it can in reality simplify your life as a programmer in many ways.

Just don't worry, and let's start familiarizing yourself!

What is the terminal emulator?
-------------------------------

A terminal emulator, or just a "terminal" in short, is a character-based environment to interact with your computer.

Terminal? Shell?
^^^^^^^^^^^^^^^^^

The terminal-emulator application is sometimes also referred to as a **shell**.
Despite a slight difference in their meanings, the two words -- "shell" and "terminal" --  are interchangeable to each other in many cases.
For example, "type ... into your terminal" and "type ... into your shell" are both intended for the same action.

The term "shell" is contrasted to the term **kernel**, which refers to the core functionality of the operating system, i.e. Windows, Linux, or Darwin (the core of Mac OS).

Conceptually, shell is "something that wraps around the kernel"; whereas the kernel *is* the program that makes a computer work as a computer, the shell refers to the program that receives a set of commands to let the user touch the kernel functionality.

To be precise, there is a slight difference in what a "shell" means and what a "terminal" means (and sometimes this difference matters in fact):

+ The "terminal" refers to the character-based environment where you can talk to your operating system directly (see the `historical background <history>`_ section for more details).
+ The "shell" refers to the program that runs in the terminal.

The reality is that there are several different types of "shell programs" that can run in the terminal: TC shell (``tsch``), Bourne-again shell (``bash``), and the Command Prompt on Windows (``cmd.exe``), to name a few. each of which having a *slightly* different flavor in its set of commands when interacting with the operating system. Although they look and work in quite the same way in most cases, you still need to watch out a certain shell-specific behaviors (which I try to be explicit)...

Where are they?
^^^^^^^^^^^^^^^^

Windows 10
~~~~~~~~~~~

I would recommend using the **Command Prompt** application (since it is used for Anaconda Prompt, too). It is installed on any Windows 10 computer.

* Right-click on the Start menu.
* Find the menu item "Command Prompt (C)", and select it.

It is also possible to find it from the Search bar at the bottom. Type ``cmd``, and it will show the Command Prompt app for you.

.. note::

	When you open it, you will find that the icon of the Command Prompt app shows up on the task bar. You can right-click on it, and select "Pin to taskbar" so that you don't have to look for the app again next time.

Beware of the fact that, by default, a prompt will open at your home directory.

Mac
~~~~

The **Terminal** application is installed by default.

* Open Spotlight (click on the magnifying-glass icon, or type Cmd+Space on Finder).
* Type ``terminal``. Spotlight will then suggest ``Terminal.app``, so hit the enter/return key.

.. note::

	When you open it, the icon of the Terminal app will show up in the Dock. You can keep the icon even after closing the app by dragging the icon to another place in the Dock so that you don't have to look for it again next time.

Linux
~~~~~~

The **terminal emulator** is installed by default, but the way to open it depends on the distribution you use. Please Google it...

.. _history:

A historical background of "terminals"
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In the ancient ages, people did not use to have their own "personal" computers.
They instead used to connect to the "main-frame" computer, which they shared with everyone else, using a device called "terminal".

A typical terminal consisted of a keyboard and a monitor. In most cases, they did not have any graphical user interface (e.g. desktops, icons etc.), so they communicate with the main frame only by typing *commands* to the terminal.
The terminal sends it to the main frame, which in turn sends the response back to the terminal that displays it in its monitor.

As you can imagine, it was a non-trivial duty for all novice users to learn the commands to communicate with the main frame, but that was the way how the "real programmers" grew up in those days.

As we all know, the age of real programmers is gone. We have graphical user interfaces, with lots of user-friendly functionalities, that makes it easier to familiarize ourselves and interact with our computers. Instead of us learning how to talk to it, the computer now has a persona that has interfaces intuitive for us.

On the other hand, the nice old character-based interface has not cease to exist (yet). Since they are not literally "terminals" anymore, so they are instead called "terminal *emulators*".

But why bother? Because the character-based (command-based) interfaces still outperforms graphical user interfaces in a certain aspect of computing: automation. When it comes to telling a computer how to perform a sequence of tasks on a set of files in a batch, writing a list of commands remains to be one of the most simple and secure approaches.

As an example, you can think of copying a piece of text from Microsoft Excel and pasting it into TextEdit again and again. For us human beings, it is just about repeating of the same procedure. But how can you tell the computer about what to do? It would be a bit difficult to tell it *graphically*, and you would have to resort to using a certain *language*. This is where the terminals have their advantages.


Basic commands
---------------

There are in fact *hundreds* of "basic commands" -- so large in variety
that you can do most of your routine works on the terminal!

But it is not realistic to learn everything from the beginning
(and we are going to learn Python anyway, which is easier to learn
step by step).
So here I list a couple of commands that are essential when
managing files from the terminal.

``cd``
^^^^^^^

``ls``
^^^^^^^

``mkdir``
^^^^^^^^^^

``mv``
^^^^^^

``cp``
^^^^^^

``rm``
^^^^^^

Special paths
--------------

``.``
^^^^^^

``..``
^^^^^^

How to open files in GUI from the terminal?
--------------------------------------------

Especially when editing files or just to take a look at files, it is sometimes preferrable to open the directory (or a file) from the GUI.

In such cases, you don't have to navigate the file browser yourself.
Your terminal provides you with a command to *open a file from the GUI*:

+ **Windows**: ``start <file>``
+ **Mac**: ``open <file>``
+ **Linux**: I guess ``xdg-open <file>`` should work in many distributions.
