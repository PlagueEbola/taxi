# "Taxi Service" <img src="https://st2.depositphotos.com/1446370/8455/v/950/depositphotos_84558576-stock-illustration-black-and-yellow-taxi-logo.jpg" align="left" align="Right" height="50" width="50">
This project simulates the work of a taxi service.

# What can the service do? <img src="https://t3.ftcdn.net/jpg/03/41/59/78/360_F_341597890_zmd6lPFbUknozRmWxq1X1SGVkVZWSM1H.jpg" align="left" align="Right" height="50" width="50">
- Adding and removing car models.
- Adding and removing cars.
- Adding and removing drivers.
- Adding drivers to specific cars.
- Display the list of all cars.
- displaying the list of all cars of the given driver.
- Authentication system is realized as well

# How to run? <img src="https://thumbs.dreamstime.com/b/gear-logo-template-vector-icon-illustration-design-156835720.jpg" align="left" align="Right" height="50" width="50">
1. Clone this repository.
2. Open a database environment (e.g. MySQLWorkbench). 
3. And run the script from src/main/resources/init_db.sql in the console.
4. Add the username to your database password in ConnectionUtil.
5. Build the project using the Maven command mvn clean package.
6. Deploy the WAR file to a servlet container. (You can use Tomcat. But no bigger than version 9).
7. After starting the servlet container, go to the page in your browser http://localhost:8080 .
8. If everything is correct you should get to the login page.

# How does the structure work? <img src="https://previews.123rf.com/images/dstarky/dstarky1701/dstarky170101346/69424331-list-icon-or-logo-in-modern-line-style-high-quality-black-outline-pictogram-for-web-site-design-and.jpg" align="left" align="Right" height="50" width="50">
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

# Used Technologies <img src="https://png.pngtree.com/png-clipart/20210321/original/pngtree-technology-logo-template-png-image_6139771.jpg" align="left" align="Right" height="50" width="50">
* Java `v.18.0.2`
* Maven `v.3.8.0`
* JDBC `v.4.2`
* MySQL `v.8.0.22`
* Java Servlets `v.4.0.1`
* Tomcat `v.9.0.7`
