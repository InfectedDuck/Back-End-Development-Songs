# Flask Music API

## Overview

This project is a Flask-based REST API for managing a music collection. It provides endpoints for CRUD operations on songs stored in a MongoDB database. The API includes features for health checks, counting records, retrieving all songs, fetching a song by ID, creating, updating, and deleting songs.

## Features

* **Health Check**: Endpoint to verify the API is running.
* **Count Records**: Endpoint to get the total number of songs in the database.
* **Retrieve All Songs**: Fetch all songs from the database.
* **Retrieve Song by ID**: Get details of a specific song using its ID.
* **Create Song**: Add a new song to the database.
* **Update Song**: Modify details of an existing song.
* **Delete Song**: Remove a song from the database.

## Getting Started

### Prerequisites

* **Python**: Ensure Python 3.x is installed.
* **Flask**: Install Flask using pip.
* **pymongo**: Install pymongo using pip.

### Configuration

Set the following environment variables for MongoDB connection:

- **`MONGODB_SERVICE`**: MongoDB server address.
- **`MONGODB_USERNAME`**: MongoDB username (if authentication is used).
- **`MONGODB_PASSWORD`**: MongoDB password (if authentication is used).
- **`MONGODB_PORT`**: MongoDB port (optional).

### API Endpoints

- **GET `/health`**:  
  Returns the health status of the API.

- **GET `/count`**:  
  Returns the total number of songs in the database.

- **GET `/song`**:  
  Retrieves all songs.

- **GET `/song/<int:id>`**:  
  Retrieves a song by ID.

- **POST `/song`**:  
  Creates a new song.

- **PUT `/song/<int:id>`**:  
  Updates an existing song.

- **DELETE `/song/<int:id>`**:  
  Deletes a song by ID.
