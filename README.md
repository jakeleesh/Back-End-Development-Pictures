# Get Pictures Microservice

A Flask-based REST API for managing URLs of pictures from past events of a popular band. This microservice allows users to perform CRUD operations on picture URLs and serves as one of the microservices in a larger band website application.

---

## Table of Contents

- [About the Project](#about-the-project)
  - [Key Features](#key-features)
  - [Solution Architecture](#solution-architecture)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
  - [Installation](#installation)
- [Usage](#usage)
- [Development and Deployment](#development-and-deployment)

---

## About the Project

The **Get Pictures Microservice** is responsible for:
- Storing URLs of pictures from past concerts.
- Exposing RESTful APIs to interact with picture resources.
- Providing health status endpoints for monitoring.

This microservice is part of a multi-service application built for a popular music band.

### Key Features

- **CRUD APIs**: Create, Read, Update, and Delete picture URLs.
- **Health Endpoint**: Monitor the health of the microservice.
- **Test-Driven Development**: Includes pre-written unit tests.

### Solution Architecture

- **Frontend**: Consumes picture data via API.
- **Backend**: Flask REST API with endpoints for picture management.
- **Deployment**: Hosted on IBM Code Engine.

---

## Tech Stack

- **Framework**: Flask
- **Database**: SQLite (for temporary storage)
- **Testing**: pytest
- **Deployment**: IBM Code Engine

---

## Getting Started

### Installation

1. Install virtual environment:
   ```bash
   cd /Back-End-Development-Pictures
   bash ./bin/setup.sh
   ```

2. Start
   ```bash
   flask run --debugger --reload
   curl --request GET --url http://localhost:5000/health
   ```

---

## Usage

- GET `/picture`: Retrieve all pictures.
- GET `/picture/<id>`: Retrieve a picture URL by ID.
- POST `/picture`: Add a new picture URL.
- PUT `/picture/<id>`: Update a picture URL by ID.
- DELETE `/picture/<id>`: Delete a picture URL by ID.

---

## Development and Deployment

### Testing

- Run tests using pytest

### Deployment

- Build and push Docker image.
- Deploy using IBM Code Engine.
