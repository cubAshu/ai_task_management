project name: ai_task_managemnet
purpose of aplication: AI Task & Knowledge Management Engine is a full-stack enterprise-style application designed to centralize task management, document knowledge retrieval, AI-assisted task generation, user access control, auditability, and operational analytics.

The system combines a FastAPI backend with a React frontend and MySQL database, while integrating JWT-based authentication, role-based access control, FAISS semantic retrieval, and activity/audit logging.

The project was designed with maintainability, modularity, API-first development, and real-world backend engineering practices in mind.

Technologies used: Python FastAPI React JavaScript MySQL SQLAlchemy JWT FAISS Axios Git GitHub


steps required to run the application: 
▶️ Run Backend
From the backend directory:

uvicorn app.main:app --reload
Backend:

http://127.0.0.1:8000
Swagger:

http://127.0.0.1:8000/docs

⚛️ Frontend Setup
Open another terminal.

cd frontend
Install dependencies:

npm install
Start the development server:

npm run dev
The frontend will normally be available through the URL displayed by Vite.

INSTALLATION:

🐍 Backend Setup
Navigate to the backend directory:

cd backend
Create a virtual environment:

Windows
python -m venv venv
Activate it:

venv\Scripts\activate
Linux / macOS
python3 -m venv venv
source venv/bin/activate
Install dependencies:

pip install -r requirements.txt
🗄️ Database Configuration
Create a MySQL database.

Example:

CREATE DATABASE ai_task_manager;
Configure the database connection in the backend environment configuration.

Example:

DATABASE_URL=mysql+pymysql://username:password@localhost:3306/ai_task_manager
🔐 Environment Variables
Example backend .env:

DATABASE_URL=mysql+pymysql://username:password@localhost:3306/ai_task_manager

SECRET_KEY=your-secret-key

ALGORITHM=HS256

ACCESS_TOKEN_EXPIRE_MINUTES=60

