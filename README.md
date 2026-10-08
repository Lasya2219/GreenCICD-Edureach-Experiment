# EduReach Platform

EduReach Platform is a full-stack college intelligence and student support application with a React + TypeScript frontend and a Node.js + TypeScript backend.

## Project Structure

- client/ - Vite + React frontend
- server/ - Express + TypeScript backend
- server/knowledge-base/ - knowledge base content used by the backend RAG flow

## Features

- College and course discovery interface
- Student-facing homepage with sections for academics, events, mentors, and achievements
- Authentication flows for login and signup
- Chat and counseling UI components
- Backend API for auth, chat, and voice assistant integration
- Knowledge-base powered response support on the server

## Tech Stack

- Frontend: React, TypeScript, Vite
- Backend: Node.js, Express, TypeScript
- Database: MongoDB via Mongoose
- AI / RAG: LangChain and Google GenAI integrations
- Auth: JWT and bcryptjs

## Prerequisites

- Node.js 24 or newer for the server
- npm
- MongoDB connection string
- Google GenAI API key if you are using AI/chat features

## Setup

### 1. Clone the repository

```bash
git clone <your-github-repo-url>
cd edureach-platform
```

### 2. Install frontend dependencies

```bash
cd client
npm install
```

### 3. Install backend dependencies

```bash
cd ../server
npm install
```

### 4. Configure environment variables

Create a .env file inside server/ with the required values for your local setup.

Example:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GOOGLE_GENAI_API_KEY=your_google_genai_key
```

If the frontend also needs environment values, add a .env file inside client/ as needed.

## Running the App

### Frontend

```bash
cd client
npm run dev
```

### Backend

```bash
cd server
npm run dev
```

## Build

### Frontend

```bash
cd client
npm run build
```

### Backend

```bash
cd server
npm run build
```

## Linting

### Frontend

```bash
cd client
npm run lint
```

## Notes

- The client is a Vite-based single-page app.
- The server exposes auth, chat, and VAPI-related routes.
- The repository already includes a root .gitignore for common Node.js, build, and environment files.

## License

Add your license here if you want to publish the project publicly.
