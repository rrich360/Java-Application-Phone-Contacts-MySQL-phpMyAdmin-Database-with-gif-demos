# Java-Phone-App-For-Contacts


# Project Summary : 

 In this Java project, you will see how to make a phone app for managing contact
information from friends, colleagues, co-workers, and familly. In this app, the user
can update their picture with their contact information. 


# Objectives for this Java Application: 
 
- Create a SignUp Form.
- Create a Login Form. 
- Connect Java to MySQL.
- Read data from MySQL Database.
- Update Data to MySQL. 
- Delete Data from Database.
- Populate table in phpMyAdmin Database.
- Display images in contacts profile.
- Search Data in MySQL Database. 
- Display selected data in text fields. 
- Insert, Update, Delete Image from Database. 



# Tech stack used in this Project : 

- Java SE 8 . 
- NetBeans IDE .
- Server environment in directory folder (Windows,Apache,MySQL,PHP)
- PhpMyAdmin .



# HOW IT WORKS :


# 1 - Register Form
 
•	In this form a new user can register to the system and I used a error function to check if the username 
already exists in the database. 

•	I used a browseImage function to enable the user to add a picture to their profile. 

•	Created a verify function to check the following :
  - if the first name + last name + username + password is void
  - if the password field equals the retype password field
  - if the username is already selected or if an image is not inserted
  - verify that when you click on "create a account" link in the login form, it closes and automatically
    redirects to the Register form.
  - verify that when you click on "already have a account" link in the Register form, it redirects the user to the Login form.



![Registration Form](https://user-images.githubusercontent.com/20470279/107133506-efb6c000-68b6-11eb-8486-f39237ebc2cd.gif)




# 2 - Login Form

•	In this form the user can log in to the system by entering the username and password.

•	If you enter the wrong username or password an error message will popup. Otherwise, the contact form should pop up.

•	The user can show and hide the password characters by checking the checkbox (ShowPass).

•	When you click on 'CreateAccount' link, the form will close and redirect to the Registration form.


![Login-Form](https://user-images.githubusercontent.com/20470279/107137126-4d5b0480-68d7-11eb-8601-72cf590b601a.gif)



# 3 - Contact Form

•	When the user logs in successfully, this form will show up with the logged user's profile pic in the top-left corner of the UI next to the username displayed 
in the left-top corner as well. A contact list will appear in the bottom table of the form, when 
you select a row from the table, the contact information will be appear into the fields.




![Contact-UI](https://user-images.githubusercontent.com/20470279/107137858-7c28a900-68de-11eb-8f6c-0407c9ac94f4.gif)



# 4 - Functionality of the contact UI

you can add, edit, or delete contacts. In the form the user also has the option of navigating between contacts, whether it be 
navigating forwards; backwards; skip from back to front of the contact list.


![Add-delete-user](https://user-images.githubusercontent.com/20470279/107138521-dd527b80-68e2-11eb-9e7e-160e3d48bb92.gif)


# 5 - Store users and contacts in seperate tables in the database 
insertContact : function from the contactQuery class to insert a new contact into the database. In a use-case scenario, where new users have registered and subscribed to the phone app, I created a table called 'users' in the 'javacontactsapp' database. Also, in a scenario where the users want to add contacts from friends, family, and colleagues in their profile, I created a seperate table called 'mycontacts' in the same database. 



![Store-user-database](https://user-images.githubusercontent.com/20470279/107140825-d9c6f080-68f2-11eb-817b-f8709200d39b.gif)




# 6 - Update contact information 
updateContact : The gif you see below demonstrates an instance when the app prompts the user to update the contact info WITH profile picture if NO picture is inserted.



![edit-store-contact](https://user-images.githubusercontent.com/20470279/107141470-e2b9c100-68f6-11eb-8e79-2f5be45d10f9.gif)
# 


updateContact : The code below represents the function that allows the contact information to be updated without changing the profile picture. 


![4 6](https://user-images.githubusercontent.com/20470279/60803936-5196cd00-a14a-11e9-8200-c36120430cb0.JPG)
# 


deleteContact : is the function from the contactQuery class to remove the selected contact information from the database .




![4 7](https://user-images.githubusercontent.com/20470279/60803941-53f92700-a14a-11e9-8194-19eff6f98f41.JPG)







