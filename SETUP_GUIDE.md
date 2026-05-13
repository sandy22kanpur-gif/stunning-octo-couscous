# Wingo Colour Prediction - Installation & Setup Guide

## Prerequisites

- Node.js v14+
- MongoDB (local or Atlas)
- npm or yarn

## Backend Setup

### 1. Install Dependencies
```bash
cd backend
npm install
```

### 2. Configure Environment
Create a `.env` file in the backend directory:
```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/wingo-prediction
JWT_SECRET=your_secret_key_change_this_in_production
NODE_ENV=development
```

### 3. Run Backend
```bash
npm start
# or for development with auto-reload
npm run dev
```

The backend will run on `http://localhost:5000`

## Frontend Setup

### 1. Install Dependencies
```bash
cd frontend
npm install
```

### 2. Run Frontend
```bash
npm run dev
```

The frontend will run on `http://localhost:3000`

## Running the Complete Application

### Terminal 1 - Backend
```bash
cd backend
npm install
npm start
```

### Terminal 2 - Frontend
```bash
cd frontend
npm install
npm run dev
```

### Terminal 3 - MongoDB (if running locally)
```bash
mongod
```

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user

### Users
- `GET /api/users/profile` - Get user profile (requires auth)

### Predictions
- `POST /api/predictions/place` - Place a bet (requires auth)
- `GET /api/predictions` - Get user's predictions (requires auth)

### Admin
- `GET /api/admin/users` - Get all users (admin only)
- `PUT /api/admin/users/:userId` - Update user balance (admin only)
- `GET /api/admin/rounds` - Get all game rounds (admin only)
- `POST /api/admin/rounds/:roundId/result` - Declare game result (admin only)

## Features

✅ User Registration & Login
✅ Colour Prediction Game (6 colors)
✅ Real-time Balance Updates
✅ Bet Placement with 5x Multiplier
✅ Admin Dashboard
✅ User Management
✅ Game Round Management
✅ Statistics Tracking

## Deployment

### Frontend (Vercel/Netlify)
```bash
cd frontend
npm run build
```

### Backend (Heroku/Railway)
```bash
# Push to Git and deploy
```

## Troubleshooting

**MongoDB Connection Error:**
- Ensure MongoDB is running locally or update MONGODB_URI to your Atlas connection string

**CORS Error:**
- Check that frontend URL matches the CORS configuration in backend

**Port Already in Use:**
- Change PORT in .env file or kill the process using the port

## Default Admin Account

Create an admin user by modifying the User model to set `role: 'admin'` during registration or through the database.

## Contact & Support

For issues or questions, create an issue in the GitHub repository.
