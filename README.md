# Securing-Web-App-using-Spring-Boot
This project demonstrates the implementation of a secure web application using **Spring Boot** and **Thymeleaf**. The application includes basic user authentication, role-based access control, and navigation through different HTML pages (`home`, `hello`, and `login`). The security configurations are done using `WebSecurityConfigurerAdapter` and MVC configuration classes.

## Features
- **User Authentication:** Implements login functionality and restricts access to certain pages based on user roles.
- **Thymeleaf Integration:** Uses Thymeleaf for rendering dynamic HTML pages.
- **Role-Based Access Control:** Configures specific pages to be accessible only after authentication.
- **Spring Security:** Configured to manage user authentication, session management, and secure routes.

## Technologies Used
- **Spring Boot**
- **Thymeleaf**
- **Spring Security**
- **Java**

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/web-security-spring-boot.git
    cd web-security-spring-boot
    ```

2. Build the project using Maven:
    ```bash
    mvn clean install
    ```

3. Run the application:
    ```bash
    mvn spring-boot:run
    ```

4. Access the application:
    - Navigate to `http://localhost:8080/home` for the home page.
    - Navigate to `http://localhost:8080/hello` for a greeting (requires login).

## Usage
- By default, the application is configured with an in-memory user:
    - **Username:** `user`
    - **Password:** `password`

- Pages:
    - `/home` – Public page.
    - `/hello` – Secured page, accessible only after login.
    - `/login` – Login page for user authentication.

## Project Structure

- **MvcConfigure:** Defines the view controllers for the application (e.g., `/home`, `/hello`, `/login`).
- **WebSecurityConfig:** Manages the security configurations, allowing access control for different pages and handling user authentication.
- Thymeleaf templates:
    - **home.html:** Public page.
    - **hello.html:** Protected page accessible only after login.
    - **login.html:** Custom login page.

## Contributing
Feel free to open issues or submit pull requests. Any contributions to improve the application or its security features are welcome!

## License
This project is licensed under the MIT License.
