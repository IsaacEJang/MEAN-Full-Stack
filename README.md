# Full Stack Using MEAN

## Overview

Travlr Getaways is a full-stack web application built using the MEAN stack (MongoDB, Express.js, Angular, and Node.js). It allows users to browse and book vacation packages while enabling administrators to manage travel listings, bookings, and customer interactions through a Single Page Application (SPA).


## User Webiste (Node.js & Express)
![User Interface](https://github.com/user-attachments/assets/04d48650-078a-4b55-94fe-2fd3d5c1477b)

## Admin Website (Angular)
![Admin Site](https://github.com/user-attachments/assets/5a0a2366-4f26-4a04-98d5-95107169ff57)


## Architecture

### Frontend Development

In this project, we utilized multiple types of frontend development: 
- **Express HTML**: Offered basic templating capabilities to render pages, which was initially used during development to quickly set up server-side rendered pages.
- **JavaScript**: Provided client-side interactivity, particularly when making asynchronous requests to the server for a more dynamic user experience.
- **SPA with Angular**: Unlike traditional multi-page applications, the SPA dynamically loads content without reloading the page, providing a seamless, fast, and interactive user experience.

The SPA approach was chosen for its ability to improve user experience by reducing page load times and creating a more dynamic interface, while Express HTML was used for early development and server-side rendering when needed.

### Backend Development & NoSQL

We opted for **MongoDB**, a NoSQL database, for its flexibility in handling large volumes of unstructured data. Unlike relational databases, MongoDB’s schema-less structure allowed us to evolve the database without complex migrations, which is crucial for scaling the application as the number of users and bookings increases.

## Functionality

### JSON vs JavaScript

While **JavaScript** is the language for scripting web pages, **JSON** (JavaScript Object Notation) is a data format used for sending structured data between the frontend and backend. JSON is lightweight and easy for both humans and machines to read, making it ideal for transmitting data across the web. In this project, JSON enabled the backend (Express) to communicate with the frontend (Angular) by sending and receiving data in a structured format, bridging the two layers.

### Refactoring for Efficiency

During development, we refactored the **trip browsing components** into reusable UI components. For instance, the trip cards displaying different destinations were consolidated into a single reusable component, making future updates easier. The benefits of this approach include:
- **Code reusability**: Write once, use anywhere.
- **Maintenance efficiency**: Changes in the UI could be made in one place and reflected across the application.
- **Consistent user experience**: Ensured that the trip cards behaved consistently throughout the application.

## Testing

API testing in full-stack applications ensures the reliability of request and retrieval methods. We performed **unit tests** for individual API endpoints, which included testing GET and POST requests for booking management. The added layer of **JWT-based authentication** added complexity to testing, as the API requests needed to include valid tokens. Security testing involved validating that only authorized users could access specific endpoints, preventing unauthorized data access.

### Methods, Endpoints, and Security

- **Methods**: HTTP methods such as GET, POST, PUT, and DELETE were tested for correctness.
- **Endpoints**: Testing was performed on `/api/trips`, `/api/bookings`, and user authentication endpoints.
- **Security**: Authentication was handled using JWT tokens to secure communication between the frontend and backend.

## Reflection

This course has been instrumental in advancing my skills as a full-stack developer. I have learned how to build scalable web applications using modern frameworks such as Angular and Express. Additionally, I’ve developed a deeper understanding of API development and testing, which will make me a more marketable candidate in the software engineering field. The hands-on experience with the MEAN stack has not only refined my programming skills but also strengthened my ability to design scalable, secure, and user-friendly web applications.
