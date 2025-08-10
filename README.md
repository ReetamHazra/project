# Food Recipe Project

A full-stack web application for sharing, browsing, and managing food recipes. This project consists of a Node.js/Express backend and a React frontend, designed to provide a seamless experience for users to discover, add, edit, and view recipes.

## Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [API Endpoints](#api-endpoints)
- [Screenshots](#screenshots)
- [License](#license)

## Features
- User authentication (register, login)
- Add, edit, and delete recipes
- Upload and display recipe images
- Browse and search recipes
- View detailed recipe information
- Responsive and modern UI

## Tech Stack
- **Frontend:** React, Vite, CSS
- **Backend:** Node.js, Express
- **Database:** MongoDB (via Mongoose)

## Project Structure
```
backend/
  config/           # Database connection
  controller/       # Route controllers (user, recipe)
  middleware/       # Authentication middleware
  models/           # Mongoose models (user, recipe)
  public/images/    # Uploaded recipe images
  routes/           # Express routes (user, recipe)
  server.js         # Entry point for backend
frontend/food-blog-app/
  src/
	 assets/         # Images and static assets
	 components/     # Reusable React components
	 pages/          # Main app pages (Home, Add, Edit, Details)
	 App.jsx         # Main React app
	 main.jsx        # Entry point
  public/           # Static files
  vite.config.js    # Vite configuration
```

## Getting Started

### Prerequisites
- Node.js & npm
- MongoDB instance (local or cloud)

### Backend Setup
1. Navigate to the backend folder:
	```sh
	cd backend
	```
2. Install dependencies:
	```sh
	npm install
	```
3. Configure your MongoDB connection in `config/connectionDb.js`.
4. Start the backend server:
	```sh
	node server.js
	```

### Frontend Setup
1. Navigate to the frontend app folder:
	```sh
	cd frontend/food-blog-app
	```
2. Install dependencies:
	```sh
	npm install
	```
3. Start the frontend development server:
	```sh
	npm run dev
	```

## API Endpoints
- `POST /api/user/register` — Register a new user
- `POST /api/user/login` — User login
- `GET /api/recipe` — Get all recipes
- `POST /api/recipe` — Add a new recipe
- `GET /api/recipe/:id` — Get recipe details
- `PUT /api/recipe/:id` — Edit a recipe
- `DELETE /api/recipe/:id` — Delete a recipe

## Screenshots
Add screenshots of your app here (UI, features, etc.)

## License
This project is licensed under the MIT License.