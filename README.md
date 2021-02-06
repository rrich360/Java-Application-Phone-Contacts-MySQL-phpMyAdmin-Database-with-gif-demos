# Java-Phone-App-For-Contacts


# Project Summary : 

 In this Java project, you will see how to make a phone app for managing contact
information from friends, colleagues, co-workers, and familly. In this app, the user
can update their picture with their contact information. 

  Also, the user can store more 
information than usual due to the additional address field along with name, phone number, 
email, and group. The address field could automatically calibrate route for user convenience 
when they are driving. 

 This app is mainly comprised from NetBeans Editor, MySQL Database, and phpMyAdmin Database 
to securely store the user’s login data and contacts that he or she may have included in their 
phone. 





# Objectives for this Java Application: 

- Connect Java to MySQL. 
- Create a SignUp Form.
- Create a Login Form. 
- Read data from MySQL Database.
- Update Data to MySQL. 
- Delete Data from Database.
- Populate table in phpMyAdmin Database.
- Display images in contacts profile.
- Search Data in MySQL Database. 
- Display selected data in text fields. 
- Insert, Update, Delete Image from Database. 



# Tools used in this Java Project : 

- Java SE 8 . 
- NetBeans IDE .
- XAMPP .
- PhpMyAdmin .
- MySQL Database .



# HOW IT WORKS :


 1 - SignUp Form
 
•	In this form a new user can register to the system and I used a error function to check if the username 
already exists in the database. 

•	I used a browseImage function to enable the user to add a picture to their profile. 

•	Created a verify function to check the following :
  - if the first name + last name + username + password is void
  - if the password field equals the retype password field
  - if the username is already selected or if an image is not inserted
  - verify that when you click on "create a account" link in the login form, it closes and automatically
    redirects to the SignUp form.
  - verify that when you click on "already have a account" link in the SignUp form, it redirects the user to the Login form.



![1 0-signUpForm](https://user-images.githubusercontent.com/20470279/60803507-6161e180-a149-11e9-9c48-269cd20be534.JPG)




2 - Login Form

•	In this form the user can log in to the system by entering the username and password.

•	If you enter the wrong username or password an error message will popup. Otherwise, the contact form should pop up.

•	The user can show and hide the password characters by checking the checkbox (ShowPass).

•	When you click on 'CreateAccount' link, the form will close and redirect to the SignUp.



![2 0-loginForm](https://user-images.githubusercontent.com/20470279/60803513-645cd200-a149-11e9-9ec4-d0f3c97c099d.JPG)




3 - Main Form

•	When the user logs in successfully, this form will show up with the logged user profile pic and username displayed 
in the left top part of the form which is circled in red.



![3 0-MainFormForContacts](https://user-images.githubusercontent.com/20470279/60803518-66bf2c00-a149-11e9-8812-b659ff407716.JPG)





as you can see when the user logs in successfully, a contact list will appear in the jtable at the bottom of the form, when 
you select a row from the jtable the data will be displayed into the fields.



![3 1-Contacts](https://user-images.githubusercontent.com/20470279/60803521-69218600-a149-11e9-86f7-53dbfa8e3c1c.JPG)




you can add, edit, or delete contacts. In the form the user also has the option of navigating between contacts, whether it be 
navigating forwards; backwards; skip from back to front of the contact list.




4.Functions code used in this Form


populateJtable : to display the logged user contacts in jtabel . The code circled in red allows the picture file to be scaled to size 
automatically when added with the contact information. The red check mark displayed is where the picture is set after the scaling is complete. The 
following picture below displays the code for the function : 



![4 0](https://user-images.githubusercontent.com/20470279/60803523-6b83e000-a149-11e9-9dcb-4d3c091781cc.JPG)



browseImage : to browse image from the computer to the jlabel . The following picture below is an example of the code used 
for browseImage.




![4 1](https://user-images.githubusercontent.com/20470279/60803533-6f176700-a149-11e9-9939-1477ce2509a2.JPG)



insertContact : function from the contactQuery class to insert a new contact into the database . The following picture below
displays the code for insertContact.



![4 2](https://user-images.githubusercontent.com/20470279/60803538-72aaee00-a149-11e9-8ba2-36e5553424aa.JPG)


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



