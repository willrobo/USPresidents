# US Presidents
A Java web application that displays important and interesting information about all US presidents.

## Application URL
http://www.shaundashjian.com:8080/USPresidents

## How to Use the Application
The user could go through the list of all U.S. Presidents. The User could search by term number, go to the next or previous president.

## Technology
The application uses the MVC architecture with JSP and servlets.

1. **The DAO:**
The DAO (Data Access Object) reads the input from a file and catches an exception if you try to type in a president other than presidents 1-45
It also has a getPresident() method to get the president object.
2. **The Servlet:**
The servlet gets the information from the DAO and maintains session-specific information per user. It manages which president is being presented based on termNumber with the current president variable. If the user goes past president 45 it goes back to president 1 and if the user goes below president 1 it move them to president 45.
3. **The JSP:**
The JSP uses [Bootstrap](http://getbootstrap.com). It makes the current president appear. It has 2 arrows that move through the hashmap of presidents. It has a text box which allows you to search by term number as well as next and previous buttons.

