SkillSync: AI Career Recommendation Platform

SkillSync is a full-stack web application designed to help users discover their ideal career path. It combines a modern, responsive frontend, a secure user authentication system, and an AI-powered prediction engine to provide personalized career recommendations based on a user's multiple intelligence scores.
This project uses a microservice-style architecture, splitting the user management and the AI prediction into two separate, dedicated backend services.

---

OVERVIEW:

This project integrates:
A Node.js + Express backend for APIs and authentication.
A React.js frontend for an interactive UI.
A Python model for AI or data processing tasks.
It follows a modular structure for maintainability and scalability.

---

TECH STACK:

Layer	Technology Used:

Frontend	React.js, HTML5, CSS3, JavaScript
Backend	Node.js, Express.js
Database	MongoDB (via Mongoose)
Model	Python 3, virtual environment
Authentication	JWT (JSON Web Token), bcrypt for password hashing
Version Control	Git & GitHub



---

FOLDER STRUCTURE:

project-root/
│
├── backend/              # Node.js backend
│   ├── config/           # Database config
│   ├── controllers/      # Route controllers
│   ├── models/           # Mongoose models
│   ├── routes/           # Express routes
│   ├── middlewares/      # Auth and validation middleware
│   └── server.js         # Entry point
│
├── frontend/             # React frontend
│   ├── src/
│   ├── public/
│   └── package.json
│
├── model/                # Python model logic
│   ├── model.py
│   ├── requirements.txt
│   └── .env/ (virtual environment)
│
└── README.md


---

SETUP GUIDE:

Follow these steps to run the project locally.


---

1. Backend Setup

cd backend
npm install
node server.js

> Ensure your .env file in the backend directory is properly configured.




---

2️. Frontend Setup

cd frontend
npm install
npm start

> Starts the React app, usually at http://localhost:3000




---

3️. Model Setup (Python)

cd model
python3 -m venv .env
source .env/bin/activate
pip install -r requirements.txt
python3 model.py

This runs the Python-based model service.
You can create a requirements.txt file with necessary libraries such as:

flask
numpy
pandas
scikit-learn
requests




---

ENVIRONMENT VARIABLES:

Create a .env file in the backend directory with the following keys:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
CLIENT_URL=http://localhost:3000

If your model also needs environment variables, you can define them in its .env file too.


---

USAGE: 

1. Start Backend → node server.js


2. Start Frontend → npm start


3. Start Model → python3 model.py


4. Open your browser → http://localhost:3000




---

TROUBLESHOOTING: 

Issue	Possible Fix

Token missing	Ensure frontend sends JWT in Authorization header
MongoDB connection error	Check MONGO_URI in .env file
Module not found	Run npm install or pip install -r requirements.txt again
CORS error	Verify backend has app.use(cors()) enabled



---

CONTRIBUTING:

Contributions are always welcome!

1. Fork the repository


2. Create your feature branch: git checkout -b feature-name


3. Commit changes: git commit -m 'Add new feature'


4. Push to branch: git push origin feature-name


5. Submit a Pull Request




---

LICENSE:

This project is licensed under the MIT License.
Feel free to modify and use it for personal or educational purposes.
