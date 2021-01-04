# *Django Tutorial: Working with forms*

> - *Prerequisites:	Complete all previous tutorial topics, including Django Tutorial Part 8: User authentication and permissions.*

> - *Objective:	To understand how to write forms to get information from users and update the database. To understand how the generic class-based editing views can vastly simplify creating forms for working with a single model.*

<hr>

***Overview***

*An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server. Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data, including text boxes, checkboxes, radio buttons, date pickers and so on.*

<hr>

***HTML Forms***

*While here we just have one text field for entering the team name, a form may have any number of other input elements and their associated labels. The field's type attribute defines what sort of widget will be displayed. The name and id of the field are used to identify the field in JavaScript/CSS/HTML, while value defines the initial value for the field when it is first displayed. The matching team label is specified using the label tag (see "Enter name" above), with a for field containing the id value of the associated input.*

***Django form handling process***

* *The main things that Django's form handling does are:*

   - Display the default form the first time it is requested by the user.
   - Receive data from a submit request and bind it to the form.
   - Clean and validate the data.
   - If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem fields.
   - If all data is valid, perform required actions (e.g. save the data, send an email, return the result of a search, upload a file, etc.)
   - Once all actions are complete, redirect the user to another page.
  

