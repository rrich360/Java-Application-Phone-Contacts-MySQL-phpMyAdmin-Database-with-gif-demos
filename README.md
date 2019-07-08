# Java-Phone-App-For-Contacts


Project Summary : 

In this Java project, you will see how to make a phone app for managing contact
information from friends, colleagues, co-workers, and familly. In this app, the user
can update their picture with their contact information. Also, the user can store more 
information than usual due to the additional address field along with name, phone number, 
email, and group. The address field is convenient for users who may choose to be in route 
to their friend’s house or etc they could upload it to GPS. The app mainly uses Java with 
NetBeans Editor and MySQL Database to securely store the user’s login data and contacts that 
the user may have included in their phone. 





Java Swing Components used in this project : 

- JFrame 
- JPanel 
- JTextfield.
 - JButton. 
- JTabel. 
- JLabel. 
- JDatechooser. 
- JCombobox. 
- JTextarea 




Objectives for this Java Application: 

- Connect Java to MySQL. 
- Create a SignUp Form.
 - Create a Login Form. 
- Insert Data to MySQL Database.
 - Update Data to MySQL. 
- Delete Data from Database.
 - Populate JTable From MySQL Database.
 - Create a JTable Model. 
- Display Images in a JTable.
 - Populate JCombobox From MySQL Database.
 - Search Data in MySQL Database. 
- Display Selected JTable Row Data in JTextFIelds. 
- Insert, Update, Delete Image from Database. 



Tools used in this Java Project : 

- Java SE 8 . 
- NetBeans IDE .
 - XAMPP .
 - PhpMyAdmin .
 - MySQL Database .



HOW IT WORKS :


 1 - SignUp Form
 
•	In this form a new user can register to the system and we will use an isUsernameExist function… to check if the username 
already exists in the database, 

•	a browseImage function from Myfunc class to browse and show image into a jlabel ( in this form jlabel name is jLabelPic ), 

•	a verifData function to check the following :
  - if the first name + last name + username + password is void
  - if the password field equals the retype password field
  - if the username is already selected or if an image is not inserted
  - verify that when you click on jLabelCreateAccount the form closes and automatically
    opens the login form.                  



2 - Login Form

•	In this form the user can log in to the system by entering the username and password.

•	If you enter the wrong username or password an error message will popup. Otherwise, the contact form should pop up.

•	The user can show and hide the password characters by checking the checkbox ( jCheckBoxShowPass) 

•	When you click on jLabelCreateAccount this form will close and SignUp form will open.



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
automatically when added with the contact information. The red check mark is where the picture is set after the scaling is done. The 
following picture below displays the output : 



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




		PICTURE 4.4



updateContact : this function is from the contactQuery class that edits the selected contact information. The following picture 
displays the code for this function. The red circle includes the Boolean status for true along with the prepared statement query 
for Pic if the user wants to update their picture with their contact info.




		PICTURE 4.5




The following picture below displays the output when the contact information is edited and updated : 




PICTURE 4.55



updateContact : The code you see below is part of the function that is displayed in the picture above except the code has the option 
for updating the contact info WITHOUT the picture.




		PICTURE 4.6





deleteContact : is the function from the contactQuery class to remove the selected contact information from the database .




		PICTURE 4.7



showData : this function allows navigation between contacts on the form ( show first, next, pervious, last ).



		PICTURE 4.9




The picture below displays the output for the contact form used in the phone app. The following contacts can be seen with pictures 
and can be traversed through via directional tags circled in red.



		PICTURE 5.0






