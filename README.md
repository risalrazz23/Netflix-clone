# Netflix Clone

A full-stack web application mimicking some of the core functionalities and UI of Netflix, built with the MERN stack (MongoDB, Express.js, React, Node.js) and Tailwind CSS.

## Features

*   User authentication (sign-up, login, logout - noting that login/logout backend is WIP).
*   Landing page showcasing features like "Enjoy on your TV", "Download your shows", "Watch everywhere", "Create profiles for kids".
*   FAQ section on the landing page.

## Tech Stack

**Frontend:**
*   React
*   Redux
*   React Router
*   Tailwind CSS
*   NextUI
*   Vite

**Backend:**
*   Node.js
*   Express.js
*   MongoDB (with Mongoose)
*   JSON Web Tokens (JWT) for authentication
*   bcryptjs for password hashing

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

*   Node.js (which includes npm) installed on your machine.
*   MongoDB installed and running.

### Backend Setup

1.  **Clone the repository (if you haven't already):**
    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```
2.  **Navigate to the root project directory.**
3.  **Install NPM packages:**
    ```bash
    npm install
    ```
4.  **Create a `.env` file in the `backend` directory.**
    Add the following environment variables. Replace `<your_mongodb_connection_string>` and `<your_jwt_secret>` with your actual values.
    ```env
    MONGO_URI=<your_mongodb_connection_string>
    JWT_SECRET=<your_jwt_secret>
    PORT=8000
    ```
5.  **Start the backend server:**
    ```bash
    npm run dev
    ```
    The backend server should now be running, typically on `http://localhost:8000`.

### Frontend Setup

1.  **Navigate to the frontend directory:**
    ```bash
    cd frontend
    ```
2.  **Install NPM packages:**
    ```bash
    npm install
    ```
3.  **Start the frontend development server:**
    ```bash
    npm run dev
    ```
    The frontend development server should now be running, typically on `http://localhost:5173`. Open this URL in your browser to see the application.

## Project Structure

```
.
├── backend/                    # Backend (Node.js/Express.js)
│   ├── config/                 # Configuration files (database, environment variables)
│   ├── controllers/            # Request handlers for different routes
│   ├── models/                 # Mongoose schemas for MongoDB
│   ├── routes/                 # API route definitions
│   └── server.js               # Main backend server entry point
├── frontend/                   # Frontend (React)
│   ├── public/                 # Static assets (images, videos)
│   ├── src/
│   │   ├── assets/             # Frontend specific assets (images, logos)
│   │   ├── components/         # Reusable UI components
│   │   ├── constants/          # Constant values (e.g., text for accordions)
│   │   ├── pages/              # Top-level page components (AuthScreen, HomePage, SignUpPage)
│   │   ├── redux/              # Redux store and related files
│   │   ├── App.jsx             # Main React application component
│   │   ├── main.jsx            # React application entry point
│   │   └── index.css           # Global CSS styles
│   ├── .eslintrc.cjs           # ESLint configuration
│   ├── package.json            # Frontend dependencies and scripts
│   ├── tailwind.config.js      # Tailwind CSS configuration
│   └── vite.config.js          # Vite configuration
├── .gitignore                  # Git ignore file
├── package.json                # Backend dependencies and scripts (root level)
└── README.md                   # This file
```

### Key Directories:

*   **`backend/`**: Contains all the server-side code.
    *   **`controllers/`**: Logic for handling requests.
    *   **`models/`**: Database schemas.
    *   **`routes/`**: API endpoint definitions.
*   **`frontend/`**: Contains all the client-side React application code.
    *   **`components/`**: Reusable UI elements.
    *   **`pages/`**: Main views of the application.
    *   **`redux/`**: State management setup.
