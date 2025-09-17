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
pip install -r requirements.txt
python init_db.py
uvicorn main:app --reload
```

### Frontend Setup
```bash
cd frontend
npm install
npm run dev
```

## Default Users

After running `init_db.py`:
- **Admin**: admin@crime.gov / admin123
- **User**: user@example.com / user123

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