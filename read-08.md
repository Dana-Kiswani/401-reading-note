
# *List Comprehensions*

***`List comprehensions` provide a concise way to create lists.***
*It consists of brackets containing an expression followed by a for clause, then zero or more for or if clauses. The expressions can be anything, meaning you can put in all kinds of objects in lists.*

*List comprehension is an elegant way to define and create lists based on existing lists. Rather than creating an empty list and adding each element to the end, you simply define the list and its contents at the same time by following this format:*

`new_list = [expression for member in iterable]`


***Using Conditional Logic***

*A more complete description of the comprehension formula adds support for optional conditionals. The most common way to add conditional logic to a list comprehension is to add a conditional to the end of the expression:*

`new_list = [expression for member in iterable (if conditional)]`

***Debugging With PySnooper***

*Debugging is a painful but necessary practice in software development. The tools that are available in Python range from the built-in debugger, to tools integrated with your coding environment, to the trusty print function. In this episode Ram Rachum describes his work on PySnooper and how it can be used to speed up your problem solving in complex or legacy applications.*
