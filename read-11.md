
# *JupyterLab is the data science UI we have been looking for*

*The Project Jupyter (formally known as IPython) is a polyglot, web-based, open-source data science tool. Fostering reuse and reproducibility, it supports interactive data science and scientific computing across multiple programming languages (the so-called kernels) via the idea of notebooks.
The language-agnostic behavior of Jupyter has made it a possible game-changer, as it unites multiple open source communities around the same tool. It now has a large community and is growing insanely fast, resulting in numerous extensions popping up at Github — including a kernel for SAS maintained by SAS itself, a kernel for SPARQL querying, multiple widgets, and much more.*

# *NumPy Tutorial: Data Analysis with Python*

* ***What is NumPy?***
- NumPy is a Python library used for working with arrays.
- It also has functions for working in domain of linear algebra, fourier transform, and matrices.
- NumPy was created in 2005 by Travis Oliphant. It is an open source project and you can use it freely.
- NumPy stands for Numerical Python.

* *Import NumPy*
> Once NumPy is installed, import it in your applications by adding the import keyword:

`import numpy`

* *Checking NumPy Version*
> The version string is stored under __version__ attribute.

```
import numpy as np

print(np.__version__)
```

* *Create a NumPy ndarray Object*

> - *NumPy is used to work with arrays. The array object in NumPy is called ndarray.*
> - *We can create a NumPy ndarray object by using the array() function.*

```
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)

print(type(arr))
```


* *NumPy Array Indexing*

> - Access Array Elements
> - Array indexing is the same as accessing an array element.
> - You can access an array element by referring to its index number.
> - The indexes in NumPy arrays start with 0, meaning that the first element has index 0, and the second has index 1 etc.


*Data Types in NumPy*
*NumPy has some extra data types, and refer to data types with one character, like i for integers, u for unsigned integers etc.*

> *Below is a list of all data types in NumPy and the characters used to represent them.*

`i` - integer <br>
`b` - boolean <br> 
`u` - unsigned integer <br> 
`f` - float <br> 
`c` - complex float <br>
`m` - timedelta <br> 
`M` - datetime <br> 
`O` - object <br> 
`S` - string <br>
`U` - unicode string <br> 
`V` - fixed chunk of memory for other type ( void ) 
