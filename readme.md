# WanderJoy - Interactive Online Travel Booking Website

## Overview

WanderJoy is an interactive travel booking website built using the **MERN** (MongoDB, Express.js, React, Node.js) stack. It efficiently manages **1,000+ travel listings** and handles up to **500 concurrent user requests**, offering a seamless experience for users searching and booking travel destinations.

![DashboardWanderJoy](https://github.com/user-attachments/assets/f31fc0e5-b008-4612-8b61-6118411f9f84)


## Features

- **User Authentication:** Secure sign-up/login system with JWT authentication.
- **Browse Listings:** View and filter through 1,000+ travel destinations.
- **Advanced Search & Filtering:** Search by location, price, rating, and amenities.
- **User Reviews & Ratings:** Allow users to rate and review their travel experiences.
- **Admin Dashboard:** Manage listings, users, and bookings.

## Tech Stack

### Frontend

- **React.js** (UI Components, State Management)
- **Redux/Context API** (State Management)
- **Tailwind CSS/Bootstrap** (Responsive Design)

### Backend

- **Node.js** (Server-side runtime)
- **Express.js** (Web framework)
- **MongoDB** (NoSQL Database)
- **Mongoose** (ODM for MongoDB)
- **JWT & Bcrypt.js** (Authentication & Security)

### Other Technologies

- **Stripe API** (Secure payment processing)
- **AWS S3 / Cloudinary** (Image storage)
- **Nginx / PM2** (Production deployment)

## Installation

### Prerequisites

Ensure you have the following installed:

- **Node.js** (v14+)
- **MongoDB** (Local or cloud instance)
- **npm/yarn**

### Steps to Run Locally

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-repo/wanderjoy.git
   cd wanderjoy
   ```

2. **Install Dependencies**

   ```bash
   # Install frontend dependencies
   cd client
   npm install

   # Install backend dependencies
   cd ../server
   npm install
   ```

3. **Set Up Environment Variables**

   - Create a `.env` file in the `server` directory and configure the following:
     ```env
     PORT=5000
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_secret_key
     STRIPE_SECRET=your_stripe_key
     CLOUDINARY_URL=your_cloudinary_url
     ```

4. **Run the Application**

   ```bash
   # Start Backend
   cd server
   npm run dev

   # Start Frontend
   cd ../client
   npm start
   ```

5. **Access the App**

   - Open [http://localhost:3000](http://localhost:3000) in your browser.

## Deployment

### Frontend

- **Vercel / Netlify**
  ```bash
  npm run build
  vercel deploy
  ```

### Backend

- **Deploy using PM2 & Nginx on VPS**
  ```bash
  pm2 start server.js
  ```
- **Deploy to Heroku**
  ```bash
  git push heroku main
  ```

## Contributing

1. **Fork the Repository**
2. **Create a Branch**
   ```bash
   git checkout -b feature-branch
   ```
3. **Commit Changes**
   ```bash
   git commit -m "Added new feature"
   ```
4. **Push & Create PR**
   ```bash
   git push origin feature-branch
   ```


