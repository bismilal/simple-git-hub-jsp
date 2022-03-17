# simple-git-hub-jsp
Assisted Practice: 4.1 Creating a Simple JSP File

This section will guide you to:
●	Create a JSP file and run it in the browser

Development Environment
●	Eclipse IDE for Enterprise Java Developers v2019-03 (4.11.0)
●	Apache Tomcat Server v9.0
●	JRE: OpenJDK Runtime Environment 11.0.2

This lab has seven subsections, namely:
4.1.1	Creating a dynamic web project
4.1.2	Creating a JSP file index.jsp
4.1.3	Checking for servlet-api.jar
4.1.4	Building the project
4.1.5	Publishing and starting the project
4.1.6	Running the project
4.1.7	Pushing the code to your GitHub repositories

 
Step 4.1.1: Creating a dynamic web project
•	Open Eclipse 
•	Go the File menu. Choose New->Dynamic Web Project
•	Enter the project name as SimpleJSP. Click on Next
•	Enter nothing in the next screen and click on Next
•	Check the checkbox Generate web.xml deployment descriptor and click on Finish
•	This will create the project files in the Project Explorer

Step 4.1.2: Creating a JSP file index.jsp
•	In the Project Explorer, expand the project SimpleJSP
•	Expand WebContent. Right click on WebContent. Choose New->JSP File
•	Enter the filename as index.jsp and click on Finish
•	Enter the following code:

<%@ page language="java" contentType="text/html; charset=UTF-8"     pageEncoding="UTF-8"%>
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Simple JSP</title>
</head>
<body>
<%
        out.println("<h2>My first JSP page.</h2>");
%>
</body>
</html>
•	Click on the Save icon

Step 4.1.3: Checking for servlet-api.jar
•	Before building the project, we need to add servlet-api.jar to the project
•	Servlet-api.jar file is already present in your practice lab. (Refer FSD: Lab Guide - Phase 2)
•	To add it to the project, follow the below mentioned steps:
◦	In the Project Explorer, right click on SimpleJSP and choose Properties
◦	Select Java Build Path from the options on the left
◦	Click on Libraries tab on the right
◦	Under ClassPath, expand the node that says Apache Tomcat 
◦	If there is an existing entry for servlet-api.jar, then click on Cancel and exit the window
◦	If it is not there, then click on Classpath entry and click on Add External JARs button on the right
◦	From the file list, select the servlet-api.jar file and click on Ok
◦	Click on Apply and Close

Step 4.1.4: Building the project
•	From the Project menu at the top, click on Build
•	If any compile errors are shown, fix them as required

Step 4.1.5: Publishing and starting the project
•	If you do not see the Servers tab near the bottom of the IDE, go to Window menu and click on Show View->Servers
•	Right click on the Server entry and choose Add and Remove
•	Click the Add button to move SimpleJSP from the Available list to the Configured list
•	Click on Finish
•	Right click on the Server entry and click on Publish
•	Right click on the Server entry and click on Start
•	This will start the server

Step 4.1.6: Running the project
•	To run the project, open a web browser and type: http://localhost:8080/SimpleJSP

Step 4.1.7: Pushing the code to your GitHub repositories
●	Open your command prompt and navigate to the folder where you have created your files.
cd <folder path>
●	Initialize your repository using the following command:
git init
●	Add all the files to your git repository using the following command:
git add .
●	Commit the changes using the following command:
git commit .  -m “Changes have been committed.”
●	Push the files to the folder you initially created using the following command:
git push -u origin master


