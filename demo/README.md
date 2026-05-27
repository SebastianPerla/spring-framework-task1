# Spring Framework Task 1

This project is Task 1 for the Spring Framework assignment.

## Technologies

- Java 17
- Spring Boot
- Maven
- Spring Web MVC
- Thymeleaf

## Description

The application demonstrates a basic Spring Boot MVC project.

It contains:

- a controller,
- a direct HTTP response using `@ResponseBody`,
- a Thymeleaf HTML view,
- a static image loaded from the resources folder.

## How to run

Run the main class:

```text
DemoApplication
```

The application starts on:

```text
http://localhost:8080
```

## Endpoints

### Basic response

HTTP method:

```text
GET
```

URL:

```text
http://localhost:8080/
```

Expected response:

```text
Hello Vistula, in my first Spring controller.
```

This endpoint uses `@ResponseBody`, so the returned text is written directly into the HTTP response body.

### Employees response

HTTP method:

```text
GET
```

URL:

```text
http://localhost:8080/employees
```

Expected response:

```text
Sebastian Perla, Cristiano Ronaldo, Wilson Perla
```

### Greeting view

HTTP method:

```text
GET
```

URL:

```text
http://localhost:8080/greeting?name=Vistula
```

Expected result:

The browser displays `greeting.html` with the text:

```text
Hello, Vistula!
```

The page also displays the `vistula.png` image from:

```text
src/main/resources/static/images/vistula.png
```

## Important files

- `src/main/java/com/example/demo/DemoApplication.java` - starts the Spring Boot application.
- `src/main/java/com/example/demo/EmployeeController.java` - handles HTTP requests.
- `src/main/resources/templates/greeting.html` - Thymeleaf view.
- `src/main/resources/static/images/vistula.png` - image used in the view.

## Screenshots

Add screenshots here before submitting:

- `http://localhost:8080/`
- `http://localhost:8080/greeting?name=Vistula`
