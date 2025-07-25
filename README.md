# Book World

A full-featured book review and management application built with the MERN stack (`MongoDB`, `Express`, `React`, `Node.js`). Users can browse books, leave reviews with star ratings, and manage their favorites. Admins have extended capabilities for adding, editing, and deleting books.

## Features

- **User Authentication:**

  - Secure user registration and login system.
  - JWT for authorization.

- **Book Listing with Reviews & Ratings:**

  - Browse and search for books.
  - Leave comprehensive reviews with star ratings.
  - Read and gain insights from community reviews.

- **User Profile Pages:**

  - Personalized profiles to track activity.
  - Manage and curate a list of favorite books.

- **Advanced Feature:**

  - Unique nested commenting system using Depth-First Search (DFS) for efficient comment deletion within the review tree structure.

- **User Roles & Permissions:**
  - Admin capabilities to add, update, and delete book listings.

## Technologies Used

- **Frontend:**

  - React.js
  - Recoil for State Management
  - Tailwind CSS
  - Shadcn UI library
  - React Hook Form
  - Lucide-React for icons

- **Backend:**

  - Node.js
  - Express.js
  - MongoDB
  - Mongoose for MongoDB object modeling
  - CORS for Cross-Origin Resource Sharing
  - JWT for token-based authentication
  - Bcrypt for secure password storage

- **Other Dependencies:**
  - Axios
  - Zod for schema validation
  - React Router DOM for routing

## Installation Guide

### Requirements

- Node.js
- MongoDB

You can use use Mongo Atlas URL instead of local MongoDB

### Configure Environment Variables

Rename .env.example to .env in both backend and frontend directories.

Add your `MONGO_URL`, `JWT_SECRET`, `CLOUD_NAME`, `CLOUD_API_KEY`, `CLOUD_API_SECRET`, and `PORT` to the backend .env files.

If you don't have Cloudinary, you can replace `cloudStorage` with `diskStorage` in `/backend/middleware/upload.js`.

### Installation

#### Clone the Repository

```shell
git clone https://github.com/Vasisthayadav2123/book-Review
cd book-world
```

#### Install packages

```shell
cd book-world
cd backend
npm install
cd ..
cd frontend
npm install
```

#### Start Frontend

Make sure you are in `frontend` directory

```shell
npm run dev
```

#### Start Backend

Make sure you are in `backend` directory

```shell
node index.js
```

Now open `localhost:5173` on your browser

#### special thanks to NEET64 for the boilerplate code. 🙏