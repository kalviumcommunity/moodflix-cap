# 🎬 MoodFlix – AI-Powered Mood-Based Movie Recommendation System

A full-stack web application that recommends movies based on your current and desired mood, using AI emotion detection and public movie APIs.

## 🚀 Tech Stack

### Frontend
- **React** with **Vite** - Modern React framework
- **TailwindCSS** - Utility-first CSS framework
- **Framer Motion** - Animation library
- **React Router** - Client-side routing

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **MongoDB** with **Mongoose** - Database and ODM
- **JWT** - Authentication tokens
- **bcrypt** - Password hashing

### AI/ML
- **TensorFlow.js** or **face-api.js** - Mood detection (optional)

### APIs
- **TMDb API** - Movie database
- **JustWatch API** - Streaming availability

## 📁 Project Structure

```
moodflix/
├── backend/                 # Backend server
│   ├── src/
│   │   ├── config/         # Configuration files
│   │   ├── controllers/    # Route controllers
│   │   ├── models/         # Mongoose models
│   │   ├── routes/         # API routes
│   │   ├── middleware/     # Custom middleware
│   │   ├── utils/          # Utility functions
│   │   └── server.js       # Entry point
│   ├── .env.example        # Environment variables template
│   └── package.json
│
├── frontend/               # Frontend application
│   ├── src/
│   │   ├── components/     # Reusable components
│   │   ├── pages/          # Page components
│   │   ├── context/        # React Context providers
│   │   ├── hooks/          # Custom React hooks
│   │   ├── services/       # API services
│   │   ├── utils/           # Utility functions
│   │   ├── styles/         # Global styles
│   │   └── main.jsx        # Entry point
│   ├── .env.example        # Environment variables template
│   └── package.json
│
└── README.md
```

## 🛠️ Setup Instructions

### Prerequisites
- Node.js (v18 or higher)
- MongoDB (local or Atlas)
- npm or yarn

### Backend Setup

1. Navigate to backend directory:
```bash
cd backend
```

2. Install dependencies:
```bash
npm install
```

3. Create `.env` file (copy from `.env.example`):
```bash
cp .env.example .env
```

4. Configure environment variables in `.env`:
```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/moodflix
JWT_SECRET=your-super-secret-jwt-key-change-this
JWT_EXPIRE=7d
TMDB_API_KEY=your-tmdb-api-key
NODE_ENV=development
```

5. Start the server:
```bash
npm run dev
```

The backend will run on `http://localhost:5000`

### Frontend Setup

1. Navigate to frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Create `.env` file (copy from `.env.example`):
```bash
cp .env.example .env
```

4. Configure environment variables in `.env`:
```env
VITE_API_URL=http://localhost:5000/api
```

5. Start the development server:
```bash
npm run dev
```

The frontend will run on `http://localhost:5173`

## 📋 Features

- ✅ User Authentication (Signup/Login with JWT)
- ✅ Mood Selection Interface
- ✅ Mood-Based Movie Recommendations
- ✅ Watchlist Management
- ✅ Movie Rating System
- ✅ Admin Dashboard
- ✅ Dark/Light Mode
- ✅ Responsive Design
- ✅ AI Mood Detection (Optional)

## 🔐 API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/me` - Get current user

### Movies
- `GET /api/movies/recommend` - Get mood-based recommendations
- `GET /api/movies/:id` - Get movie details
- `GET /api/movies/search` - Search movies

### Watchlist
- `GET /api/watchlist` - Get user watchlist
- `POST /api/watchlist` - Add to watchlist
- `DELETE /api/watchlist/:id` - Remove from watchlist

### Ratings
- `POST /api/ratings` - Rate a movie
- `GET /api/ratings/:movieId` - Get movie rating

### Admin
- `GET /api/admin/users` - Get all users
- `GET /api/admin/movies` - Manage movies
- `GET /api/admin/feedback` - View feedback

## 🚢 Deployment

### Backend (Render/Railway)
1. Push code to GitHub
2. Connect repository to Render/Railway
3. Set environment variables
4. Deploy

### Frontend (Netlify/Vercel)
1. Build the project: `npm run build`
2. Connect repository to Netlify/Vercel
3. Set environment variables
4. Deploy

## 📝 Development Timeline

- **Week 1**: Setup, Authentication, Mood Selection
- **Week 2**: Movie Recommendations, Watchlist, Ratings
- **Week 3**: AI Detection, Admin Dashboard, Polish, Deployment

## 🤝 Contributing

This is a capstone project. For questions or issues, please contact the project team.

## 📄 License

This project is for educational purposes.
capstone project 