# Wingo Colour Prediction Website

A modern web application for wingo colour prediction with a comprehensive admin panel.

## Features

- **User Interface**: Intuitive colour prediction game interface
- **Admin Panel**: Manage predictions, users, and game settings
- **Real-time Updates**: Live prediction tracking
- **User Authentication**: Secure login and registration
- **History Tracking**: View prediction history and statistics

## Project Structure

```
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── admin/
│   │   └── App.jsx
│   └── package.json
├── backend/
│   ├── routes/
│   ├── controllers/
│   ├── models/
│   ├── middleware/
│   └── server.js
├── database/
│   └── schema.sql
└── README.md
```

## Tech Stack

- **Frontend**: React.js, Tailwind CSS
- **Backend**: Node.js, Express.js
- **Database**: MongoDB/MySQL
- **Authentication**: JWT

## Installation

### Prerequisites
- Node.js v14+
- npm or yarn
- MongoDB or MySQL

### Setup

1. Clone the repository
```bash
git clone https://github.com/sandy22kanpur-gif/stunning-octo-couscous.git
cd stunning-octo-couscous
```

2. Install backend dependencies
```bash
cd backend
npm install
```

3. Install frontend dependencies
```bash
cd ../frontend
npm install
```

4. Configure environment variables
```bash
# Create .env files in backend and frontend directories
```

5. Run the application
```bash
# Terminal 1 - Backend
cd backend
npm start

# Terminal 2 - Frontend
cd frontend
npm start
```

## Usage

- User can play colour prediction games
- Admin can manage game settings and view statistics
- Real-time updates for active games

## License

MIT License
