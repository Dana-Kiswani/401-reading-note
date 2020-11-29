# *Big O Notation*

*Anyone who's read Programming Pearls or any other Computer Science books and doesn’t have a grounding in Mathematics will have hit a wall when they reached chapters that mention O(N log N) or other seemingly crazy syntax.*
*Hopefully this article will help you gain an understanding of the basics of Big O and Logarithms.
For example, if an algorithm increments each number in a list of length n, we might say: “This algorithm runs in O(n) time and performs O(1) work for each element”.*

*So, below are some common orders of growth along with descriptions and examples where possible.*

- *O(1)*
> *O(1) describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.*

- *O(N)*
> *O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set.*

- *O(N2)*
> *O(N2) represents an algorithm whose performance is directly proportional to the square of the size of the input data set.*

- *O(2N)*
> *O(2N) denotes an algorithm whose growth doubles with each additon to the input data set.*

<hr>

# *Names and Values in Python*
*The behavior of names and values in Python can be confusing. Like many parts of Python, it has an underlying simplicity that can be hard to discern, especially if you are used to other programming languages.*
*Assigning a value to a name never copies the data, it never makes a new value. Assignment just makes the name on the left refer to the value on the right.*
*Python is dynamically typed, which means that names have no type. Any name can refer to any value at any time. A name can refer to an integer, and then to a string, and then to a function, and then to a module.*


