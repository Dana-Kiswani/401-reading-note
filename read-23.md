# *Django Best Practices: Custom User Model*

***Setup***
*To start, create a new Django project from the command line. We need to do several things:*

  - create and navigate into a dedicated directory called `accounts` for our code
  - *install `Django`*
  - *make a `new Django` project called config*
  - *make a new app `accounts`*
  - *start the local web server*
  
***AbstractUser vs AbstractBaseUser***

*There are two modern ways to create a custom user model in Django: `AbstractUser` and `AbstractBaseUser`. In both cases we can subclass them to extend existing functionality however `AbstractBaseUser` requires* ***much, much more work.*** *Seriously, don't mess with it unless you really know what you're doing.*
  
 ***Conclusion***
Now that our custom user model is configured you can easily and at any time add additional fields to it. 
  
  
 # *Substituting a custom User model*
 
*Django allows you to override the default user model by providing a value for the ***AUTH_USER_MODEL*** setting that references a custom model:*

`AUTH_USER_MODEL = 'myapp.MyUser'`

> *This dotted pair describes the name of the Django app (which must be in your `INSTALLED_APPS`), and the name of the Django model that you wish to use as your user model.*


# *Changing to a custom user model mid-project*

*Changing* ***AUTH_USER_MODEL*** *after you’ve created database tables is significantly more difficult since it affects foreign keys and many-to-many relationships.*

*This change can’t be done automatically and requires manually fixing your schema, moving your data from the old user table, and possibly manually reapplying some migrations.*

> *In addition, you may run into a CircularDependencyError when running your migrations as Django won’t be able to automatically break the dependency loop due to the dynamic dependency. If you see this error, you should break the loop by moving the models depended on by your user model into a second migration. (You can try making two normal models that have a ForeignKey to each other and seeing how makemigrations resolves that circular dependency if you want to see how it’s usually done.)*




