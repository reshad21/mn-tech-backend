# Mntech digital assignment tusk

## Overview

This is the backend of the Mntech digital system. It provides RESTful API endpoints to manage users, purches product. The system supports user authentication, authorization, and transaction management, ensuring secure and reliable operations.

## Features

- **User Authentication & Authorization:** Sign up, login, and role-based access control (admin and user).
- **Bike Management:** Admins can add, update, and delete product from the system.
- **Booking Management:** Users can rent product, and the system tracks bookings, costs, and returns.
- **Error Handling:** Comprehensive error handling for all operations.
- **Database Transactions:** Ensures consistency and rollback in case of failures during critical operations.

## Technology Stack

- **Node.js**: Backend runtime environment.
- **Express.js**: Web framework for building the RESTful API.
- **MongoDB**: NoSQL database for storing users, product, and bookings.
- **Mongoose**: ODM (Object Data Modeling) library for MongoDB.
- **JWT**: JSON Web Tokens for user authentication.
- **bcrypt**: Library for hashing passwords.
- **Zod**: Schema validation library.

# API Endpoints

## User Routes

- **Sign Up:** `POST /api/auth/signup`  
  Register a new user.

- **Login:** `POST /api/auth/login`  
  Authenticate a user and return a token.

- **Get Profile:** `GET /api/users/me`  
  Retrieve the profile of the logged-in user.

- **Update Profile:** `PUT /api/users/me`  
  Update the profile of the logged-in user.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/bike-rental-reservation-system.git
   cd bike-rental-reservation-system
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## Environment Variables

Create a `.env` file in the root directory and configure the following environment variables:

```env
PORT=5000
MONGO_URI=mongodb://localhost:5000/bike-rental
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=1d
```
