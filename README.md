# Crime Report Management System

A modern web application for real-time crime reporting and management with role-based access control.

## Features

- **Multi-Role System**: Normal Users, Police Officers, and Administrators
- **Real-time Notifications**: Instant updates on complaint status
- **Secure Authentication**: JWT-based authentication with role management
- **File Upload**: Image attachments for complaints
- **Professional Dashboard**: Clean, modern UI for all user types

## Tech Stack

### Backend
- FastAPI (Python)
- SQLite Database
- JWT Authentication
- File Upload Support

### Frontend
- Next.js 15.5
- TypeScript
- Tailwind CSS
- Modern UI Components

## Project Structure

```
CrimeR/
├── backend/          # FastAPI backend
├── frontend/         # Next.js frontend
└── README.md        # This file
```

## Quick Start

### Backend Setup
```bash
cd backend
python -m venv venv
venv\Scripts\activate  # Windows
# source venv/bin/activate  # Linux/Mac
pip install -r requirements.txt
python init_db.py
python -m uvicorn main:app --reload --host 0.0.0.0 --port 8000
```

### Frontend Setup
```bash
cd frontend
npm install
cp ../.env.example .env.local
npm run dev
```

## Demo Login Credentials

After running `init_db.py`:
- **Admin**: admin@crimewatch.com / password123
- **Police**: officer@police.gov / password123
- **User**: citizen@email.com / password123

## API Endpoints

- `POST /auth/register` - User registration
- `POST /auth/login` - User login
- `POST /auth/refresh` - Refresh token
- `POST /complaints/register` - File complaint
- `GET /complaints/` - Get complaints
- `POST /complaints/{id}/approve` - Approve complaint
- `POST /complaints/{id}/reject` - Reject complaint
- `GET /users/profile` - Get user profile
- `PUT /users/profile` - Update profile

## License

MIT License - 2025