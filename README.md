# Full Stack Using MEAN

## Overview

Travlr Getaways is a full-stack web application built using the MEAN stack (MongoDB, Express.js, Angular, and Node.js). It allows users to browse and book vacation packages while enabling administrators to manage travel listings, bookings, and customer interactions through a Single Page Application (SPA).


## Screenshots

| Pages | View |
|--------------------------|------------|
| **User Website (Node.js & Express):** <br /><br /> This page shows the user interface built with Node.js and Express. | ![User Interface](https://github.com/user-attachments/assets/04d48650-078a-4b55-94fe-2fd3d5c1477b) |
| **Admin Website (Angular):** <br /><br /> This page shows the admin interface built with Angular. | ![Admin Site](https://github.com/user-attachments/assets/5a0a2366-4f26-4a04-98d5-95107169ff57) |



## Architecture

### Frontend Development

In this project, I used a combination of Express HTML, JavaScript, and Angular for the frontend:
- **Express HTML**: I initially used this for server-side rendering during development, which allowed me to quickly set up pages.
- **JavaScript**: Provided the client-side interactivity, allowing me to make asynchronous requests to the server.
- **SPA with Angular**: I transitioned to using Angular’s SPA architecture because it offers a more seamless user experience. Unlike traditional multi-page apps, the SPA reduces load times by dynamically updating content without reloading the page.

### Backend & NoSQL Database

For the backend, I opted for **MongoDB**, a NoSQL database, because it provides flexibility in handling large volumes of unstructured data. Unlike traditional relational databases, MongoDB’s schema-less design allowed me to evolve the data structure without complex migrations, which will be crucial as the application scales.

## Functionality

### JSON vs JavaScript

While **JavaScript** powers client-side scripting, **JSON** (JavaScript Object Notation) is used to send structured data between the frontend and backend. In this project, JSON played a crucial role in allowing the Angular frontend to communicate with the Express backend, exchanging data such as trip details and booking information.

### Refactoring for Efficiency

As the project progressed, I refactored several parts of the code to improve functionality and efficiency. For example, I turned trip listing components into reusable UI elements, which allowed me to create a consistent design across different parts of the app while minimizing redundancy. Refactoring also made it easier to maintain and update the application in the long run.

## Testing

To ensure the reliability of the application, I performed various types of API testing. This included:
- **Unit testing** the API endpoints for booking management, which involved testing the methods for retrieving and posting data (GET and POST requests).
- **Security testing** to ensure that only authorized users could access specific endpoints. This added complexity to the testing process, especially with the use of **JWT authentication**, where valid tokens were required for access.

### Methods, Endpoints, and Security

- **Methods**: I tested HTTP methods like GET, POST, PUT, and DELETE to ensure they performed the correct operations on data.
- **Endpoints**: Testing focused on the `/api/trips`, `/api/bookings`, and `/api/users` endpoints.
- **Security**: Using **JWT-based authentication**, I ensured that API requests were secure, with protected routes for logged-in users only.

## Reflection

This project and course have significantly helped me progress toward my professional goals. I’ve gained a deeper understanding of full-stack development, specifically using modern frameworks like Angular and Express. Building and testing a scalable web application has improved my programming skills and strengthened my ability to design secure, efficient solutions. These new skills make me a stronger candidate in the software engineering field, and I’m excited to apply them to real-world challenges.

---
