# Backend Ledger

A backend ledger system built using Node.js, Express, MongoDB, and JWT authentication. The project demonstrates secure user authentication, account management, immutable ledger entries, and transaction processing similar to real-world financial systems.

## Features

* User Registration and Login using JWT Authentication
* Secure Logout with Token Blacklisting
* Account Creation and Retrieval
* Balance Calculation using Ledger Entries
* Double-Entry Ledger System (Credit/Debit)
* Idempotent Transaction Processing
* MongoDB Transactions using Sessions
* Email Notifications using Nodemailer and Gmail OAuth2

## Tech Stack

* Node.js
* Express.js
* MongoDB Atlas
* Mongoose
* JWT (jsonwebtoken)
* Nodemailer
* bcryptjs

## Installation

```bash
git clone <repository-url>
cd backend-ledger
npm install
```

Create a `.env` file and add the required environment variables.

## Run the Project

```bash
npm run dev
```

The server will start on:

```
http://localhost:5000
```

## API Endpoints

### Authentication

* POST `/api/auth/register`
* POST `/api/auth/login`
* POST `/api/auth/logout`

### Accounts

* POST `/api/accounts`
* GET `/api/accounts`
* GET `/api/accounts/balance/:accountId`

### Transactions

* POST `/api/transactions`
* POST `/api/transactions/system/initial-funds`

## Notes

This project was tested using Postman and MongoDB Atlas.
