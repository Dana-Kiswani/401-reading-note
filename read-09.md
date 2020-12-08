
***Dunder Methods***

*Dunder or magic methods in Python are the methods having two prefix and suffix underscores in the method name. Dunder here means “Double Under (Underscores)”. These are commonly used for operator overloading. Few examples for magic methods are: __init__, __add__, __len__, __repr__ etc.*

- ***So what's magic about the __init__ method?*** The answer is, you don't have to invoke it directly. The invocation is realized behind the scenes. When you create an instance x of a class A with the statement "x = A()", Python will do the necessary calls to __new__ and __init__.The __init__ method for initialization is invoked without any call, when an instance of a class is created, like constructors in certain other programming languages such as C++, Java, C#, PHP etc. These methods are the reason we can add two strings with ‘+’ operator without any explicit typecasting.*

> Here’s a simple implementation :

``` ruby 
# magic method to initiate object 
    def __init__(self, string): 
        self.string = string 
```

- *We will demonstrate the Length class and how you can overload the "+" operator for your own class. To do this, we have to overload the __add__ method. Our class contains the __str__ and __repr__ methods as well. The instances of the class Length contain length or distance information. The attributes of an instance are self.value and self.unit.,The above snippet of code prints only the memory address of the string object. Let’s add a __repr__ method to provide a string representation of your object for the consumer of your class .*

``` ruby
 # print our string object 
    def __repr__(self): 
        return 'Object: {}'.format(self.string)
```

- ***The call method*** *Before we will come to the __call__ method, we have to know what a callable is. In general, a "callable" is an object that can be called like a function and behaves like one. All functions are also callables. Python provides a function with the name callable.*

``` ruby
 def __call__(self):
        return "spam"
```

***Probability and Statistics*** *are the foundational pillars of Data Science. In fact, the underlying principle of machine learning and artificial intelligence is nothing but statistical mathematics and linear algebra. Often developers will encounter situations, especially in Data Science, where they have to read some research paper which involves a lot of maths in order to understand a particular topic.

> *In Python ,,, You can visualize uniform distribution in python with the help of a random number generator acting over an interval of numbers (a,b). You need to import the uniform function from scipy.stats module.*

> *In Python ,,, You can generate a normally distributed random variable using scipy.stats module's norm.rvs() method. The loc argument corresponds to the mean of the distribution. scale corresponds to standard deviation and size to the number of random variates. If you want to maintain reproducibility, include a random_state argument assigned to a number.*


