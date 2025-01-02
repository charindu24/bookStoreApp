
# Book Store  App

This is a full-stack web application built with the MERN stack (MongoDB, Express, React, Node.js) designed to manage a book store. The project integrates Firebase for user authentication and MongoDB for storing book and user data. It includes both the frontend (React) and backend (Node.js/Express) applications.

---

## Table of Contents
1. Installation
2. Frontend Setup
3. Backend Setup
4. Environment Variables
5. Running the Project
6. License

---

## Installation

To get started with the project, clone the repository to your local machine:

```bash
git clone https://github.com/charindu24/bookStoreApp.git
cd bookStoreApp
```

Once the project is cloned, follow the setup instructions for both the frontend and backend.

---

## Frontend Setup

### Prerequisites
- Node.js and npm must be installed. You can download and install them from the [official Node.js website](https://nodejs.org/).

### Steps to Run the Frontend

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Create a `.env.local` file in the root directory (where `package.json` is located) and add the following environment variables for Firebase:

   

3. Install Node dependencies:
   ```bash
   npm install
   ```

4. Start the frontend application:
   ```bash
   npm run dev
   ```

   This will launch the frontend on your local development server.

---

## Backend Setup

### Prerequisites
- You need a MongoDB Atlas account or a local MongoDB setup.
- Node.js and npm installed.

### Steps to Run the Backend

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Install Node dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory (same level as `package.json`) and add the following environment variables:

   ```env
   DB_URL = "mongodb+srv://charinducdb:BookStore11122@bookstoreapp.raarh.mongodb.net/bookStore?retryWrites=true&w=majority&appName=bookStoreApp"

JWT_SECRET_KEY='dbcef1d0b78007d346541268576af649ff910e9725eb85c26593662930854b36583cbb81bcd6e76259fd6d8ab98b7cdaaed0e07130916f0744a94cb4e1de680f'


   ```

   - **DB_URL**: Your MongoDB connection string (for MongoDB Atlas or local MongoDB setup).
   - **JWT_SECRET_KEY**: A secure secret key used for signing JSON Web Tokens (JWTs).

4. Start the backend application:
   ```bash
   npm run start:dev
   ```

   The backend server will start running and listen for API requests.

---

## Environment Variables

### Frontend (.env.local):
VITE_API_KEY="AIzaSyD6F9AC5gbvAt7melvG9yuUuE8kPeEnSC0"
VITE_AUTH_DOMAIN="book-storeapp.firebaseapp.com"
VITE_PROJECT_ID="book-storeapp"
VITE_STORAGE_BUCKET="book-storeapp.firebasestorage.app"
VITE_MESSAGING_SENDERID="828038357486"
VITE_APP_ID="1:828038357486:web:eba253b4708cd40478aeff"

### Backend (.env):
- `DB_URL`: MongoDB connection URL (MongoDB Atlas or local MongoDB URL).
- `JWT_SECRET_KEY`: A secret key for signing JWT tokens for secure authentication.

---

## Running the Project

1. Clone or unzip the project folder.
2. Follow the setup instructions for both frontend and backend as described above.
3. Run the frontend by navigating to the frontend directory and running:
   ```bash
   npm run dev
   ```
4. Run the backend by navigating to the backend directory and running:
   ```bash
   npm run start:dev

locally backend npm start
   ```

Your application should now be up and running locally.

---

## License

This project is licensed under the MIT License - see the LICENSE file for details.
