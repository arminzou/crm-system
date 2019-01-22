# CRM-System
A CRM (Customer Relationship Management System) Web Application created using Spring MVC and Hibernate. This Web application is a mini version which has the following features:
- Login for employees (user) of the Company
- Add and Update new Customer Info
- Search customer 
- Delete Customer from database
- Register new users

The Application is created using following Technologies 
- Java - Programming Language
- Spring MVC - For User Interface
- Spring Security - Secure user account and restrict access base on role
- Hibernate - JDBC (Java Database Connectivity)
- MySQL - Database
- Tomcat - Localhost Server
---

# Setup
The Project can be setup locally with the following steps:
- Use `git clone` to clone this repo to your local machine:
```
$ git clone https://github.com/amz27/CRM-System.git
```
- Create a Database
	- Run the two scripts of `sql-scripts` to set up database 

- Run the project on Tomcat Server 

## Home page
A simple login button on the top-right that redirect to login page

![home](https://user-images.githubusercontent.com/39773496/51560291-2b0dff80-1e52-11e9-8bad-76b123e32947.JPG)

## Registration page
User can register new account 

![sign-up](https://user-images.githubusercontent.com/39773496/51560602-f189c400-1e52-11e9-934f-422cf8a74a55.JPG)

## Add Customer page
Add new Customer in the database

![add-customer](https://user-images.githubusercontent.com/39773496/51560607-f2baf100-1e52-11e9-9777-fc0212c2bbcf.JPG)

## Update Customer page
Update Customer page is similar to *Add Customer page* above, except the text fields are auto populated with customer information

---
# Spring Security
	• Secure the CRM Web App
	• Secure a custom login page
	• Define users and roles authentication 
	• Protect URLs based on role
	• Use JSP tags to hide/show content based on role
	• Store users, passwords and roles in DB (bcrypt -> encrypted)
  
## Login page
Customized login page that authenticate a user

> ![login](https://user-images.githubusercontent.com/39773496/51560349-4b3dbe80-1e52-11e9-8026-da5420d9ee0b.JPG)


## Customer list views
### Employee view
Spring Security hide content/restrict access from employee
	- Employees are not allowed to perform add, update and delete operations

> ![employee-view](https://user-images.githubusercontent.com/39773496/51560538-be473500-1e52-11e9-96a6-be6095cd7c5b.JPG)


### Manager view
Spring Security hide content/restrict access from Manager
	- Managers are not allowed to perform delete operation

> ![manager-view](https://user-images.githubusercontent.com/39773496/51560546-c2735280-1e52-11e9-873d-712839fc7090.JPG)

### Administrator view
Admin can access all operations

> ![admin-view](https://user-images.githubusercontent.com/39773496/51560553-c43d1600-1e52-11e9-9e99-95ce2c9147cf.JPG)



## MySQL Database
- Customer table
![customer-table](https://user-images.githubusercontent.com/39773496/51560769-7c6abe80-1e53-11e9-9d5b-6bf8928c8cb5.JPG)
- User table
![user-table](https://user-images.githubusercontent.com/39773496/51560836-a91ed600-1e53-11e9-8eba-1b9d2338bec5.JPG)
- Role table
![role-table](https://user-images.githubusercontent.com/39773496/51560837-a9b76c80-1e53-11e9-983b-53b1735fe196.JPG)

> Note: The passwords are encrypted using bcrypted password. Simply use `fun123` as password for testing purpose. 

## Demo:
![crm-demo](https://user-images.githubusercontent.com/39773496/51571544-6a4b4900-1e70-11e9-91cd-56857b6f303c.gif)
