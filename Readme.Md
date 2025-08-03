# 📦 Parcel Delivery System  
A full-stack MERN (MongoDB, Express.js, React.js, Node.js) application for managing parcel delivery. It allows customers to book parcels, agents to manage assigned deliveries, and admins to oversee the system.  

## Live Server Link: https://parceltrack.netlify.app/

🚀 Features  
- 🔐 Secure Authentication for customers, agents, and admins  
- 📦 Create, view, update & track parcels  
- 🧑‍✈️ Assign parcels to agents with location tracking  
- 🔔 Real-time notifications using WebSocket  
- 📊 Generate daily, weekly & monthly reports  
- 🎨 Modern UI with React, Tailwind CSS, and DaisyUI  
🛠️ Technologies Used  
Frontend: React, React Router, Tailwind CSS, DaisyUI, Leaflet (maps), Recharts (charts), jsPDF (PDF export)  
Backend: Node.js, Express.js, MongoDB, WebSocket, bcryptjs, dotenv  
⚙️ Getting Started  
1. Clone the repo  
   git clone https://github.com/Arjon200141/excel-tech-mern-task  
2. Install backend dependencies  
   cd excel-tech-mern-task-server  
   npm install  
3. Install frontend dependencies  
   cd ../excel-tech-mern-task-client  
   npm install  
4. Create a `.env` file in `excel-tech-mern-task-server` and add:  
   MONGODB_URI=your-mongodb-uri  
   PORT=5000  
5. Run backend  
   cd excel-tech-mern-task-server  
   npm start  
6. Run frontend  
   cd ../excel-tech-mern-task-client  
   npm run dev  
Your app runs at:  
Frontend → http://localhost:5173  
Backend  → http://localhost:5000  
📡 API Endpoints  
Auth:  
- POST /users/login  
- POST /users/register  
Users:  
- GET /users  
- DELETE /users/:userId  
Agents:  
- GET /agents  
- PATCH /agents/:id/location  
Parcels:  
- POST /parcels  
- GET /parcels  
- GET /parcels/:id  
- PATCH /parcels/:id/assign-agent  
- GET /agentparcels/:agentId  
- PATCH /agparcels/:id/status  
- GET /tracking/:parcelId  
Notifications:  
- GET /notifications/:userId  
- PUT /notifications/:userId/mark-as-read  
Reports:  
- GET /parcels/reports  
📁 Folder Structure  
project-root/  
├── excel-tech-mern-task-client/  
│   └── src/  
│       ├── assets/  
│       ├── Components/  
│       ├── App.jsx  
│       └── main.jsx  
├── excel-tech-mern-task-server/  
│   ├── .env  
│   ├── index.js  
│   └── package.json  
└── README.md  
🤝 Contributing  
- Fork this repo  
- Create a feature branch  
- Commit and push changes  
- Open a pull request  