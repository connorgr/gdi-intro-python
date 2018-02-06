![Girl Develop It Logo](../images/gdi_logo_badge.png)

###Intro to Python
####Section 1
@@@

## Welcome!
<!-- ## Welcome to <br> Girl Develop It -->
<!-- Affordable and accessible programs to learn software through mentorship and hands-on instruction. -->
@@@

<!-- ## Some rules -->

<p class="popText">We are here for <span class="underline">you</span> – Please give feedback!</p>

<p class="popText">*Every* question is important</p>

<p class="popText">Help each other</p>

<p class="popText">Have fun</p>
@@@

## Code of Conduct
We expect all attendees to show respect and courtesy to other attendees throughout GDI classes and events.

<hr />

GDI is dedicated to providing a harassment-free community and learning experience for everyone.

<hr />

If you are being harassed, notice that someone else is being harassed, or have any other concerns, please contact your local Chapter Leader(s) immediately. Contact information for your local Chapter Leader can be found on <a href="https://www.girldevelopit.com/chapters">our Chapters page</a>.

<hr />

Full: https://www.girldevelopit.com/code-of-conduct
@@@

###What we will cover today

* What is programming?
* Why Python?
* Variables and arithmetic
* Statements and Error Messages
* Development Environment Setup
@@@

###Python 2.7 vs Python 3

@@@

###What is programming?</h3>
@@@

##### Programming is teaching the computer to do a task.

“Program”: made of one or more files of code, each of which solve part of a task
<hr />
The Python code we will write is translated into a format the computer can understand through the Python <a href="http://en.wikipedia.org/wiki/Interpreter_(computing)">Interpreter</a>
<hr />
Before diving into what the interpreter does, let's focus on how to give it instructions in Python
@@@

##### Program: Terminal

<figure>
  <img alt="A screenshot of the Apple Terminal application" src="../images/terminal.png" width="50%" style="border-radius: 5px;">
  <figcaption>In Terminal you can issue commands to the operating system through a command line interface (“make a folder named Photos”)</figcaption>
</figure>
@@@

##### Program: Python Shell

<figure>
  <img alt="A screenshot of the Python shell" src="../images/pythonShell.png" width="50%" style="border-radius: 5px;">
  <figcaption>A command line program that runs inside of the terminal, takes Python code as input, interprets it, and prints out any results.</figcaption>
</figure>
@@@

##### Program: Text Editor

<figure>
  <img alt="A screenshot of the Atom text editor" src="../images/atom.png" width="60%" style="border-radius: 5px;">
  <figcaption>A program that opens text files and allows the user to edit and save them.</figcaption>
</figure>
@@@

##### Popular (Free) Text Editors
* <a href="https://atom.io/">Atom</a>
* <a href="https://code.visualstudio.com/">VSCode</a>
* <a href="https://www.sublimetext.com/">Sublime Text</a>
* Command line text editors like Vim or Emacs

@@@

### Why Python?
@@@

##### Python benefits
* Suitable for beginners, yet used by professionals and top software companies
* Readable, intuitive, maintainable code
* Rapid rate of development
* Variety of applications
Note: Block 1 begins - 25 minutes
@@@

###What is Python used for?

* Data Science + Research (pandas, numpy, scipy)
* Machine Learning (tensorflow, scikit-learn)
* Web development (Django, Flask)
* 3D animation and image editing (Maya, Blender)
* Game Development (Civilization 4, EVE Online)
* Multi-purpose Object Oriented programming (much like Java, C++, or Ruby)
* Scripting (much like Bash)
@@@

### Who is using Python?

* Blender
* DeepMind (and most AI/ML companies, thereof)
* Disney
* Dropbox
* Google
* NASA
@@@


###Let's Develop It
Let's setup our computer for Python programming

