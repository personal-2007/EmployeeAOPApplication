# EmployeeAOPApplication

A simple Employee Management Application developed using **Java, Spring Framework, Spring AOP, and Maven**. This project demonstrates basic employee operations and automatic logging using annotation-based configuration without XML.

## Features

- Add employee details
- Display employee ID and name
- Calculate and display employee salary
- Automatically log messages before each service method executes using Spring AOP
- Configure Spring using annotations instead of XML
- Manage dependencies using Maven

## Technologies Used

- Java 17+
- Spring Framework 6
- Spring AOP
- AspectJ Weaver
- Maven
- Eclipse IDE

## Project Structure

```text
EmployeeAOPApplication/
├── pom.xml
├── README.md
└── EmployeeAOPApplication/
    └── src/
        └── main/
            └── java/
                └── com/
                    └── employee/
                        ├── AppConfig.java
                        ├── Main.java
                        ├── EmployeeService.java
                        └── LoggingAspect.java
```

## Application Output

```text
Logging: Adding employee
Employee added: Selva
Logging: Displaying employee
Employee ID: 101
Employee Name: Selva
Logging: Calculating salary
Employee Salary: 25000.0
```

## How to Run in Eclipse

1. Clone or download this repository.
2. Open Eclipse IDE.
3. Import the project using **File → Import → Existing Maven Projects**.
4. Select the project folder containing `pom.xml`.
5. Right-click the project and select **Maven → Update Project**.
6. Ensure Java 17 or later is configured.
7. Open `Main.java`.
8. Select **Run As → Java Application**.
9. View the execution output in the Eclipse Console.

## Spring AOP Implementation

The `LoggingAspect` class uses the `@Aspect`, `@Component`, and `@Before` annotations to intercept employee service methods and print log messages before execution.

The `AppConfig` class uses `@Configuration`, `@ComponentScan`, and `@EnableAspectJAutoProxy` to configure the application without XML.

## Database

MySQL is not required for this project. Employee details are stored in Java instance variables during execution and are not permanently saved.

## Learning Objectives

- Understand Spring dependency management with Maven.
- Learn annotation-based Spring configuration.
- Implement Spring AOP using AspectJ annotations.
- Apply before advice to service methods.
- Build and run a Spring application in Eclipse.

## Author

**Selva**

GitHub Repository: https://github.com/personal-2007/EmployeeAOPApplication
