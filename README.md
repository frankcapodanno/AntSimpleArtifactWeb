# AntSimpleArtifactWeb

A simple JAVA EE Artifact based on Dynamic Web App of Eclipse that uses Maven Ant Task.
This simple artifact uses JAVA API 7 and the Jersey Rest 2.29 that use hk2 injection. This artifact support out of box servlets, jsp, rest services. This Projekt need **ANT**(>1.7) and **MAVEN** (>=3) installed.

## Project Structure
* .\WebContent --> Frontend and libs
* .\src\main\java --> Code
* .\src\test\java --> Tests
* .\maven-lib --> maven task jar
* .\server-lib --> libs that needs tomcat

## End-Points

* {Main Endpoint}/ --> JSP 
* {Main Endpoint}/servlet-test --> Servlet Example
* {Main Endpoint}/rest/api/resource --> Rest Example

## Ant tasks

Are defined different ant tasks. When you import this project in Eclipse, you need to execute as command **ant resolve** to download all neccessary libraries and after you need to refresh your projekt.

The tasks in order to execute :
* clean : remove the builds directories, reports directory, and the web application lib directory
* init : create all the builds directories, reports directory and the web application lib directory
* resolve : using Maven download all the dependencies
* compile : Compile the code
* test : if the compile is succesful g
* dist : Create the final WAR file (packaging)
