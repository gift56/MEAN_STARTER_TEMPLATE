# MEAN Stack Task Manager Template

Welcome to the **MEAN Stack Task Manager Template**! This project is a professional starter kit for building scalable full-stack applications using **M**ongoDB, **E**xpress.js, **A**ngular, and **N**ode.js.

## 🚀 Overview

This template provides a solid foundation for developing modern web applications with a separation of concerns between the client-side (Angular) and server-side (Node.js/Express). It includes a configured setup for connecting to MongoDB and serving a RESTful API.

## 🛠️ Tech Stack

- **MongoDB**: NoSQL database for flexible data storage.
- **Express.js**: Fast, unopinionated, minimalist web framework for Node.js.
- **Angular**: Platform for building mobile and desktop web applications.
- **Node.js**: JavaScript runtime environment for the server.

## 📋 Prerequisites

Ensure you have the following installed on your local development machine:

- [Node.js](https://nodejs.org/) (LTS version recommended)
- [Angular CLI](https://angular.io/cli): `npm install -g @angular/cli`
- MongoDB: Ensure the MongoDB service is running locally or have a connection string for a cloud instance.

## 📂 Project Structure

The project is organized into two main directories:

- `backend/`: Contains the Node.js/Express server code, API routes, and database models.
- `client/`: Contains the Angular frontend application source code.

## ⚡ Getting Started

Follow these steps to get the application up and running.

### 1. Clone the Repository

```bash
git clone [[<your-repo-url>]()](https://github.com/gift56/MEAN_STARTER_TEMPLATE.git)
cd tMEAN_STARTER_TEMPLATE
```

### 2. Setup Backend

Navigate to the backend directory, install dependencies, and start the server.

```bash
cd backend
npm install
```

**Configuration:**
Create a `.env` file in the `backend` folder (if not already present) to configure your environment variables (e.g., Database URI, Port).

**Start Server:**
```bash
npm start
# OR for development with auto-reload (requires nodemon)
npm run dev
```
*The backend server will typically run on `http://localhost:3000`.*

### 3. Setup Client

Open a new terminal, navigate to the client directory, install dependencies, and start the Angular development server.

```bash
cd ../client
npm install
ng serve
```
*The frontend application will run on `http://localhost:4200`.*

## 🏃‍♂️ Running Backend and Client Together

To streamline development, you can run both the backend and client from a single command if you configure `concurrently` in the root directory.

1.  **Install concurrently in the root:**
    ```bash
    npm install concurrently --save-dev
    ```

2.  **Add scripts to root `package.json`:**
    ```json
    "scripts": {
      "dev": "concurrently \"npm run start --prefix backend\" \"npm run start --prefix client\""
    }
    ```

3.  **Run the app:**
    ```bash
    npm run dev
    ```

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## 📄 License

This project is licensed under the MIT License.