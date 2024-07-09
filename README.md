#URL Shortener Project

-Overview

The URL Shortener project is a web application built using Node.js and Express.js, designed to shorten long URLs into more manageable and shareable links. The project uses MongoDB as the database to store URL mappings and user information. Authentication and authorization are implemented using JSON Web Tokens (JWT) to ensure secure access to user-specific functionalities.

-Key Features

1. User Registration and Authentication

* Users can register with a unique email and password.
* Passwords are hashed and stored securely in the database.
* Registered users can log in to access their account.
  
2. JWT-Based Authentication

* Upon successful login, a JWT is generated and returned to the user.
* This token is used for subsequent authenticated requests.
* Middleware is used to verify the token and protect routes that require authentication.
  
3. URL Shortening

* Authenticated users can submit long URLs to be shortened.
* The application generates a unique short URL and stores the mapping in MongoDB.
* Users can view a list of their shortened URLs.
  
4. Redirection

* When a short URL is accessed, the application redirects the user to the original long URL.
* URL access statistics can be tracked (e.g., number of clicks).

5. User-Specific URL Management

* Users can view, edit, and delete their shortened URLs.
* Each user's data is protected, ensuring that only the owner can manage their URLs.
  
-Technologies Used

-> Node.js: Server-side JavaScript runtime.

-> Express.js: Web framework for Node.js, used to build the API and handle HTTP requests.

->MongoDB: NoSQL database to store URL mappings and user data.

-> Mongoose: ODM (Object Data Modeling) library for MongoDB and Node.js, used to interact with the database.

-> JWT (JSON Web Tokens): Used for secure user authentication and authorization.
