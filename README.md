✈️ Online Airlines Booking Platform

An Online Airlines Booking Platform application built with Spring Boot designed to manage flight logistics and enable seamless user booking. This system allows Admins to maintain all flight information and facilitates Users to search, view, and book available flights.

✨ Features and Workflow

This application implements a comprehensive flight management and booking workflow managed across two core user roles:

Admin/Staff Functionality (Flight Management):

Admins or authorized staff log in to the portal.

They are responsible for managing all aspects of the flight inventory, including:

Adding new flights with details like flight number, aircraft, and seating capacity.

Deleting flights that are no longer operational.

Updating flight details, including setting the starting point (source) and destination.

Adjusting flight timings (departure and arrival dates/times).

User/Passenger Functionality (Search & Booking):

Users (Passengers) can register and log in to the portal.

They can search and view flight details based on their desired source and destination.

Users can see all relevant information, including timings, dates, and ticket prices.

They can book flights accordingly and complete the reservation process through the portal.

Technical Features: Built on Spring Boot for robust backend logic and a clean, responsive front-end framework.

🚀 Getting Started

Follow these steps to set up and run the project on your local machine. You will be using Spring Tool Suite (STS) for development.

📋 Prerequisites

Ensure the following software is installed on your system:

Java Development Kit (JDK) 17+

Apache Maven (for dependency management and building)

MySQL Database (e.g., MySQL Workbench or a similar client)

Key Project Dependencies (Added via STS Initializer):
The project is built using the following core Spring Boot dependencies, which are typically included when creating the project in Spring Tool Suite (STS) or using the Spring Initializr:

Spring Data JPA: Used for interacting with the MySQL database via ORM (Object-Relational Mapping).

Spring Web (MVC): Enables the creation of the web application, handling requests, and defining RESTful endpoints.

MySQL Driver (Connector/J): The JDBC driver necessary to connect the Spring application to the MySQL database.

Spring Boot DevTools: Provides development-time features like automatic application restarts upon code changes.

⚙️ Installation and Setup

1. Database Setup

The first step is to create the necessary database and prepare the schema using MySQL.

Open your MySQL Workbench or command-line client.

Create the required database as specified for this project:

CREATE DATABASE online_airlines_booking;












2. Configuration Update

You need to update the database credentials in the Spring Boot configuration file.

Navigate to the configuration file:

src/main/resources/application.properties












Find the following lines related to MySQL connection and update them to match your local setup. Ensure the database name matches online_airlines_booking.

# Database Configuration Properties
spring.datasource.url=jdbc:mysql://localhost:3306/online_airlines_booking
spring.datasource.username=root
spring.datasource.password=YOUR_MYSQL_PASSWORD_HERE












3. Build and Run

With the database configured, you can now build and launch the application using Spring Tool Suite (STS).

Open Spring Tool Suite (STS):

Import the project as an existing Maven project.

Run the Application:

Right-click the project in the Project Explorer.

Select Run As -> Spring Boot App.

The application will now start, typically accessible at http://localhost:8080 unless configured otherwise.
