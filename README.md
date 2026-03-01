# Meal Planner

A meal planning application with a FastAPI backend and React frontend for managing weekly meal plans and recipes.

## What It Is

A full-stack meal planning application that helps users organize their weekly meals and manage recipes. The backend provides REST API endpoints for meal data management, while the frontend offers an intuitive interface for planning meals and tracking ingredients.

## Tech Stack

### Backend
- **Framework**: FastAPI with Python
- **CORS**: Enabled for frontend integration
- **Async**: Full async/await support
- **Port**: 8000

### Frontend
- **Framework**: React 19 with TypeScript
- **Build**: Vite with SWC
- **Routing**: React Router DOM
- **Port**: 5173

## Getting Started

### Backend Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install fastapi uvicorn
python main.py
```

The backend will run on `http://localhost:8000`

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

The frontend will be available at `http://localhost:5173`

### Building for Production

**Backend**: Deploy Uvicorn server with FastAPI app

**Frontend**:
```bash
npm run build
```

## Features

- **Meal Planning**: Organize meals for the entire week
- **Recipe Management**: Store and manage recipe data
- **Ingredient Tracking**: Keep track of ingredients and quantities
- **Easy Navigation**: Clean UI with React Router for seamless experience

## API Endpoints

- `GET /api/hello` - Health check endpoint
- Additional endpoints as implemented in backend

## Project Structure

```
meal-planner/
├── backend/
│   ├── main.py          # FastAPI app and routes
│   └── venv/            # Python environment
├── frontend/
│   ├── src/
│   │   ├── components/  # React components
│   │   ├── pages/       # Page components
│   │   └── App.jsx      # Main app
│   ├── public/
│   └── package.json
└── README.md
```

## Development Notes

- CORS middleware allows frontend communication during development
- Frontend configured to work with backend at `http://localhost:8000`
- React Router enables client-side navigation
- Vite provides fast development experience with HMR
- Can be deployed to any hosting platform (Vercel, Netlify, etc.)

## Environment Setup

Make sure both backend and frontend are running on their respective ports for full functionality:
- Backend: `http://localhost:8000`
- Frontend: `http://localhost:5173`
