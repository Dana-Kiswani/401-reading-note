***Classes and Objects***

*Python is an object oriented programming language. Unlike procedure oriented programming, where the main emphasis is on functions, object oriented programming stresses on objects.*
*An object is simply a collection of data (variables) and methods (functions) that act on those data.*

***Creating Classes***
> *The class statement creates a new class definition. The name of the class immediately follows the keyword class followed by a colon as follows:*

``` ruby
 class ClassName:
    variable = 'blah'

    def function(self):
        print("This is a message inside the class.") 
```

> `myobjectx = MyClass()`

<hr>

***Recursive Functions in Python***

*Recursion is a common mathematical and programming concept. It means that a function calls itself. This has the benefit of meaning that you can loop through data to reach a result.*
*This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.*
*Now that we have some intuition about recursion, let’s introduce the formal definition of a recursive function. A recursive function is a function defined in terms of itself via self-referential expressions.*

<hr>

***Python Testing with pytest: Fixtures and Coverage***

*Pytest is a robust Python testing tool, pytest can be used for all types and levels of software testing. pytest can be used by development teams, QA teams, independent testing groups, individuals practicing TDD, and open source projects. In fact, projects all over the Internet have switched from unittest or nose to pytest, including Mozilla and Dropbox.*

<hr>

***Fixtures***
*If your tests need to work on data you typically need to set them up. This is often a process that has to be repeated and independent for each test. This often leads to duplicate code.*

<hr>

***Maintaining State***
*When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:*

*Thread the state through each recursive call so that the current state is part of the current call’s execution context Keep the state in global scope A demonstration should make things clearer.*
