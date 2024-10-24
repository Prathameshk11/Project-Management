# Fullstack Project Management Application (MERN)

## Overview
The **Project Management Application** is a comprehensive solution for managing multiple projects and tasks, enabling teams to collaborate effectively. Built using the MERN stack (MongoDB, Express.js, React, and Node.js), the application provides features like project prioritization, team collaboration tools, and deadline management, fostering better productivity and organization.

## Features

### Admin Features:
1. **Project Management:**
   - Create, edit, and manage multiple projects.
   - Assign project priorities (high, medium, low).
   - Track project status and deadlines.

2. **User and Team Management:**
   - Add and manage team members.
   - Assign tasks to individual or multiple users.
   - Manage user roles and permissions (admin/user).

3. **Task Management:**
   - Assign, update, and manage tasks across different projects.
   - Set task statuses: to-do, in-progress, or completed.
   - Add and manage task priorities (high, medium, low).
   - Manage sub-tasks within larger tasks.

4. **Asset Management:**
   - Upload and manage project-related assets (images, documents, etc.).

### User Features:
1. **Project Interaction:**
   - View and track projects and their progress.
   - Interact with tasks: mark as in-progress or completed.
   - Collaborate with team members through comments on tasks.

2. **Task Management:**
   - View assigned tasks.
   - Track task status, deadlines, and priorities.

3. **Profile Management:**
   - Update personal profiles.
   - Change account password securely.

### General Features:
1. **Dashboard:**
   - Visualize project timelines and task progress.
   - Manage tasks based on project priorities.

2. **Authentication and Authorization:**
   - Secure login system.
   - Role-based access control (admin/user).

3. **Deadline and Progress Tracking:**
   - Automatic reminders for upcoming project deadlines.
   - Detailed progress tracking for individual projects and tasks.

## Technologies Used

### Frontend:
- **React** (Vite)
- **Redux Toolkit** for State Management
- **Headless UI** for building accessible components
- **Tailwind CSS** for styling

### Backend:
- **Node.js** with **Express.js**

### Database:
- **MongoDB** for efficient and scalable data storage

### Other Tools:
- **JWT (JSON Web Token)** for authentication
- **Cloudinary** (optional) for asset management

## Setup Instructions

### Server Setup

1. Create an `.env` file in the `server` folder with the following variables:
    ```bash
    MONGODB_URI=your MongoDB connection URL
    JWT_SECRET=your secret key
    PORT=8800 # or any port number
    NODE_ENV=development
    ```

2. Set up MongoDB:
    - Visit [MongoDB Atlas](https://www.mongodb.com/cloud/atlas), create an account, and configure a new cluster.
    - Create a new database and configure the `.env` file with the MongoDB connection URL.

3. To start the server:
    ```bash
    cd server
    npm install
    npm start
    ```
   You should see a message indicating that the server is running and the database is connected.

### Client Setup

1. Create an `.env` file in the `client` folder with the following variables:
    ```bash
    VITE_APP_BASE_URL=http://localhost:8800
    VITE_APP_FIREBASE_API_KEY=your Firebase API key (optional)
    ```

2. To run the client:
    ```bash
    cd client
    npm install
    npm start
    ```

3. Open [http://localhost:3000](http://localhost:3000) to view the application in your browser.

## Project Structure

- **client/**: Contains the React frontend.
- **server/**: Contains the Express backend.
- **utils/**: Utility functions, middlewares, and helpers.
- **models/**: Mongoose models for MongoDB.
- **controllers/**: Application logic for tasks, users, and projects.
- **routes/**: API routes for tasks, users, and projects.

## Future Enhancements

- Integration with **Cloudinary** for better asset management.
- Add **real-time notifications** for task updates.
- Implement **task reminders** for due dates.
- Improve the **dashboard UI** for better data visualization.
- Add **Kanban view** for task management.



---

**Developed by:** [Prathamesh Khokaralkar]