* Let's install a text editor - [Install Atom](https://atom.io/)
* (Windows only) [Install Python 2.7](http://www.python.org/download/)
* (Windows only): After installing Python, open the "powershell" program and type:
<pre style="width: 100%">[Environment]::SetEnvironmentVariable("Path", "$env:Path;C:\Python27", "User")</pre>
* Locate and run the terminal program. Type 'python' and hit enter.
* More setup instructions are available: [here](http://learnpythonthehardway.org/book/ex0.html)
Note: 15 minutes
@@@

## Block 2
Note: 30 minutes
@@@

###Working in the Python Shell

Open up your terminal and type 'python' <!-- .element class="left-align" -->

* Follow along with the examples in the slides. Type them in! <!-- .element class="fragment" -->
* Feel free to explore as well. You will not accidentally break things <!-- .element class="fragment" -->
* Line with $ means you are in the terminal (not python). <!-- .element class="fragment" -->
* Line with >>> means you are in python <!-- .element class="fragment" -->
* Type exit() to leave python and return to the terminal. <!-- .element class="fragment" -->

@@@

###Variables and Arithmetic
```python
>>> 3 + 4
7
>>> 2 * 4
8
>>> 6 - 2
4
>>> 4 / 2
2
```
```python
>>> a = 2
>>> print a
2
>>> b = 3
>>> c = a + b
>>> print c
5
```
```python
>>> a = 0
>>> a = a + .5
>>> print a
0.5
```
@@@

###Strings
```python
>>> a = 'Hello '
>>> b = 'World'
>>> c = a + b
>>> print c
'Hello World'
```
```python
>>> a = "Spam "
>>> b = a * 4
>>> print b
"Spam Spam Spam Spam "
```
@@@

###Data types
* Variables are names of objects <!-- .element class="fragment" -->
* Among other things, variables are used to represent things that vary or that can't be known until the program is run <!-- .element class="fragment" -->
* Objects always have a "type" <!-- .element class="fragment" -->
* The type of an object helps define what it can do <!-- .element class="fragment" -->
* The type can be found using: type() <!-- .element class="fragment" -->
* type() is a function. We call it by using parenthesis and pass it an object by placing the object inside the parenthesis <!-- .element class="fragment" -->
@@@

#### Data type examples
```python
>>> print type(4)
<type 'int'>
>>> a = 4
>>> print type(a)
<type 'int'>
>>> print type("Winter is here.")
<type 'str'>
>>> print type(3.5)
<type 'float'>
```
@@@

###Data types - continued ...
* Objects can be used with a set of operators <!-- .element class="fragment" -->
* An int or float can be used with any of: +, -, \*, / <!-- .element class="fragment" -->
* A string can be used with + <!-- .element class="fragment" -->
* What happens if we try to use the other operators with a string? <!-- .element class="fragment" -->
```python
>>> print "One string" / "Two string"
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unsupported operand type(s) for /: 'str' and 'str'
```
@@@


###Errors

* There are different kinds of errors that can occur. We've seen a few of these so far <!-- .element class="fragment" -->
* A runtime error results in an Exception. An Exception gives us some information about the nature of the error and how to correct it <!-- .element class="fragment" -->
* One type of exception is a SyntaxError. This results when our code can not be evaluated because it is incorrect at a syntactic level. In other words, we are not following the "rules" of the language. <!-- .element class="fragment" -->
* Some other examples are the TypeError and NameError exceptions. <!-- .element class="fragment" -->
@@@

###Errors - continued ...

* A \# is a code comment. These are not evaluated by Python

```python
# SyntaxError - Doesn't conform to the rules of Python.
# This statement isn't meaningful to the computer
>>> 4sherlock)watson(moriarty) + 10

# NameError - Using a name that hasn't been defined yet.
>>> a = 5
>>> print b

# TypeError - Using an object in a way that its type does not support
>>> 'string1' / 'string2'
```
@@@

###Let's Develop It
* We'll practice what we've learned in the shell
* Review the slides on your computer and practice entering any commands you didn't fully understand before
* Ask the teacher or a TA for any help
Note: Let's develop it: 30 minutes.
@@@

###Using the terminal
Try each of the following commands in turn:

Command         | Short for               | Description
----------------|-------------------------|-------------
pwd             | Print working directory | Displays what folder you are in
ls              | List                    | Displays the files and folders in the current folder
cd <folder>     | Change Directory        | Change to another folder, where <folder> is the target
cat <filename>  | Concatenate k           | Prints the contents of the file
file <filename> | File                    | Displays the type of the file

Note: Block 3 begins, 30 minutes
@@@

###Creating a folder
We need a folder to save and run our code from.

($ shows the shell prompt where commands are entered. Lines without $ are output)
```bash
$ cd
$ pwd
/home/username ( or /User/username or similar)
$ mkdir gdipython
$ cd gdipython
$ pwd
/home/username/gdipython
```
Now that the folders are made, we only have to use this in the future:

`$ cd ~/gdipython`
@@@

###The Text Editor
Atom: Type 'atom .', then File -> New File ('program.py') <!-- .element class="left-align" -->

Other: Open App, open gdipython folder, create file. <!-- .element class="left-align" -->

In the text editor, enter the following: <!-- .element class="left-align" -->

```python
print 'This is a Python program'
```

---
Open a terminal and type
```bash
$ cd ~/gdipython
$ python program.py
```

You should see the terminal print:

`This is a Python program`
@@@

###User Input
To obtain user input, use 'raw_input()'. This will become a string

We use float() to make it a number

Change the program.py text to the following and run it again
```python
input_value = raw_input("Enter a radius:")
radius = float(input_value)
area = 3.14159 * radius * radius
print "The area of a circle with radius", input_value, "is", area
```
@@@

###Let's Develop It
Write your own program that uses raw_input and does something else with the value

You can use float() or int() to treat the input as a number if you need a number, or you can use the input directly if you need a string

Note: Let's develop it: 15 minutes
@@@

###Questions?
