# Blog Web Application

## Assignment Overview

This assignment is designed to assess your problem-solving abilities, logical thinking, and full-stack development skills. You will create a basic web application where users can log in, view a list of blogs, and edit a blog post. Ensure that only one user can edit a blog at a time.

### Setup the Project

1. Initialize a Node.js project.
2. Set up Express.js and MongoDB connection.
3. Set up React application.

### User Authentication

1. Create a user model and authentication routes (register, login).
2. Implement JWT for secure authentication.
3. Ensure routes are protected and accessible only to authenticated users.

### Blog Management

1. Create a blog model with fields: `title`, `content`, `lastEditedBy`, `isLocked`, `lockedBy`, `lockedAt`.
2. Implement routes to get a list of blogs, get blog details, and edit a blog.
3. Ensure that only one user can edit a blog at a time using a locking mechanism.
4. Implement a feature to unlock a blog after a certain period of inactivity.

### Frontend Implementation

1. Create a login page.
2. Implement a page to list blogs.
3. Implement a blog edit page with a locking mechanism.
4. Show appropriate messages if a blog is locked by another user.

### Bonus

1. Implement unit tests for backend routes.
2. Use Redux for state management in the frontend.

## Deliverables

1. A GitHub repository with two folders: `backend` and `frontend`.
2. `.env` file (if any).
3. Detailed instructions on how to run the application locally.
4. A short write-up explaining your approach, any challenges faced, and how you solved them.

## Setup Instructions

### Backend

1. Navigate to the `backend` folder extract the folder.
2. Run `npm install` to install dependencies.
3. a `.env` file has MongoDB connection string and JWT secret.
4. Run `npm run dev` to start the server in development mode.

### Frontend

1. Navigate to the `frontend` folder extract the folder.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the React application.

### Approach

- **Backend**: Built RESTful APIs using Express.js and implemented JWT for authentication. Created a locking mechanism in the blog model to manage concurrency.
- **Frontend**: Developed React components for login, blog listing, and blog editing. Integrated with backend APIs to handle authentication and blog operations.

### Challenges

- **Concurrency Control**: Ensuring that the locking mechanism is effective and handles edge cases such as network failures or timeouts.
- **State Management**: Handling the state of the blog editing process to ensure that the UI reflects the current state accurately.
