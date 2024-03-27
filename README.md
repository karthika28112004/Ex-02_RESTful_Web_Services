# Ex-02_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/5622815a-06d6-4787-a5b5-36df577e7981)

Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.




Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/6da95ca3-942f-42ff-b4cd-9e94371db4a3)

 
 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/f534f2ca-9849-4002-b76f-b28877c38d13)



Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/8c01ee00-fa4c-4c4b-bbbb-f9d6f418a548)

Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 

 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/688de30e-6347-4e7f-802c-019ee034e6ef)




Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.




Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/68c96ebb-79f7-4d01-8969-d5cf63e17e35)

 
 


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/f0d95985-1732-4791-b973-2a97a252bc0e)



Step 6: An editing tab will open. Alter getHtml() method with the following.
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/4995fcac-28a7-4bc0-8152-a6029073ebb9)

 
 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/6204fadb-7a02-4e12-ac57-fa2feb1dac1b)



Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/e523b04d-b7ef-40df-ad11-98e241a6c016)

 
 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/7dc1aa4c-83b4-4cd5-9070-2ffc2c042cab)



Step 11: Save the project and build it.
![image](https://github.com/karthika28112004/Ex-02_RESTful_Web_Services/assets/128035087/b12d6820-44fe-4ec1-8257-140a915033a5)

Step 12: Run the JSP file and you should see the output in a new browser window.
 
 


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
