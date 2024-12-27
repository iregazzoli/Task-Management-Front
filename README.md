Task Management

This repository contains the frontend section for task management, developed using NestJS for the backend and React for the frontend.

## Project Structure

- **Frontend**: It is built with React and uses Yarn as the package manager.
- **Backend**: It is built using NestJS and uses NPM as the package manager and can be found [here](https://github.com/iregazzoli/Task-Management-Server).

## Prerequisites

- Node.js (v16 or later versions)
- Yarn (for frontend) and NPM (for backend)

## Getting Started

### Frontend Setup

1. Navigate to the frontend directory:

   ```bash
   cd task-management-frontend

   ```

2. Install the frontend dependencies using Yarn:

   ```bash
   yarn install
   ```

3. Start the frontend development server:

   ```bash
   yarn start
   ```

   The frontend will be available at `http://localhost:3001`.

### Backend Setup

1. Navigate to the backend directory:

   ```bash
   cd ../task_management
   ```

2. Install the backend dependencies using NPM:

   ```bash
   npm install
   ```

3. Start the backend development server:

   ```bash
   npm run start:dev
   ```

   The backend will be available at `http://localhost:3000`

---

## Backend Database Setup

To configure the backend to connect to the database, you need to set up the appropriate environment variables. The database credentials are stored in the `.env.stage.dev` file.

### Steps to Configure Database Credentials

1. Navigate to the backend directory:

   ```bash
   cd task_management
   ```

2. Open the `.env.stage.dev`, this file contains environment variables that configure the backend's connection to the database.

3. Set the following environment variables in the `.env.stage.dev` file:

   ```ini
   DB_HOST=
   DB_PORT=
   DB_USERNAME=
   DB_PASSWORD=
   DB_DATABASE=
   JWT_SECRET=<jwt_secret_keye>
   ```

---

## Example `.env.stage.dev` file

```ini
DB_HOST=localhost
DB_PORT=5432
DB_USERNAME=postgres
DB_PASSWORD=postgres
DB_DATABASE=task-management
JWT_SECRET=Secret51
```

---

Now, you should be ready to run the backend with the correct database credentials and JWT secret key.

## Running Both Frontend & Backend Simultaneously

For development purposes, you can run both the frontend and backend servers simultaneously:

- Frontend: `yarn start` (in the `task-management-frontend` directory)
- Backend: `npm run start:dev` (in the `task_management` directory)

---
