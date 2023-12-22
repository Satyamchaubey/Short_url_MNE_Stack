URL Shortener Project
Introduction
This project aims to build a URL shortening service using Node.js, Express.js, and MongoDB. It enables users to submit lengthy URLs, generates unique shortened versions, and tracks the number of clicks on these shortened URLs.

Installation
Clone this repository.
Install dependencies using npm install.
Getting Started
Run MongoDB locally or specify the database URL in mongoose.connect().
Start the server using npm start.
Access the application on http://localhost:5000.
Project Structure
server.js: Contains the server setup and API endpoints.
/models/shortUrl.js: Defines the MongoDB schema for storing URLs.
/views/index.ejs: Frontend view with form to shorten URLs and display of shortened URLs.
Dependencies
Express.js: Web framework for Node.js.
Mongoose: MongoDB object modeling for Node.js.
EJS: Templating engine for server-side HTML rendering.
Shortid: Library for generating unique short IDs.
API Endpoints
GET '/': Renders the homepage with a form to submit URLs and a list of shortened URLs.
POST '/shortUrls': Handles URL submission, generates short URL, and stores in the database.
GET '/:shortUrl': Redirects users to the original URL based on the short URL provided.

File Structure:

- /
  - server.js
  - /models
    - shortUrl.js
  - /views
    - index.ejs

Usage
Access the application on the provided URL.
Submit a lengthy URL in the provided form.
Receive a shortened URL for sharing.
Click on the shortened URL to be redirected to the original URL.
Development
Use npm run start to start the server.
Use nodemon server.js for development with automatic restart on file changes.
Additional Notes
Ensure MongoDB is running locally or update the database URL in mongoose.connect().
