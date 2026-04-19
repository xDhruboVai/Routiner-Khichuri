# Routiner Khichuri

Routiner Khichuri is a web application for generating clash-free class routines based on course selection, faculty preferences, section availability and schedule constraints.

Live site: https://routiner-khichuri.vercel.app/

## Features

- Clash-free routine generation (class and exam conflict checks)
- Faculty preference and avoid filters
- Preferred section selection
- Ignored time slots and allowed-day filtering
- Seat-status aware filtering for sections

## Tech Stack

- Frontend: React, Vite
- Backend: Node.js, Express
- Data fetching: Axios

## Project Structure

```text
.
├── backend
│   ├── src
│   │   ├── scheduler.js
│   │   └── server.js
│   └── package.json
├── frontend
│   ├── src
│   ├── public
│   └── package.json
└── package.json
```

## Getting Started

### 1) Install dependencies

From the repository root:

```bash
npm install
```

Install workspace dependencies:

```bash
cd backend && npm install
cd ../frontend && npm install
```

### 2) Run in development

From the repository root:

```bash
npm run dev
```

This starts both backend and frontend concurrently.

Default local URLs:

- Backend: http://localhost:4000
- Frontend: http://localhost:5173

## Data Source and Acknowledgment

Course data is fetched from the Eniamza CDN endpoint:

- https://usis-cdn.eniamza.com/connect.json

Special thanks to Eniamza for providing and maintaining this CDN:

- https://github.com/Eniamza

## Scripts

### Root

- npm run dev: Start backend and frontend together

### Backend

- npm run dev: Start backend with nodemon
- npm run start: Start backend with node

### Frontend

- npm run dev: Start Vite dev server
- npm run build: Build production assets
- npm run preview: Preview production build
- npm run lint: Run ESLint
