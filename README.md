# This project simulates the work of a "Taxi Service".

# What can the service do?
- Adding and removing car models.
- Adding and removing cars.
- Adding and removing drivers.
- Adding drivers to specific cars.
- Display the list of all cars.
- displaying the list of all cars of the given driver.
- Authentication system is realized as well

# How to run?
1. Clone this repository.
2. Open a database environment (e.g. MySQLWorkbench). 
3. And run the script from src/main/resources/init_db.sql in the console.
4. Add the username to your database password in ConnectionUtil.
5. Build the project using the Maven command mvn clean package.
6. Deploy the WAR file to a servlet container. (You can use Tomcat. But no older than version 9).
7. After starting the servlet container, go to the page in your browser http://localhost:8080 .
8. If everything is correct you should get to the login page.

# How does the structure work?
- controller: Servlets that handle HTTP requests and responses.
- dao: Data Access Object interfaces and their implementations.
- model: Plain Old Java Objects (POJOs) that represent data.
- service: Service interfaces and their implementations that perform business logic.
- util: Utility class used in a project to create a database connection.
- filter: Servlet Filters used to intercept requests and responses.
- resources: Non-Java files such as database scripts.
- webapp: Contains web resources such as JSP files.
- WEB-INF: Contains configuration files for the web application.
- views: Contains JSP files used as views in the application for cars, drivers, manufacturers, authentication.

# Used Technologies
- Java `v.18.0.2`
- Maven `v.3.8.0`
* JDBC `v.4.2`
* MySQL `v.8.0.22`
* Java Servlets `v.4.0.1`
* Tomcat `v.9.0.7`