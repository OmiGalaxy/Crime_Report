# Setup Instructions

## Prerequisites
- Python 3.8+
- Node.js 18+
- npm or yarn

## Backend Setup
```bash
cd backend
python -m venv venv
venv\Scripts\activate  # Windows
# source venv/bin/activate  # Linux/Mac
pip install -r requirements.txt
python init_db.py
python -m uvicorn main:app --reload --host 0.0.0.0 --port 8000
```

## Frontend Setup
```bash
cd frontend
npm install
cp ../.env.example .env.local
npm run dev
```

## Demo Login Credentials
- **Admin**: admin@crimewatch.com / password123
- **Police**: officer@police.gov / password123  
- **User**: citizen@email.com / password123

## URLs
- Frontend: http://localhost:3000
- Backend: http://localhost:8000
- API Docs: http://localhost:8000/docs