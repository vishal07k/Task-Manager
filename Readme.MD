# Task Manager Application

## Overview
The **Task Manager** is a web application built using **Express.js** and **MongoDB** with an **HTML** frontend. It allows users to register, log in, and manage their tasks efficiently. Users can create, edit, and delete tasks through a user-friendly interface.

## Features
- **User Authentication**: Register and log in with secure authentication.
- **Task Management**:
  - Add new tasks.
  - Edit existing tasks.
  - Delete tasks.
  - View all tasks in a list.
- **Responsive UI**: A simple and clean HTML frontend for easy interaction.

## Technologies Used
- **Backend**: Node.js, Express.js, MongoDB
- **Frontend**: HTML, CSS, JavaScript
- **Authentication**: bcrypt.js (for password hashing), express-session
- **Database**: MongoDB (Mongoose ODM)

## Installation and Setup

### Prerequisites
Ensure you have the following installed:
- **Node.js** (v14 or later)
- **MongoDB** (Running locally or using a cloud service like MongoDB Atlas)

### Steps to Set Up
1. **Clone the Repository**
   ```sh
   git clone https://github.com/vishal07k/Task-Manager.git
   cd task-manager
   ```
2. **Install Dependencies**
   ```sh
   npm install
   ```
3. **Set Up Environment Variables**
   Create a `.env` file in the root directory and add the following:
   ```env
   PORT=3000
   MONGO_URI=mongodb://localhost:27017/task_manager
   SESSION_SECRET=your_secret_key
   ```
4. **Run the Application**
   ```sh
   npm start
   ```
   The server will start on `http://localhost:3000`

## Folder Structure
```
/task-manager
│-- /public         # Static files (CSS, JS)
│-- /views          # HTML files
│-- /routes         # Express routes
│-- /models         # Mongoose models
│-- server.js       # Main server file
│-- package.json    # Project dependencies
│-- .env            # Environment variables
```

## API Endpoints
### User Authentication
- `POST /register` - Register a new user
- `POST /login` - Log in an existing user
- `GET /logout` - Log out user

### Task Management
- `GET /tasks` - View all tasks
- `POST /tasks` - Add a new task
- `PUT /tasks/:id` - Edit a task
- `DELETE /tasks/:id` - Delete a task

## Future Enhancements
- Add task categories and priorities.
- Implement user role management (Admin/User).
- Add email notifications for task deadlines.

## License
This project is licensed under the MIT License.

## Contact
For any issues or contributions, please reach out at **your-khamkarvishal6@example.com** or create a GitHub issue.

