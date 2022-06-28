# GameGo
GameGo is a website application that offers users a hardcore gaming experience. The application makes it easy for our gamers to purchase and download the most popular games. 

GameGo Ecommerce consists of the following components:

- Spring boot Java / Spring boot backend
- Angular administration web application
- Node JS front end application


![Free_Sample_By_Wix (2)](https://user-images.githubusercontent.com/99148885/176082439-1fa8b817-be75-4e60-a6cf-5934eff5782c.jpg)


Features:
Registration is free for new users.
-	A user's profile page can be created and maintained.
-	Using the application, users can login.
-	Products available for adding to the shopping cart
- Cart containing the items the user has added for purchase and removing items that the user no longer wants to purchase.
-	Remove the purchased items from the inventory by checking out the items in the cart.

The following technologies were used for the backend:

- An endpoint for AWS
- PostgreSQL for the database.
- Implementing Hibernate so that clients can access data bases
- Access the database using a session.
- Objects are abstracted away from the database structure, so we do not have to map them to the objects.
- Create tables using annotations in JPA.

Configuring Hibernate:

- Create a maven project with the Spring tool suite.
- Create the Postgres and Hibernate dependencies on the pom.xml file.
- The new file should be called hibernate.cfg.xml and placed in the src/main/resources folder
-  Use the boilerplate code in a generic text editor.
- Replace "localhost" in line 13 with the AWS endpoint URL and the name of the new schema created in DBeaver.
- The name of the schema on line 18 should match the name on line 13.
- Important: After you run Hibernate for the first time, On line 23 replace the “create” keyword with “update”.

Spring Boot (Spring Project)

· Used to create standalone Spring-based applications that you can just run”

Configuration:

- Open a maven project
- On the pom.xml file create the dependencies
- In the src/main/resources, create a new file and call it applicationContext.xml
- Right click the applicationContext.xml file and Open with Generic text editor and use the boilerplate code.
- Wiring Beans with Annotation Driven (stereotype annotations)
- @Component- makes the class a Bean
- @Repository - DAO/Repository classes that you want to make a Spring Bean
- @Service - Service classes that you want to make a Spring Bean
- @Controller - Controller Classes that you want to make a Spring Bean (this annotation actually has additional functionality if using Spring MVC)
- Spring MVC: enables us to create complex applications also using plain java classes. The model object can be passed between view and controller using maps.

Spring MVC Structure:

DispatcherServlet - This is SpringMVC’s Front Controller, works under the hood, so we just have to configure it and HTTP requests will go straight to our controller layer.

HandlerMapping - This is an Interface that is responsible for sending requests to the proper controller.

- @Controller: with Spring MVC, it indicates that the class will handle HTTP requests from the DispatcherServlet.
- @RequestMapping: This annotation in a @Controller Class specifies what URIs the controller will handle. It can be placed before the Class declaration or above a method declaration.
- There are also @___Mapping annotations that specify what verbed requests go to a certain method E.g. @GetMapping
- Logging (with Log4j): We use Logging in our project to record application events, debugging information, or other notable occurrences during the application’s runtime.

Configuration

- We need a log4j2 maven dependency in our pom.xml
- We will employ the use of the log4j2.properties file in our src/main/resources folder to set configurations for log4j. This includes configurations such as:
- Threshold level
- Where the log transcript will populate
- Other stuff we don’t really really have to know

Frontend

- Angular is a development platform, built on TypeScript. As a platform, Angular includes:
- A component-based framework for building scalable web applications.
- A collection of well-integrated libraries that cover a wide variety of features, including routing, forms management, client-server communication, and more.

Configuration

- Install Node Js
- Install npm package manager
- Install the Angular CLI, open a terminal window and run the following command:
- Create a workspace and initial application
- Run the application
- The Angular CLI includes a server, for you to build and serve your app locally.
- Navigate to the workspace folder, such as my-app.
- Run the following command
- The ng serve command launches the server, watches your files, and rebuilds the app as you make changes to those files.
- The --open (or just -o) option automatically opens your browser to http://localhost:4200/.
- If your installation and setup was successful, you should see a page similar to the following.

