# BookMyShow -- Movie Ticket Booking Application

A full-stack movie ticket booking application built with a **Java Spring
Boot backend** and a **HTML, CSS, and JavaScript frontend**. The project
is organized into separate `Backend` and `Frontend` folders.

## Tech Stack

### Backend

-   Java
-   Spring Boot
-   Spring Data JPA
-   Hibernate / JPA
-   Maven
-   MySQL

### Frontend

-   HTML
-   CSS
-   JavaScript

## Project Structure

``` text
BookMyShow/
├── Backend/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/cfs/BookMyShowBE/
│   │   │   │   ├── config/
│   │   │   │   ├── controller/
│   │   │   │   ├── dto/
│   │   │   │   ├── entity/
│   │   │   │   ├── repository/
│   │   │   │   └── service/
│   │   │   └── resources/
│   │   │       └── application.properties
│   │   └── test/
│   ├── pom.xml
│   ├── mvnw
│   └── mvnw.cmd
├── Frontend/
│   ├── app.js
│   ├── index.html
│   └── style.css
└── .gitignore
```

## Backend Architecture

The backend follows a layered structure:

-   **Controller:** Handles incoming HTTP requests and returns API
    responses.
-   **Service:** Contains application and business logic.
-   **Repository:** Uses Spring Data JPA to interact with the database.
-   **Entity:** Represents persistent application data.
-   **DTO:** Defines the data exchanged between the client and backend.
-   **Config:** Holds application configuration, including cross-origin
    settings.

## Main Application Areas

The codebase is organized around these application areas:

-   Movies
-   Theatres
-   Shows
-   Customer profiles
-   Bookings and show-seat availability

## Getting Started

### Prerequisites

Install the following before running the project:

-   JDK compatible with the Java version configured in `Backend/pom.xml`
-   MySQL Server
-   Git
-   A code editor such as Visual Studio Code or IntelliJ IDEA

### 1. Clone the repository

``` bash
git clone https://github.com/almazkhan-dev/BookMyShow.git
cd BookMyShow
```

### 2. Configure the database

1.  Start your MySQL server.
2.  Create a database for the application, or use the database name
    configured in your local setup.
3.  Open `Backend/src/main/resources/application.properties`.
4.  Configure your local database URL, username, and password.

**Security:** Keep real database passwords, API keys, and other
credentials out of Git. Use local environment-specific configuration for
secrets. Do not commit those values to the repository.

### 3. Run the backend

Open a terminal in the project root and run:

``` bash
cd Backend
```

On Windows:

``` powershell
.\mvnw.cmd spring-boot:run
```

On macOS/Linux:

``` bash
./mvnw spring-boot:run
```

Alternatively, open the `Backend` folder in IntelliJ IDEA and run the
Spring Boot application class:

`BookMyShowBeApplication`

### 4. Run the frontend

Open `Frontend/index.html` in a browser, or use the Live Server
extension in Visual Studio Code.

If the frontend cannot communicate with the backend, check that the
backend is running and that the API base URL configured in
`Frontend/app.js` matches your local backend address.

## Development Notes

-   Keep backend configuration and frontend API URLs aligned with your
    local environment.
-   Do not commit passwords, tokens, or other secrets.
-   After making changes, test the affected backend APIs and frontend
    flows before committing.

## Future Improvements

Possible areas for further development include automated tests, improved
validation and error handling, deployment, and additional booking-flow
enhancements.

## Author

**Almaz Khan**

-   GitHub: [almazkhan-dev](https://github.com/almazkhan-dev)
-   Project repository:
    [BookMyShow](https://github.com/almazkhan-dev/BookMyShow)
