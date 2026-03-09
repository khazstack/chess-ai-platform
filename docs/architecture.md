# Architecture — Chess AI Platform

## 1. Overview

The system consists of four main components:

- Frontend
- Backend API
- Chess Engine Service
- Database

These components work together to provide chess gameplay and AI-based analysis.

---

## 2. Frontend

The frontend is the user interface of the platform.

Responsibilities:

- Display the chess board
- Handle user interaction
- Show move history
- Load and display games
- Send requests to backend API
- Display analysis results

Technology:

- Next.js
- TypeScript
- chess.js
- Chessground

---

## 3. Backend API

The backend processes requests from the frontend.

Responsibilities:

- User authentication
- Game management
- Saving games
- Loading game history
- Communicating with the chess engine
- Sending analysis results

Technology:

- FastAPI
- Python

---

## 4. Chess Engine Service

The engine service performs chess analysis using Stockfish.

Responsibilities:

- Analyze positions
- Calculate best move
- Provide evaluation scores
- Return principal variations

Technology:

- Stockfish
- python-chess

---

## 5. Database

The database stores all persistent data.

Stored data:

- Users
- Games
- Moves
- Analysis results

Technology:

- PostgreSQL

---

## 6. System Flow

User interacts with the frontend.

Frontend sends requests to the backend API.

Backend processes requests and stores data in the database.

For analysis, backend communicates with the chess engine service.

The result is returned to the frontend and displayed to the user.
