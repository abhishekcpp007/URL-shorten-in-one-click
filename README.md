

---

# ShortURL - URL Shortener Application

## Overview

ShortURL is a simple URL shortener built using Node.js, Express.js, and MongoDB with Mongoose for data persistence. This application allows users to shorten long URLs, store them in a MongoDB database, and redirect shortened URLs to their original destinations.

## Features

- Shorten long URLs with ease.
- Redirect shortened URLs to the original links.
- MongoDB as the primary database for storing URLs.
- Lightweight and easy to set up.

## Requirements

Ensure you have the following installed before running the project:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [MongoDB](https://www.mongodb.com/) (locally or on a cloud service)
- [Nodemon](https://www.npmjs.com/package/nodemon) (for development)

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/shorturl.git
cd shorturl
```

### 2. Install Dependencies

Install the necessary Node.js dependencies by running the following command:

```bash
npm install
```

### 3. Set up Environment Variables

Create a `.env` file in the root of the project with your MongoDB URI and any other environment variables. Here's an example:

```
MONGODB_URI=mongodb://localhost:27017/shorturl
PORT=3000
```

### 4. Start the Server

To start the server in development mode (with auto-restart using Nodemon):

```bash
npm run dev
```

The server will be running on `http://localhost:3000`.

### 5. API Endpoints

- **POST /shorten** - Create a shortened URL from a long URL.
- **GET /:shortUrl** - Redirect the shortened URL to the original long URL.

## Folder Structure

```bash
|-- src/
|   |-- routes/           # Route handling
|   |-- server.js         # Entry point of the application
|-- .env                  # Environment variables
|-- package.json          # Dependencies and scripts
```

## Scripts

- **`npm run dev`**: Runs the application in development mode using Nodemon, automatically restarting the server on file changes.

## Dependencies

- **express**: Web framework for building the server.
- **body-parser**: Middleware to parse incoming request bodies.
- **dotenv**: Loads environment variables from a `.env` file.
- **mongodb**: MongoDB driver for Node.js.
- **mongoose**: MongoDB object modeling tool for schema-based data handling
