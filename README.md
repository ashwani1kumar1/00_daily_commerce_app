# MERN Architecture (Bhopal Services Platform)

This project now uses MERN only:

- Frontend: React (Vite + React Router)
- Backend: Node.js + Express
- Database: MongoDB

## Project Structure

- frontend/ → React app (Vite + React Router)
- backend/ → Express + MongoDB service

## Run Frontend

1. Open terminal in `frontend`
2. Install dependencies: `npm install`
3. Start: `npm run dev`

## Run Backend

1. Open terminal in `backend`
2. Start MongoDB from workspace root: `docker compose up -d mongodb`
3. Create `.env` using [backend/.env.example](backend/.env.example)
4. Install dependencies: `npm install`
5. Start: `npm run dev`

## API Base URL (frontend)

Set in `frontend/.env`:

`VITE_API_BASE_URL=http://127.0.0.1:8000`

## Implemented Pages

- Login
- Home
- Services
- Providers
- Bookings
- Admin

## Implemented Platform Features

- JWT login flow from React to Express API
- MongoDB persistence for users, providers, bookings, payments
- Role-based API access (customer/provider/admin)
- Booking creation + booking listing by role
- UPI/Card payment intent + mark paid endpoint
- Admin analytics endpoint
