# ITEC-3280-Web-Programming-Assignment-11-solution

Download Here: [ITEC 3280– Web Programming Assignment 11 solution](https://jarviscodinghub.com/assignment/php-form-processing-and-mysql-database-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Part I – product_order.php
Create a form page called product_order.php that contains the following form controls:
Product (drop down list) product – iPad, iPhone 6S, Galaxy 5S, Moto X, and so on
Quantity (number) quantity
Unit Price (number) unit_price
Discount Rate (%)(number) discount_rate
Order Date (date) order_date
First Name (text box) first_name
Last Name (text box) last_name
Payment Type (drop down list) payment_type – Visa, Master, Discover, Amex, and so on
Card Number (text box) card_number
Security Code (text box) security_code

When the submit button is clicked, the form data is posted to order_process.php.

Part II– Create MySQL Database and Table
Using MySql, create a database called “ordersdb” and then create a table called “orders” with the following fields:
id (INT, Primary Key, Auto Number)
product (VARCHAR, 100)
quantity (INT)
unit_price (DECIMAL)
discount_rate (DECIMAL)
order_date (DATE)
first_name (VARCHAR, 50)
last_name (VARCHAR, 50)
payment_type (VARCHAR, 15)
card_number (VARCHAR, 20)
security_code (VARCHAR, 10)

Create a pair of user name and password (e.g, user1 and pass1) by using the following settings.
– Username: user1
– Password: pass1
– Host: Local
– Check all privileges under Data and Structure sections
Then edit user1’s privileges to grant all privileges of the “ordersdb” so that the user1 can access to the database.
Once the sales table is created, export the “ordersdb” using SQL format and submit with other files.
Part III – Create Connection File
Create a new PHP file named “connection.php”. This file will contain the connection string to connect to the “ordersdb”.

Part IV– order_process.php
Create and use a SQL INSERT statement to add the user loan input data into the orders table created in Part II.
To execute the insert statement, use mysqli_query function as follows.
//Execute SQL Statement and store results as a recordset
$rs = mysqli_query($con, $sqlstring);

As you have done in assignment 10, the page should also include a header and footer file. Use the PHP include() or require() function. The header file (header.php) contains the page heading (use an h2 tag) – “ABC Loan Company”. The footer file (footer.php) contains the page footing – copyright 2014 and your email address.

Also, use the PHP include() or require() function to include the connection.php.
Next, add the code to insert the user input into the “orders” table. (Be sure to use scalar variables within the SQL INSERT statement). After the INSERT statement is executed, close the connection to the database.
Finally, display the output:
PRODUCT ORDER
Name: firstnamevariable + lastnamevariable

Product: productvariable
Unit Price: unitpricevariable
Discount Rate: discountratevariable
Order Total: ordertotalvariable
Order Date: orderdatevariable
Payment Information:
paymenttypevariable + creditcardnumbervariable (= 12 stars (*) + last 4 digit numbers )
Today’s Date is: PHP Date
