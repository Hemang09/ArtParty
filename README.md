<p align="center">
  <img src="https://raw.githubusercontent.com/Hemang09/ArtParty/main/frontend/public/logo.png" width="150" alt="ArtParty Logo">
</p>

<p align="center">
  <a href="#-overview">Overview</a> • 
  <a href="#-features">Features</a> • 
  <a href="#-installation">Installation</a> • 
  <a href="#-how-to-play">How to Play</a> • 
  <a href="#-license">License</a>
</p>

# 🎨 ArtParty  
### A Real-Time Multiplayer Drawing and Guessing Game  
Built with **React**, **Node.js**, **Socket.IO**, **TypeScript**, and **MongoDB**

---

## 🌈 Overview

**ArtParty** is a fun, real-time multiplayer drawing and guessing game inspired by Skribbl.io!  
Draw, guess, and compete with your friends to see who’s the best artist and quickest thinker — all in real time.

---

## 🌟 Features

- 🎨 **Interactive Drawing Canvas** – Smooth drawing experience with mouse and touch support  
- 📹 **Video Chat** – See and talk to your friends while playing  
- 🗣️ **Voice Input & Feedback** – Use your voice for chatting and real-time updates  
- 🔄 **Smart Reconnection** – 30-second grace period to rejoin a game without losing progress  
- ⏱️ **Timed Rounds & Turns** – Fast-paced, exciting gameplay with countdowns  
- 🏆 **Dynamic Scoring System** – Rewarding both quick guessers and skilled artists  
- 👥 **Private Rooms** – Password-protected lobbies for friends  
- 🔐 **JWT Authentication** – Secure token-based user sessions  
- 📱 **Responsive Design** – Works perfectly on desktop, tablet, or mobile  
- ⚡ **Real-Time Communication** – Instant updates via WebSockets  
- 🖌️ **Customizable Drawing Tools** – Choose colors, brush sizes, and clear your canvas  
- 💡 **Smart Hints** – Automatic hints if you’re stuck too long  

---

## 🎮 How to Play

1. **Create or Join** a game room (optionally protected by a password)  
2. **Wait for Players** – Minimum of 2 players required to start  
3. **Take Turns Drawing** – Choose from 3 random word options when it’s your turn  
4. **Guess the Word** – Type your guesses in the chat box  
5. **Earn Points** – The faster you guess, the higher your score  
6. **Win the Game** – The player with the highest score after all rounds wins  

---

## 🎯 Scoring System

| Action | Points |
|--------|--------:|
| 🥇 First to guess | 120 |
| 🥈 Second to guess | 110 |
| 🥉 Third to guess | 100 |
| ⏰ Late guess | 80 |
| ✏️ Drawer bonus (if guessed) | +50 |
| ❌ Drawer penalty (if no one guesses) | -60 |

---

## 🛠️ Tech Stack

### **Frontend**
- ⚛️ React 18 with TypeScript  
- 🔌 Socket.IO Client for real-time communication  
- 🖼️ HTML5 Canvas API for drawing functionality  
- 💎 Ant Design for UI components  
- 🎨 Tailwind CSS for styling  

### **Backend**
- 🟢 Node.js with Express  
- 🔌 Socket.IO for WebSocket communication  
- 🗄️ MongoDB with Mongoose for data persistence  
- 🔐 JWT for authentication  
- 🧂 bcrypt for password hashing  

---

## 🚀 Getting Started

### **Prerequisites**
Make sure you have the following installed:
- Node.js (v18+ recommended)  
- MongoDB (local or Atlas)  
- npm  

---

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/Hemang09/ArtParty.git
   cd ArtParty
   ```

2. **Install backend dependencies**

   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies**

   ```bash
   cd ../frontend
   npm install
   ```

4. **Setup environment variables**

   Create `.env` in the backend directory:

   ```env
   PORT=3000
   JWT_SECRET=your_super_secret_jwt_key_here
   MONGODB_URI=mongodb://localhost:27017/artparty
   FRONTEND_URL=http://localhost:5173
   NODE_ENV=development
   ```

5. **Run the application**

   **Backend** (Terminal 1):

   ```bash
   cd backend
   npm run dev
   ```

   **Frontend** (Terminal 2):

   ```bash
   cd frontend
   npm run dev
   ```

6. **Open your browser**

   Navigate to `http://localhost:5173`

## 📁 Project Structure

```
ArtParty/
├── backend/
│   ├── controllers/     # Route controllers
│   ├── handlers/        # Socket event handlers
│   ├── middleware/      # Auth & validation middleware
│   ├── models/          # MongoDB models
│   ├── routes/          # Express routes
│   ├── services/        # Game logic & state management
│   └── utils/           # Helper functions
├── frontend/
│   ├── src/
│   │   ├── components/  # Reusable UI components
│   │   ├── pages/       # Main page components
│   │   └── utils/       # Frontend utilities
│   └── public/
└── README.md
```

## 🎨 Canvas Features

- **Drawing Tools**: Pencil, eraser, color picker
- **Brush Sizes**: Adjustable stroke width (1-20px)
- **Color Palette**: 12 preset colors + custom color picker
- **Clear Canvas**: Reset drawing area
- **Real-time Sync**: All players see drawings instantly

## 🔧 Configuration

### Game Settings

You can modify game settings in `backend/utils/gameConfig.js`:

```javascript
export const GAME_CONFIG = {
  MIN_PLAYERS: 2,
  MAX_PLAYERS: 8,
  TOTAL_ROUNDS: 3,
  TURN_TIME: 80, // seconds
  PREPARATION_TIME: 5, // seconds
  WORD_SELECTION_TIME: 10, // seconds
};
```
## 📝 License

This project is licensed under the **Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License**.

- ✅ You may share and redistribute the material
- ❌ You may not use this project for commercial purposes
- ❌ You may not modify or create derivative works
- ✅ You must give appropriate credit

See the [LICENSE](https://creativecommons.org/licenses/by-nc-nd/4.0/) for details.

## 📞 Contact

**Hemang** - [@Hemang](https://github.com/Hemang09)

Project Link: [https://github.com/Hemang09/ArtParty](https://github.com/Hemang09/ArtParty)

---

<div align="center">
  <p>Made with ❤️ by <a href="https://github.com/Hemang09/ArtParty">Hemang09</a></p>
  <p>⭐ Star this repo if you like it!</p>
</div>

