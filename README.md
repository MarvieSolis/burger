# Eat-the-Burger

## Functionality
*Eat-the-Burger* is a playful web application that lets users add new burgers onto the orders and/or devour previously made burgers. Burgers are added by typing in their name in the input field at the bottom of the page followed by clicking the "Add the Burger!" button. To devour a burger, just press the "EAT IT!" buttons located to the right of each respective burger. After devouring a burger, that respective burger will now be listed on the right.

## Usefulness
This program utilizes **jQuery**, **node**, **MySQL**, **handlebars** and **express** to create and access a database, run a server, and link HTML and CSS files. This enables the program to utilize it's internal database of burgers and have it updated in realtime until the database and/or table is dropped. The database is formed by running the `schema.sql` and `seeds.sql` files in MySQL. `connection.js` then uses `server.js` to connect to that database. Once the connection is established, `burger_controller.js` uses express to access different routes to perform the GETs and POSTs needed for the application. These routes then call the various functions in the `orm.js` file. These functions are "selectAll", "insertOne", and "updateOne". SelectAll returns all the data from the database and displays the eaten and the ready-to-be-eaten burgers. InsertOne adds a new burger to the database when the user enters in a new burger. Lastly, updateOne is called when a user "eats" a burger, changing the burger's status.


## Getting started
People can learn more about the different tools and languages used by clicking the following links: [jQuery.com](https://www.jquery.com/) - [w3schools](https://www.w3schools.com/jquery/default.asp) - [express](https://www.npmjs.com/package/express) - [MySQL](https://www.mysql.com/).


## The Site is live!
[Click here to see the page on Heroku!](https://marvie-c-solis-eat-the-burger.herokuapp.com/)