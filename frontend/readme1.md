# 🎬 MoodFlix – AI-Powered Mood-Based Movie Recommendation System

**MoodFlix** is a full-stack web application that recommends movies based on your current and desired mood, combining optional AI emotion detection with real-time movie metadata and streaming availability.

---

## 🚀 Tech Stack

### Frontend
* **React (Vite)** – Fast modern React framework
* **TailwindCSS** – Utility-first styling with Dark/Light mode support
* **Framer Motion** – Smooth UI transitions and micro-animations
* **React Router** – Client-side routing and protected views

### Backend
* **Node.js & Express.js** – RESTful API server
* **MongoDB & Mongoose** – NoSQL database and ODM
* **JWT & bcrypt** – Secure token-based authentication and password hashing

### AI / ML & External APIs
* **TensorFlow.js / face-api.js** – Optional webcam-based mood detection
* **TMDb API** – Movie metadata, posters, ratings, and genre filtering
* **JustWatch API** – Real-time streaming platform availability

---

## 📋 Key Features

* ✅ **User Authentication** – Secure registration and login with JWT & bcrypt
* ✅ **Mood Selection Interface** – Interactive mood picker with smooth Framer Motion animations
* ✅ **Mood-Based Movie Recommendations** – Dynamic recommendations mapped to user mood
* ✅ **AI Mood Detection (Optional)** – Real-time facial emotion recognition via webcam
* ✅ **Watchlist Management** – Save, view, and remove movies from a personal watchlist
* ✅ **Movie Rating System** – Rate movies and view aggregated user ratings
* ✅ **Admin Dashboard** – Manage users, movies, and user feedback
* ✅ **Responsive UI & Theme Toggle** – Seamless Dark/Light mode across desktop and mobile

---

## 📁 Project Structure

```text
moodflix/
├── backend/                 # Backend Express server
│   ├── src/
│   │   ├── config/          # Database and environment configuration
│   │   ├── controllers/     # Route business logic
│   │   ├── middleware/      # Auth & error handling middleware
│   │   ├── models/          # Mongoose schemas (User, Watchlist, Rating)
│   │   ├── routes/          # Express API route definitions
│   │   ├── utils/           # Helper functions & API clients
│   │   └── server.js        # Backend entry point
│   ├── .env.example         # Backend environment variable template
│   └── package.json
│
├── frontend/                # Frontend React + Vite application
│   ├── src/
│   │   ├── components/      # Reusable UI components
│   │   ├── context/         # React Context providers (Auth, Theme)
│   │   ├── hooks/           # Custom React hooks
│   │   ├── pages/           # Application pages
│   │   ├── services/        # Axios/Fetch API service layer
│   │   ├── styles/          # Global CSS and Tailwind setup
│   │   ├── utils/           # Frontend helpers & AI detection utils
│   │   └── main.jsx         # Frontend entry point
│   ├── .env.example         # Frontend environment variable template
│   └── package.json
│
└── README.md