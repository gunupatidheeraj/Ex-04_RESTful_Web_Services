# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/607ea0df-5d62-4017-b267-2f6f1657f0d6)



Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 
 ![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/f4a8c6a7-af6d-4868-a3cb-9c3ee8f22085)



Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.



![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/eb4a78b6-a2c9-41cc-a151-9df9048b5d0f)


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 

 ![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/3b49f04b-2ca9-4685-88fa-1db9fbb10056)



Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.


![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/af417b59-9772-4ba9-8394-af71c001d4b0)



Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.

 Step 4: Carefully select your RESTful resource (web service) and click OK.
 
![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/d61e628d-ecde-4303-b212-159c8ecd3c28)


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.



![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/f8941114-6984-4e56-946f-d1ecd0a41e81)

Step 6: An editing tab will open. Alter getHtml() method with the following.
 
 ![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/5c362b93-215d-4e05-a8bc-46e19b8f62ca)



Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.


![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/62f09826-cf7b-431c-85b8-23fb562a8ffa)

Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 

 ![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/ac75e4e1-6ad5-499b-8ce2-564e4d28f0e5)



Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.


![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/94ddc5ae-c10e-469e-b6c5-c783cf7e458e)


Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 
![image](https://github.com/gunupatidheeraj/Ex-04_RESTful_Web_Services/assets/146909163/def44ee6-d23b-487f-aaaa-9c7839c1e360)


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
