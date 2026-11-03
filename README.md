# MERN Starter Template

A modern, production-ready MERN (MongoDB, Express, React, Node.js) starter template featuring secure authentication, user profile management, avatar uploads with Cloudinary, and password reset capabilities.

## Tech Stack

- **Backend:** Node.js, Express 5, MongoDB / Mongoose, JWT, Bcrypt, Multer & Cloudinary
- **Frontend:** React 19, TypeScript, Tailwind CSS v4, React Router DOM, Zustand, Vite
- **Package Manager:** Bun

## Features

- **Authentication:** Secure Signup, Login, and JWT auth guards.
- **Password Management:** Forgot password & password reset flows.
- **User Profiles:** Profile viewing, updating usernames and names, and avatar image uploads powered by Cloudinary.
- **Modern UI/UX:** Built with Tailwind CSS and modern component architecture.

## Getting Started

### Prerequisites

- [Bun](https://bun.com) installed on your machine.
- MongoDB connection string.
- Cloudinary credentials (for avatar uploads).

### Installation

1. Clone the repository and install dependencies:

```bash
bun run install:all
```

2. Configure environment variables in `Backend/.env`:

```env
PORT=2002
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

### Running Development Servers

From the repository root, start both the backend and frontend with:

```bash
bun run dev
```

To run either one separately:

```bash
bun run dev:server
# or
bun run dev:client
```
