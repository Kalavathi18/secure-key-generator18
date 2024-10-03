# Random Password Generator

## Overview

The Random Password Generator is a web-based application that allows users to generate strong, random passwords based on their preferred length. The application uses a secure server-side method to generate passwords with a mixture of letters, numbers, and special characters.

The front-end is built with HTML, CSS, and JavaScript, while the back-end utilizes Java Servlet for generating passwords.

## Screenshot
![image alt](https://github.com/Kalavathi18/secure-key-generator18/blob/610685a1d0fe69ea0b47da8258760b9d437bd048/Screenshot%20(166).png)
![image alt](https://github.com/Kalavathi18/secure-key-generator18/blob/27a0f0c3586ec991422330fe8825e030ce9b11d7/Screenshot%20(167).png)
![image alt](https://github.com/Kalavathi18/secure-key-generator18/blob/27a0f0c3586ec991422330fe8825e030ce9b11d7/Screenshot%20(168).png)


## Features

- Responsive user interface with a modern look.
- Password length customization (1 to 100 characters).
- Secure password generation using `SecureRandom`.
- SweetAlert2 integration for interactive alert dialogs.

## Technologies Used

- **Java Servlet (Back-end)**
- **HTML, CSS (Front-end)**
- **JavaScript with SweetAlert2 for user interactions**
- **SecureRandom for password generation**

## Project Structure

- `index.html`: Contains the front-end logic and form for password length input.
- `PasswordGeneratorServlet.java`: Java servlet responsible for generating random passwords.
  

## Setup Instructions

### Prerequisites

- **Java EE** environment setup.
- **Apache Tomcat** or another servlet container for running the Java servlet.
- Basic knowledge of Servlets and HTML.

### Steps to Run the Project

1. Clone or download the project repository.
2. Import the project into your IDE (Eclipse/IntelliJ).
3. Configure a servlet container (like Tomcat) in your IDE.
4. Deploy the project to your servlet container.
5. Open the `index.html` file in a web browser or access the application via the deployed server (e.g., `http://localhost:8080/your-app-name`).
6. Enter the desired password length and generate the password by submitting the form.

### API Endpoint

- **`/generatePassword`**: The endpoint that generates the random password. It accepts a `GET` request with a `length` parameter.

#### Example Request:

```http
GET /generatePassword?length=10
