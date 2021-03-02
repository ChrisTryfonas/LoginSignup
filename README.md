### Basics
In this repo I built a basic login/signup system that can be integrated to any website such as eshop, blog, social media etc.
The system is hosted at my laptop which is set as a local server, using WAMP software. Also I used phpMyAdmin to interract with MySQL, which is my RDBMS.  
For this project I created a database called "mydatabase" which contains a table called "users" with all the names and the passwords of the enrolled users.

Tools: html, css, php, mySQL, phpMyAdmin, WAMP local server.

### Login 
1.	The user enters ‘username’ and ‘password’ at index.php form - both required.
2.	An SQL query is executed to check if **both** of these credentials exist in my database’s table.
  i)	If yes, it means that the user has already signed up and is redirected to another page (SuccessLogin.php) that shows a message, something like “Welcome username…”.

  ii)	If not, then - at least at this beginner stage - the user is redirected to the index.php and at the url is encorporated the message “UserNOTFound”.

*The code that executes the query and checks if username και password exists at the table is in file: “includes/validation.php”.

### Signup
1.	The user enters ‘username’ and ‘password’ at index.php form- both required.
2.	Check if the username already exists in the table.
  A)	If yes, it means that this username is already taken the user must type a new one. In that case - at least at this beginner stage- the user is redirected to the index.php and at the url is encorporated the message “This_user_already_exists”.

  B)	If not, then the username is available, the insert query is executed and the user is redirected to a new page (file: “SuccessSignup”). At this page there is a button that redirects user to the homepage (index.php) in order to login after registration.



*The code that executes the query and inserts new user at the table is in file: “registration.php

### Notes 
•	“goback.php” is used to redirect the user from the SuccessSignup.php to Index.php after successful signup and if the return button is clicked.
•	“connection.php” is used to establish the connection between php and mysql database.
•	“registration.php” and “validation.php” are used for inserting a new user and checking if a user already exists respectively.
•	“style.css” is used to style not only index.php but also the registration.php and validation.php.

