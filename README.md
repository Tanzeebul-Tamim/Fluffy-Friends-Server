# Fluffy Friends - Server Side

Welcome to the server-side repository of Fluffy Friends, a soft toy marketplace. This server handles API requests and manages database functionalities.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Prerequisites](#prerequisites)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Configuration](#configuration)
- [Live Server](#live-server)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Also checkout Fluffy-Friends-Client](#also-checkout-fluffy-friends-client)
- [Contributing](#contributing)

## Features

- CRUD operations for toys.
- Database interactions using MongoDB.
- Environment-based configuration.
- Search and sort functionality for toys.

## Technologies Used

- Node.js
- Express.js
- MongoDB

## Prerequisites

- Node.js and npm installed.
- MongoDB installed and running.

## Project Structure

```
├── .gitignore          # Lists files for Git to ignore
├── README.md           # Project documentation
├── index.js            # Main entry point of the application
├── package-lock.json   # Exact dependency tree
├── package.json        # Project metadata and dependencies
├── vercel.json         # Vercel deployment settings
```

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Tanzeebul-Tamim/Fluffy-Friends-Server
    cd Fluffy-Friends-Server
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

## Configuration

Create a `.env` file in the root directory and add the following environment variables:

```
PORT=5000
DB_USER=your_db_user
DB_PASS=your_db_password
MONGODB_URI=your_mongodb_connection_string
```

## Live Server

The server is deployed on [this following URL](https://toy-marketplace-server-puce-ten.vercel.app/)

## Running the Application

- Start the server:
    ```bash
    npm start
    ```

## API Endpoints

- ***GET*** `/allToys`: Get all toys (supports search and pagination)
- ***GET*** `/totalToys`: Get total count of toys
- ***GET*** `/allToys/email/:email`: Get toys by seller email (supports sorting)
- ***GET*** `/allToys/id/:id`: Get a single toy by ID
- ***POST*** `/allToys`: Add a new toy
- ***PATCH*** `/allToys/id/:id`: Update toy details
- ***DELETE*** `/allToys/id/:id`: Delete a toy

## Also checkout Fluffy-Friends-Client
Visit the client-side repository of [Fluffy Friends](https://github.com/Tanzeebul-Tamim/Fluffy-Friends-Client) website
## Contributing

Feel free to contribute by submitting a pull request. Please ensure that your code follows the project's coding standards and includes relevant tests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
