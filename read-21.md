# *Django Tutorial : Using models*

***Overview***

 - *Prerequisites: ->  	Django Tutorial Part 2: Creating a skeleton website.* 
 - *Objective:	   ->   To be able to design and create your own models, choosing fields appropriately.*

> *Django web applications access and manage data through Python objects referred to as models. Models define the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms, etc. The definition of the model is independent of the underlying database — you can choose one of several as part of your project settings.*

***Designing the LocalLibrary models***

*We know that we need to store information about books (title, summary, author, written language, category, ISBN) and that we might have multiple copies available (with globally unique id, availability status, etc.).*
*You might also want to use models to represent selection-list options*

*Once we've decided on our models and field, we need to think about the relationships. Django allows you to define relationships that are one to one `(OneToOneField)`, one to many `(ForeignKey)` and many to many `(ManyToManyField)`*

![NO PICTUREEEE ](https://cdn-images.visual-paradigm.com/guide/uml/uml-class-diagram-tutorial/11-associations-with-different-multiplicies.png)

> *The diagram also shows the relationships between the models, including their multiplicities. The multiplicities are the numbers on the diagram showing the numbers (maximum and minimum) of each model that may be present in the relationship.*

***Model primer***
*This section provides a brief overview of how a model is defined and some of the more important fields and field arguments.*
*Models are usually defined in an application's `models.py` file. They are implemented as subclasses of `django.db.models.Model`, and can include fields, methods and metadata.*

***Fields***
*A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables. Each database record (row) will consist of one of each field value.*

<hr>

# *Django Tutorial : Django admin site*


- *Prerequisites: ->	First complete: Django Tutorial Part 3: Using models.*
- *Objective: ->	To understand the benefits and limitations of the Django admin site, and use it to create some records for our models.*

> *The Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records. This can save you a lot of time during development, making it very easy to test your models and get a feel for whether you have the right data.*


> *All the configuration required to include the admin application in your website was done automatically when you created the skeleton project (for information about actual dependencies needed, see the Django docs here). As a result, all you must do to add your models to the admin application is to register them. At the end of this article we'll provide a brief demonstration of how you might further configure the admin area to better display our model data.*





