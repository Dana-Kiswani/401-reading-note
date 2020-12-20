# *Web Scrape with Python in 4 minutes*

> *THIS WIBSITE IS NOT RESPONDING*
<hr>

# *What is Web Scraping?*

***Some websites can contain a very large amount of invaluable data. Stock prices, product details, sports stats, company contacts, you name it. If you wanted to access this information, you’d either have to use whatever format the website uses or copy-paste the information manually into a new document. Here’s where web scraping can help.***

***Web scraping*** *is the process of collecting and parsing raw data from the Web, and the Python community has come up with some pretty powerful web scraping tools..*

> *But in most cases, web scraping is not a simple task. Websites come in many shapes and forms, as a result, web scrapers vary in functionality and features.*

***How do Web Scrapers Work?***

> Automated web scrapers work in a rather simple but also complex way. After all, websites are built for humans to understand, not machines.

> * *First, the web scraper will be given one or more URLs to load before scraping. The scraper then loads the entire HTML code for the page in question. More advanced scrapers will render the entire website, including CSS and Javascript elements.*

> * *Then the scraper will either extract all the data on the page or specific data selected by the user before the project is run.*

> * *Ideally, the user will go through the process of selecting the specific data they want from the page. For example, you might want to scrape an Amazon product page for prices and models but are not necessarily interested in product reviews.*

> * *Lastly, the web scraper will output all the data that has been collected into a format that is more useful to the user.*

<hr>

*One useful package for web scraping that you can find in Python’s standard library is urllib, which contains tools for working with URLs. In particular, the urllib.request module contains a function called urlopen() that can be used to open a URL within a program.*

> *In IDLE’s interactive window, type the following to import urlopen():*
` >>> from urllib.request import urlopen`

> *The web page that we’ll open is at the following URL:*

`>>> url = "http://olympus.realpython.org/profiles/aphrodite"`

> *To open the web page, pass url to urlopen():*

`>>> page = urlopen(url)`

<hr>

# *Parsing a page with BeautifulSoup*

*We can use the BeautifulSoup library to parse this document, and extract the text from the p tag. We first have to import the library, and create an instance of the `BeautifulSoup` class to parse our document:*


`from bs4 import BeautifulSoup`
`soup = BeautifulSoup(page.content, 'html.parser')`


*we can move through the structure one level at a time. We can first select all the elements at the top level of the page using the `children` property of `soup`. Note that `children` returns a list generator, so we need to call the list function on it:*

`list(soup.children)`

`['html', 'n', <html> <head> <title>A simple example page</title> </head> <body> <p>Here is some simple content for this page.</p> </body> </html>]`

*The above tells us that there are two tags at the top level of the page — the initial <!DOCTYPE html> tag, and the `<html>` tag. There is a newline character `(n)` in the list as well. Let’s see what the type of each element in the list is:*

`[type(item) for item in list(soup.children)]`

*As you can see, all of the items are BeautifulSoup objects. The first is a Doctype object, which contains information about the type of the document. The second is a NavigableString, which represents text found in the HTML document. The final item is a Tag object, which contains other nested tags. The most important object type, and the one we’ll deal with most often, is the Tag object.*

*The Tag object allows us to navigate through an HTML document, and extract other tags and text. You can learn more about the various BeautifulSoup objects .*

