# *Django REST Framework & Docker*

***A Beginner's Guide to Docker***

*This is a beginner’s guide to Docker which is a way to isolate and run entire applications. With Docker it doesn’t matter if you are using a Mac, Windows, or Linux computer anymore. The entire development environment is isolated: programming language, software packages, databases, and more.*

*With Docker we now longer have to mess around with virtual environments. We can faithfully reproduce a production environment locally. And Docker can be shared among team members so everyone is working on the same setup. Wins all around.*

***Install Docker***

*Once Docker is done installing we can confirm the correct version is running. It should be at least version 19.*

``` ruby
$ docker --version
Docker version 19.03.5, build 633a0ea
```

*Docker Compose is an additional tool that is automatically included with Mac and Windows downloads of Docker. However if you are on Linux, you will need to add it manually. You can do this by running the command `sudo pip install docker-compose` after your Docker installation is complete.*


``` ruby
$ docker-compose --version
docker-compose version 1.24.1, build 4667896b
```

***Library Website and API***

*Django REST Framework works alongside the Django web framework to create web APIs. We cannot build a web API with only Django Rest Framework; it always must be added to a project after Django itself has been installed and configured.*

*In this chapter we will review the similarities and differences between traditional Django and Django REST Framework. The most important takeaway is that Django creates websites containing webpages, while Django REST Framework creates web APIs which are a collection of URL endpoints containing available HTTP verbs that return JSON.*

*To illustrate these concepts, we will build out a basic Library website with traditional Django and then extend it into a web API with Django REST Framework.*

*Traditional Django*

*First we need a dedicated directory on our computer to store the code. This can live anywhere but for convenience, if you are on a Mac, we can place it in the Desktop folder. The location really does not matter; it just needs to be easily accessible.*

``` ruby
$ cd ~/Desktop
$ mkdir code && cd code
```

