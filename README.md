# URL-shorten-in-one-click
This is the code for shorten the long url
Here's a basic `README.md` file for your URL shortener project:

---

# URL Shortener Project

## Overview

This is a simple URL shortener application built using Node.js, Express.js, and MongoDB. The project allows users to shorten URLs, manage them, and serves static files to enable a frontend interface.

## Features

- Shorten long URLs.
- Redirect shortened URLs to their original destinations.
- Serve static frontend files.
- Integration with MongoDB for persistent storage.

## Requirements

Before starting, ensure you have the following installed:

- [Node.js](https://nodejs.org/en/) (v14 or higher)
- [MongoDB](https://www.mongodb.com/)

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/url-shortener.git
cd url-shortener
```

### 2. Install dependencies

Run the following command to install the necessary dependencies:

```bash
npm install
```

### 3. Set up MongoDB

Make sure your MongoDB is up and running. You will need to connect to your MongoDB instance in the `db.js` file.

### 4. Running the Project

To start the server, use the following command:

```bash
npm start
```

The application will be running on `http://localhost:3000`.

### 5. Endpoints

- **POST /shorten**: Shortens a given URL.
- **GET /:shortURL**: Redirects to the original URL.

### 6. Serving Static Files

The application serves static files from the `public` folder. Ensure you place your frontend files there.

## Folder Structure

```bash
|-- public/            # Static frontend files
|-- routes/            # URL routes handling logic
|-- db.js              # MongoDB connection logic
|-- app.js             # Main application logic
```

## Middleware

- **body-parser**: Parses incoming request bodies in JSON format.
- **express.static**: Serves static files (e.g., HTML, CSS, JavaScript) from the `public` directory.

## License

This project is licensed under the MIT License.

---

You can customize this file further based on any additional features or instructions you want to include!
