
# BudgetManager

This is a simple web application to track daily incomes and expenses, where user can sign up, sign in, add, remove or edit the income or expense details.





## Features

- sign up, sign in
- email verification, forgot password
- responsive web design
- pagination
- secured REST end points
- jwt token based authentication
- CRUD operations


## Built With


- Spring Boot 2.3.0
- MySQL


## Prerequisites

* Maven
* MySQL Workbench ([click here for download](https://dev.mysql.com/downloads/workbench/))

## Open and Run Project

**For Database:**
1. open MySQL Workbench.
2. create a new database named as "db_budget_manager".

**For Spring Boot application:**
1. open application.properties and replace all "TODO" with your configuration.
2. run command "mvn install".
3. run command "mvn spring-boot:run".


## RESTful API ##

> **Secure Route**: /api/items/**

**1. API Description for User related action**
<br />
base = /api

METHOD | PATH | DESCRIPTION
------------|-----|------------
POST | /register | new user registration
POST | /login | user login
GET | /email-verification | verifying email address
POST | /request-password-reset | sending password reset link to registered email
POST | /password-reset | reset the password

**2. API Description for Item(Income or Expense)**
<br />
base = /api/items

METHOD | PATH | DESCRIPTION
------------|-----|------------
GET | / | get all items
POST | /{category} | create new item
PUT | /{category}/{id} | update item
DELETE | /{category}/{id} | delete item

{category} = income OR expense


### Thanks

I'm always happy to hear your feedback! 😊
 
