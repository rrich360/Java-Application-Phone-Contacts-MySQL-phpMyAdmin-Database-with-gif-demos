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



# 4 - Functionality of contact UI

you can add, edit, or delete contacts. In the form the user also has the option of navigating between contacts, whether it be 
navigating forwards; backwards; skip from back to front of the contact list.


![Add-delete-user](https://user-images.githubusercontent.com/20470279/107138521-dd527b80-68e2-11eb-9e7e-160e3d48bb92.gif)


# 5 Store users and their contacts in database 
insertContact : function from the contactQuery class to insert a new contact into the database. 



populateJtable : to display the logged user contacts in jtabel . The code circled in red allows the picture file to be scaled to size 
automatically when added with the contact information. The red check mark displayed is where the picture is set after the scaling is complete. The 
following picture below displays the code for the function : 



![4 0](https://user-images.githubusercontent.com/20470279/60803523-6b83e000-a149-11e9-9dcb-4d3c091781cc.JPG)



browseImage : to browse image from the computer to the jlabel . The following picture below is an example of the code used 
for browseImage.




![4 1](https://user-images.githubusercontent.com/20470279/60803533-6f176700-a149-11e9-9939-1477ce2509a2.JPG)




refreshJtable : to clear and populate a jtable again after insert update delete to show the new data . The following picture 
below displays the code for refreshJtable.


![4 3](https://user-images.githubusercontent.com/20470279/60803558-79396580-a149-11e9-97c3-f86c807e1b80.JPG)


clearFields : to clear all fields, set the comboBox selected index to 0, set jtabel icon to null,  set imgPath to null. The 
following picture displays the code that clears all the fields in the contact list.




![4 4](https://user-images.githubusercontent.com/20470279/60803913-4643a180-a14a-11e9-9096-12a93d94a231.JPG)



updateContact : this function is from the contactQuery class that edits the selected contact information. The following picture 
displays the code for this function. The red circle includes the Boolean status for true along with the prepared statement query 
for Pic if the user wants to update their picture with their contact info.




![4 5](https://user-images.githubusercontent.com/20470279/60803920-49d72880-a14a-11e9-9dea-dd582e8e2af6.JPG)




The following picture below displays the output when the contact information is edited and updated : 




![4 55-contact edited](https://user-images.githubusercontent.com/20470279/60803930-4e034600-a14a-11e9-846a-3be09fb33027.JPG)



updateContact : The code you see below is part of the function that is displayed in the picture above except the code has the option 
for updating the contact info WITHOUT the picture.




![4 6](https://user-images.githubusercontent.com/20470279/60803936-5196cd00-a14a-11e9-8200-c36120430cb0.JPG)





deleteContact : is the function from the contactQuery class to remove the selected contact information from the database .




![4 7](https://user-images.githubusercontent.com/20470279/60803941-53f92700-a14a-11e9-8194-19eff6f98f41.JPG)



showData : this function allows navigation between contacts on the form ( show first, next, pervious, last ).



![4 9](https://user-images.githubusercontent.com/20470279/60803944-565b8100-a14a-11e9-81cb-0073a6796626.JPG)




The picture below displays the output for the contact form used in the phone app. The following contacts can be seen with pictures 
and can be traversed through via directional tags circled in red.



![5 0](https://user-images.githubusercontent.com/20470279/60803949-58bddb00-a14a-11e9-9389-a2e277275990.JPG)


The following picture below is an example of all the contact information being stored in phpMyAdmin Database after the profiles have been created for contacts in the phone. I created a table called 'mycontacts' in the database.



![5 1](https://user-images.githubusercontent.com/20470279/60803954-5c516200-a14a-11e9-9cad-a34110ea27f4.JPG)



The following picture below is an example of all the users who signed up to access thier contact form in order to store additional contacts from friends, family, and colleagues in their cell phones. I created a table called 'users' in the database.


![5 2-usersTablephp](https://user-images.githubusercontent.com/20470279/60803962-5eb3bc00-a14a-11e9-9828-e8d31d94af43.JPG)



