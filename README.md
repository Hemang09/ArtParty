ArtParty ✨🎨
<div align="center"> <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React" /> <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js" /> <img src="https://img.shields.io/badge/Socket.IO-010101?style=for-the-badge&logo=socket.io&logoColor=white" alt="Socket.IO" /> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" /> <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" /> </div> <div align="center"> <h3>🎨 Real-time multiplayer drawing and guessing game inspired by Skribbl.io</h3> <p>Draw, guess, and celebrate creativity with friends in real time!</p> <h2>🧩 <a href="https://github.com/Hemang09/ArtParty" target="_blank">GitHub Repository</a></h2> </div>
🌟 Features

🎨 Interactive Drawing Canvas – Smooth drawing with mouse or touch support

📹 Video Chat – See and talk to your friends while you play

🗣️ Voice Input & Feedback – Use speech for chatting and receiving updates

🔄 Smart Reconnection – 30-second grace period to rejoin without losing progress

⏱️ Timed Rounds & Turns – Stay on your toes with countdown timers

🏆 Dynamic Scoring System – Earn points for quick guesses and creative drawings

👥 Private Rooms – Create password-protected lobbies for your friends

🔐 JWT Authentication – Secure token-based user sessions

📱 Responsive Design – Play seamlessly on desktop, tablet, or mobile

⚡ Real-time Communication – Instant updates via WebSockets

🖌️ Customizable Drawing Tools – Choose colors, brush sizes, and clear the canvas

💡 Smart Hints – Get helpful hints if you’re stuck too long

🎮 How to Play

Create or Join a private room with a password

Wait for Players – Minimum 2 players required

Take Turns Drawing – Pick one of three word options on your turn

Guess the Word – Type your guesses in the chat

Earn Points – The faster you guess, the more you score!

Win the Game – The player with the most points after all rounds wins

🎯 Scoring
Action	Points
First to guess	120
Second to guess	110
Third to guess	100
Late guess	80
Drawer bonus	+50 (when someone guesses)
Drawer penalty	-60 (if nobody guesses)
🛠️ Tech Stack
Frontend

React 18 + TypeScript

Socket.IO Client for real-time events

HTML5 Canvas for drawing functionality

Ant Design for components

Tailwind CSS for styling

Backend

Node.js + Express

Socket.IO for WebSocket communication

MongoDB + Mongoose for persistence

JWT for authentication

bcrypt for password security

🚀 Getting Started
Prerequisites

Node.js (v18+ recommended)

MongoDB (local or Atlas)

npm

Installation

Clone the repository

git clone https://github.com/Hemang09/ArtParty.git
cd ArtParty


Install backend dependencies

cd backend
npm install


Install frontend dependencies

cd ../frontend
npm install


Setup environment variables

Create a .env file inside backend/:

PORT=3000
JWT_SECRET=your_super_secret_jwt_key_here
MONGODB_URI=mongodb://localhost:27017/artparty
FRONTEND_URL=http://localhost:5173
NODE_ENV=development


Run the application

Backend (Terminal 1):

cd backend
npm run dev


Frontend (Terminal 2):

cd frontend
npm run dev


Open in browser

http://localhost:5173

📁 Project Structure
ArtParty/
├── backend/
│   ├── controllers/     # API and socket controllers
│   ├── handlers/        # Socket event handlers
│   ├── middleware/      # Auth & validation
│   ├── models/          # MongoDB schemas
│   ├── routes/          # Express routes
│   ├── services/        # Game logic & state management
│   └── utils/           # Helpers and constants
├── frontend/
│   ├── src/
│   │   ├── components/  # UI components
│   │   ├── pages/       # Game pages and views
│   │   └── utils/       # Frontend utilities
│   └── public/
└── README.md

🎨 Canvas Features

Drawing Tools: Pencil, eraser, and color picker

Brush Sizes: Adjustable (1–20px)

Color Palette: 12 presets + custom picker

Clear Canvas: Reset drawing instantly

Real-time Sync: Everyone sees updates instantly

🔧 Configuration

Edit backend/utils/gameConfig.js to adjust game behavior:

export const GAME_CONFIG = {
  MIN_PLAYERS: 2,
  MAX_PLAYERS: 8,
  TOTAL_ROUNDS: 3,
  TURN_TIME: 80, // seconds
  PREPARATION_TIME: 5, // seconds
  WORD_SELECTION_TIME: 10, // seconds
};

❤️ Acknowledgements

Inspired by Skribbl.io
 — built to bring friends together for creativity, laughter, and art.