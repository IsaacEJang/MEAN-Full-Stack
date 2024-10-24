# Travlr Getaways

## Overview

Travlr Getaways is a full-stack web application built using the MEAN stack (MongoDB, Express.js, Angular, and Node.js). It allows users to browse and book vacation packages while enabling administrators to manage travel listings, bookings, and customer interactions through a Single Page Application (SPA).

## Architecture

The system is divided into three main components:

1. **Client**: User-facing interface built with Angular, providing a seamless browsing and booking experience.
2. **Server**: Handles business logic, authentication, and data processing via Express.js.
3. **Database**: MongoDB stores all essential travel and booking data, interfacing with the server through Mongoose.

## Technology Stack

- **Frontend**: Angular
- **Backend**: Node.js with Express.js
- **Database**: MongoDB
- **Authentication**: JWT-based authentication for secure logins.

## Features

- **Trip Browsing**: Users can browse available trips, view details, and book vacations.
- **Admin Dashboard**: Admins can add, update, and delete trips through an intuitive dashboard.
- **User Authentication**: Secure login and registration for users and admins.
- **Bookings Management**: Full CRUD operations for handling trip bookings.

## API Endpoints

| Method | Purpose                   | URL                         | Description                                   |
|--------|---------------------------|-----------------------------|-----------------------------------------------|
| GET    | Retrieve list of trips     | `/api/trips`                | Returns all available trips                   |
| GET    | Retrieve a single trip     | `/api/trips/:tripId`        | Fetches details of a specific trip            |
| POST   | Create a new booking       | `/api/bookings`             | Allows a customer to book a trip              |
| PUT    | Update booking             | `/api/booking/:bookingId`   | Updates an existing booking                   |
| DELETE | Delete booking             | `/api/booking/:bookingId`   | Cancels a specific booking                    |
| POST   | User Authentication        | `/api/users/authenticate`   | Authenticates user login                      |

## Class Diagram

The class structure for Travlr Getaways includes:

- **Itinerary**: Stores trip details like total cost, miles, and stops.
- **TripInfo**: Adds specific trip information to the itinerary.
- **CruiseInfo/FlightInfo/HotelInfo**: Stores details for different travel types.
- **Booking Classes**: Manages reservation details for flights, hotels, and cruises.
- **TravelerInfo**: Stores personal information for customized travel experiences.
- **Membership Classes**: Manages user membership status and loyalty points.

## Deployment

To run the application locally:

1. Clone the repository: `git clone <repo-url>`
2. Navigate to the project directory: `cd travlr-getaways`
3. Install dependencies: `npm install`
4. Start the server: `npm start`
5. Access the application at `http://localhost:4200`

---

