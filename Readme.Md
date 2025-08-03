 # Parcel Delivery System
    2
    3 This is a full-stack MERN (MongoDB, Express, React, Node.js) application for a parcel delivery
      system. It allows customers to book parcels, agents to manage their assigned parcels, and admins
      to oversee the entire system.
    4
    5 ## Features
    6
    7 *   **User Authentication:** Secure user registration and login for customers, agents, and
      admins.
    8 *   **Parcel Management:** Create, view, update, and track parcels.
    9 *   **Agent Management:** Assign parcels to agents and track their locations in real-time.
   10 *   **Real-time Notifications:** Receive real-time notifications for important events, such as
      parcel assignment and status updates.
   11 *   **Reporting:** Generate daily, weekly, and monthly reports on parcel activity.
   12 *   **User-friendly Interface:** A modern and responsive user interface built with React and
      Tailwind CSS.
   13
   14 ## Technologies Used
   15
   16 **Frontend:**
   17
   18 *   React
   19 *   React Router
   20 *   Tailwind CSS
   21 *   DaisyUI
   22 *   Leaflet (for maps)
   23 *   Recharts (for charts)
   24 *   jsPDF (for PDF export)
   25
   26 **Backend:**
   27
   28 *   Node.js
   29 *   Express.js
   30 *   MongoDB
   31 *   WebSocket (for real-time communication)
   32 *   bcryptjs (for password hashing)
   33 *   dotenv (for environment variables)
   34
   35 ## Getting Started
   36
   37 ### Prerequisites
   38
   39 *   Node.js (v14 or later)
   40 *   npm (v6 or later)
   41 *   MongoDB (local or a cloud-based instance)
   42
   43 ### Installation
   44
   45 1.  **Clone the repository:**
      git clone <repository-url>

   1
   2 2.  **Install server dependencies:**
      cd excel-tech-mern-task-server
      npm install
   1
   2 3.  **Install client dependencies:**
      cd ../excel-tech-mern-task-client
      npm install

   1
   2 ### Configuration
   3
   4 1.  **Create a `.env` file** in the `excel-tech-mern-task-server` directory.
   5
   6 2.  **Add the following environment variables** to the `.env` file:
      MONGODB_URI=<your-mongodb-connection-string>
      PORT=5000
   1
   2 ### Running the Application
   3
   4 1.  **Start the server:**
      cd excel-tech-mern-task-server
      npm start
   1
   2 2.  **Start the client:**
      cd ../excel-tech-mern-task-client
      npm run dev

    1
    2 The client will be running at `http://localhost:5173` and the server at `http://localhost:5000`.
    3
    4 ## API Documentation
    5
    6 The backend API provides a set of RESTful endpoints for managing users, parcels, and agents. You
      can use the provided Postman collection to test the API.
    7
    8 ### Main Endpoints
    9
   10 *   `POST /users/login`: User login.
   11 *   `POST /users/register`: User registration.
   12 *   `GET /users`: Get all users.
   13 *   `DELETE /users/:userId`: Delete a user.
   14 *   `GET /agents`: Get all agents.
   15 *   `PATCH /agents/:id/location`: Update agent location.
   16 *   `POST /parcels`: Create a new parcel.
   17 *   `GET /parcels`: Get all parcels.
   18 *   `GET /parcels/:id`: Get a parcel by ID.
   19 *   `PATCH /parcels/:id/assign-agent`: Assign an agent to a parcel.
   20 *   `GET /agentparcels/:agentId`: Get all parcels assigned to an agent.
   21 *   `PATCH /agparcels/:id/status`: Update the status of a parcel.
   22 *   `GET /tracking/:parcelId`: Get tracking information for a parcel.
   23 *   `GET /notifications/:userId`: Get notifications for a user.
   24 *   `PUT /notifications/:userId/mark-as-read`: Mark a notification as read.
   25 *   `GET /parcels/reports`: Get parcel reports.
   26
   27 ## Folder Structure
  .
  ├── excel-tech-mern-task-client/  # React frontend
  │   ├── public/
  │   └── src/
  │       ├── assets/
  │       ├── Components/
  │       ├── App.jsx
  │       └── main.jsx
  ├── excel-tech-mern-task-server/  # Express backend
  │   ├── node_modules/
  │   ├── .env
  │   ├── index.js
  │   └── package.json
  └── README.md
   1
   2 ## Contributing
   3
   4 Contributions are welcome! Please feel free to open an issue or submit a pull request.