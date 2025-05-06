# airbnb-clone-project

# About the Project
The Airbnb Clone Project is a comprehensive, real-world simulation of developing a robust booking platform similar to Airbnb. It focuses on full-stack backend development with an emphasis on backend systems, database architecture, RESTful and GraphQL APIs, application security, and CI/CD integration. The project also emphasizes collaborative workflows, scalability, and effective documentation practices.

#Project Goals
1. Develop a scalable and secure booking platform.

2. Understand backend system architecture and data management.

3. Implement secure APIs using modern frameworks.

4. Practice collaborative development using Git and GitHub.

5. Design and maintain CI/CD pipelines for efficient deployment.

6. Apply industry best practices in documentation, testing, and code quality.

   

# Team Roles
| Role                             | Responsibilities                                                                                        |
| -------------------------------- | ------------------------------------------------------------------------------------------------------- |
| **Backend Developer**            | Designs and implements server-side logic, RESTful APIs, and business rules using Django.                |
| **Database Administrator (DBA)** | Designs, optimizes, and manages the relational database schema using MySQL.                             |
| **DevOps Engineer**              | Sets up Docker environments, CI/CD pipelines, and automates deployment using tools like GitHub Actions. |
| **Security Analyst**             | Implements API security, manages authentication/authorization, and performs security audits.            |
| **Technical Writer/Documenter**  | Maintains project documentation including README, API docs, and design specifications.                  |


# Technology Stack
| Technology         | Purpose                                                                                 |
| ------------------ | --------------------------------------------------------------------------------------- |
| **Django**         | A Python web framework used to build RESTful APIs and handle backend logic.             |
| **PostgreSQL**     | A relational database used to store user, property, and booking data.                   |
| **GraphQL**        | An alternative API approach enabling efficient client-server data querying.             |
| **Docker**         | Used for containerization to ensure consistent development and production environments. |
| **GitHub Actions** | CI/CD tool used to automate testing, build, and deployment workflows.                   |
| **Markdown**       | For documentation and README formatting.                                                |



# Database Design
| Entity       | Fields                                             | Relationships                                                     |
| ------------ | -------------------------------------------------- | ----------------------------------------------------------------- |
| **User**     | id, name, email, password, role                    | A user can create multiple properties and make multiple bookings. |
| **Property** | id, title, description, location, owner\_id        | Belongs to a user (owner). Can have many bookings and reviews.    |
| **Booking**  | id, property\_id, user\_id, start\_date, end\_date | Belongs to a user and a property.                                 |
| **Review**   | id, property\_id, user\_id, rating, comment        | Belongs to a property and submitted by a user.                    |
| **Payment**  | id, booking\_id, amount, payment\_status           | Tied to a booking. One booking has one payment.                   |


