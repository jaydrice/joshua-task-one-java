# First-Project-Java-Spring

This is a Spring Boot application developed as part of the "First-Project-Java-Spring" project. It utilizes Thymeleaf for dynamic webpage rendering and serves static images.

## Overview
- **Application Name**: First-Project-Java-Spring
- **Purpose**: Demonstrates a basic Spring Boot controller setup with Thymeleaf templates 
- **Controllers**:
  - `HelloController`: Returns a plain text greeting at `/`.
  - `GreetingController`: Renders a Thymeleaf template at `/greeting` with a dynamic `name` parameter.

## Screenshots

![death-the-kid png (360×306) - Google Chrome 5_17_2025 9_24_17 PM](https://github.com/user-attachments/assets/4daadc93-76d2-41ae-bdd3-522cc187dd4a)

- Successfully served from `http://localhost:8080/images/death-the-kid.png`.

### Root Page at `/`

![localhost_8080 - Google Chrome 5_17_2025 4_48_07 PM](https://github.com/user-attachments/assets/3f1f821e-ab32-4db9-ad9a-cde8a875816f)

- Displays the text "Hello Vistula, this is Jay speaking. In my first Spring Controller." at `http://localhost:8080/`.

## Setup
- **Controllers**: Split into `HelloController.java` and `GreetingController.java` in `pl.edu.vistula.first_project_java_spring.controller`.
- **Template**: `greeting.html` in `src/main/resources/templates/` uses Thymeleaf to display "Hello, ${name}!" and an image.
- **Image**: `death-the-kid.png` placed in `src/main/resources/static/images/` for use in the template.

## Build Instructions
Run the Spring Boot application and access:
   - `mvn spring-boot:run` to start Maven
   - `http://localhost:8080/` for the HelloController output.
   - `http://localhost:8080/greeting?name=Vistula` to see the Thymeleaf template with the image.

## Notes
- The `GreetingController` renders `greeting.html` with the `name` parameter.
- Verify Thymeleaf and web dependencies in `pom.xml`.
