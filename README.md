# honeyword-security

Honeyword generation is a password breach detection technique. The basic idea is to generate multiple fake passwords based on the original password and store all of them together. These false passwords as well as valid password are stored in the database or a file. The intruder may be able to reach out to the honeyword file successfully, but when reverse hash is  performed on all the passwords on the list, it is difficult to guess the correct password. If brute force attack is implemented   along all the honeywords then, the system will generate an alert to the respective user and admin on use of any of the honeyword. 

#### Software requirements: 
Xampp server 
(Keep all the html,css,php file in windows C:\xampp\htdocs\your_folder)

#### How to execute: ####
* Run Xampp server
* Create Database in sql database of XAMPP server with name "final" and table name "accounts" having fields : id, username,PhNo,email,password,password1,password2,password3,password4
* Go to your_folder in htdocs and go to Register on localhost and Register the account, you will get to see the original password and honeywords generated for understanding purpose. Also one string is with EBCDIC converted line. If you go to database you will see the encrypted passwords.
