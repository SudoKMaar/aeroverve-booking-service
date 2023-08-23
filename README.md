# AeroVerve - Booking Microservice

AeroVerve is a microservice-based airline booking system designed to provide a seamless flight booking experience to users. This microservice handles flight bookings, payments, and cancellations. It's part of the larger AeroVerve project, contributing to its functionality.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Architecture](#architecture)
- [Contributing](#contributing)
- [License](#license)

## Introduction

AeroVerve Airline Booking Microservice is a part of the AeroVerve project, a comprehensive airline booking system utilizing microservices and MVC architecture. This microservice focuses on flight bookings, payments, and cancellations.

## Features

- Create flight bookings with user and flight details.
- Process payments securely and efficiently.
- Handle booking cancellations and manage seat availability.
- Integrate with a message queue for notifications.
- Utilize a scheduled task to manage booking expiration.

## Getting Started

### Prerequisites

- Node.js and npm installed.
- A working database (e.g., MySQL, PostgreSQL) with necessary credentials.
- RabbitMQ or another message queue server set up for notifications.

### Installation

1. Clone this repository to your local machine.

   ```bash
   git clone https://github.com/SudoKMaar/aeroverve-booking-service.git
   ```

2. Navigate to the project directory.

   ```bash
   cd aeroverve-booking-service
   ```

3. Install dependencies.

   ```bash
   npm install
   ```

4. Configure environment variables.

   - Create a `.env` file based on `.env.example` and set necessary environment variables.

5. Run database migrations.

   ```bash
   npx sequelize-cli db:migrate
   ```

6. Start the microservice.

   ```bash
   npm start
   ```

## Usage

1. The microservice provides endpoints to create flight bookings, process payments, and manage cancellations.
2. Use the API documentation to understand the available endpoints and request/response formats.
3. Ensure that the message queue is correctly set up to receive booking notifications.
4. Scheduled tasks are in place to manage booking expirations.

## Architecture

AeroVerve follows a microservice-based architecture, utilizing the MVC pattern. Key components include:

- **Controllers:** Handle incoming requests, process data, and invoke services.
- **Services:** Contain the core business logic, interacting with repositories and external services.
- **Repositories:** Manage database operations, encapsulating data access logic.
- **Message Queue:** Used for sending notifications about booking events.
- **Scheduled Tasks:** Manage booking expiration and other time-based operations.

## Contributing

We welcome contributions to AeroVerve! To contribute, follow these steps:

1. Fork the repository.
2. Create a new branch for your feature/fix.
3. Implement your changes.
4. Commit your changes and push to your fork.
5. Create a pull request to the main repository.

## License

This project is licensed under the [MIT License](LICENSE).

---

AeroVerve - Elevating Flight Booking Experiences
