# *Reading and Writing Files in Python*

*In Python, there is no need for importing external library to read and write files. Python provides an inbuilt function for creating, writing, and reading files.*

***What Is a File?***
*Before we can go into how to work with files in Python, it’s important to understand what exactly a file is and how modern operating systems handle some of their aspects.*

***How to Open a Text File***
*To open a file, you need to use the built-in open function. The open function returns a file object that contains methods and attributes to perform various operations on the file.*

> *Syntax: `file_object = open("filename", "mode")`*

***The most commonly used options for modes are the following:***

- *'r' Open for reading (default)*

- *'w' Open for writing, truncating (overwriting) the file first*

- *'rb' or 'wb' Open in binary mode (read/write using byte data)*

***There are three different categories of file objects:***

- *Text files*
- *Buffered binary files*
- *Raw binary files*

***How to Read a File***
*You can read a file in Python by calling .txt file in a "read mode"(r).*

- ***Step 1)*** Open the file in Read mode: f=open("filename.txt", "r")
- ***Step 2)*** We use the mode function in the code to check that the file is in open mode. If yes, we proceed ahead if f.mode == 'r':
- ***Step 3)*** Use f.read to read file data and store it in variable content contents =f.read()
- ***Step 4)*** print contents.

***Exceptions in Python***
> *What is Exception?*
*An exception is an event, which occurs during the execution of a program that disrupts the normal flow of the program's instructions. In general, when a Python script encounters a situation that it cannot cope with, it raises an exception. An exception is a Python object that represents an error.*

*When a Python script raises an exception, it must either handle the exception immediately otherwise it terminates and quits.*

***Raising an Exceptions***
*You can raise exceptions in several ways by using the raise statement. The general syntax for the raise statement is as follows.*
