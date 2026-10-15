# BiteLoop

**Author:** Tayaba

BiteLoop is a food discovery app built around short-form video. Users can browse food videos, like and save posts, while food partners can create a profile and share videos of their food.

## Features

- Browse a vertical feed of food videos
- Register and log in as a user or food partner
- Like and save food videos
- Create food posts as a food partner
- Visit food partner profiles

## Tech Stack

- Frontend: React, Vite, React Router, Axios
- Backend: Node.js, Express
- Database: MongoDB with Mongoose
- Media storage: ImageKit

## Getting Started

### Requirements

- Node.js and npm
- A MongoDB connection URI
- An ImageKit account for media uploads

### Configure the backend

In PowerShell, from the project root:

```powershell
Copy-Item backend/.env.example backend/.env
```

Set these values in `backend/.env`:

```env
JWT_SECRET=your_jwt_secret
MONGODB_URI=your_mongodb_connection_uri
IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
```

Install dependencies and start the backend:

```powershell
cd backend
npm install
node server.js
```

The backend runs at `http://localhost:3000`.

### Start the frontend

In a second terminal, from the project root:

```powershell
cd frontend
npm install
npm run dev
```

Open the local URL printed by Vite, usually `http://localhost:5173`.

## Project Structure

```text
backend/   Express API, MongoDB models, authentication, and media upload
frontend/  React application and Vite configuration
vdeos/     Project video assets
```

## Author

Created by Tayaba.
