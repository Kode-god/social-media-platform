# MERN Social Media Application 

A full-stack social media platform built with the MERN stack (MongoDB, Express, React, Node.js), featuring user authentication, post creation, comments, likes, and profile management.



##  Features
- **User Authentication**: Register, login, and JWT-based session management
- **Post Management**: Create, view, and interact with posts
- **Social Interactions**: Like posts and add comments
- **User Profiles**: View and update profiles with avatars
- **Responsive Design**: Works on all device sizes

## Technologies
- Frontend: React, Vite, Material-UI
- Backend: Node.js, Express, MongoDB
- Authentication: JSON Web Tokens (JWT)
- Deployment: Render (Backend), Vercel (Frontend)

## Installation
### Prerequisites
- Node.js v18+
- MongoDB Atlas account
- Git

### Backend Setup
bash
git clone repo name
cd backend
npm install

# Create .env file
echo "MONGO_URI=your_mongodb_atlas_uri
JWT_SECRET=your_jwt_secret
PORT=5000" > .env

npm start


### Frontend Setup
bash
Copy
cd ../frontend
npm install
npm run dev


### API Documentation
Authentication
Endpoint	Method	Description	Request Body Example

/api/auth/register	POST	User registration	{ username, email, password }

/api/auth/login	POST	User login	{ email, password }

Posts
Endpoint	Method	Description

/api/posts	GET	Get all posts

/api/posts	POST	Create new post

/api/posts/:id/like	POST	Like/unlike post

Users
Endpoint	Method	Description
/api/users/me	GET	Get current user
/api/users/:id	GET	Get user profile
