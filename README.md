# SewaPath 🇳🇵

### Citizen-First Government Service Navigator

SewaPath is a full-stack web application designed to make government services in Nepal easier to discover and understand.

The platform helps citizens find relevant government services, explore service information, and navigate toward the resources they need through a clean, responsive interface.

<p align="center">
  <a href="https://sewapath-frontend.vercel.app/">
    <img src="https://img.shields.io/badge/Live_Demo-Visit_SewaPath-111827?style=for-the-badge" alt="SewaPath Live Demo" />
  </a>
  <a href="https://github.com/bipesh369/SewaPath">
    <img src="https://img.shields.io/badge/Source_Code-GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="SewaPath GitHub Repository" />
  </a>
</p>

---

## 📌 Why SewaPath?

Finding the right government service can be difficult when information is spread across different websites, offices, and resources.

SewaPath aims to provide a centralized and user-friendly experience where citizens can:

* Discover government services
* Browse services by category
* View service-related information
* Find relevant locations
* Access service details through a responsive interface
* Navigate government information more easily

The project focuses on solving a practical problem while demonstrating modern frontend and full-stack development skills.

---

## ✨ Key Features

### 🔎 Service Discovery

Browse and explore government services through organized categories and service information.

### 🗂️ Service Categories

Services are organized into categories to make discovering relevant information easier.

### 🗺️ Location-Based Information

Interactive maps help users understand where relevant services or locations are available.

### 🔐 Authentication

The application uses JWT-based authentication for protected functionality.

### 📱 Responsive Interface

The frontend is designed to work across desktop, tablet, and mobile screen sizes.

### 🔗 REST API

The React frontend communicates with a Node.js and Express.js backend through REST APIs.

### 🗄️ Persistent Data

MongoDB and Mongoose are used to store and manage application data.

---

## 🛠️ Tech Stack

### Frontend

| Technology   | Purpose                                |
| ------------ | -------------------------------------- |
| React.js     | User interface                         |
| JavaScript   | Application logic                      |
| Tailwind CSS | Styling and responsive UI              |
| Vite         | Frontend development and build tooling |
| Leaflet      | Interactive maps                       |

### Backend

| Technology        | Purpose                 |
| ----------------- | ----------------------- |
| Node.js           | Server-side runtime     |
| Express.js        | REST API                |
| Mongoose          | MongoDB object modeling |
| JWT               | Authentication          |
| bcryptjs          | Password hashing        |
| express-validator | Request validation      |
| Morgan            | HTTP request logging    |

### Database

**MongoDB**

Used for storing users, services, categories, and other application data.

### Development Tools

* Git
* GitHub
* npm
* Vite
* Postman / REST API testing tools

---

## 🏗️ Architecture

SewaPath follows a traditional MERN full-stack architecture:

```text
┌──────────────────────────────┐
│          React.js            │
│       Frontend / UI          │
└──────────────┬───────────────┘
               │
               │ REST API
               ▼
┌──────────────────────────────┐
│       Node.js + Express      │
│       Backend / API          │
└──────────────┬───────────────┘
               │
               │ Mongoose
               ▼
┌──────────────────────────────┐
│           MongoDB            │
│        Persistent Data       │
└──────────────────────────────┘
```

The frontend is responsible for the user experience and application interface, while the backend handles API requests, authentication, validation, and database communication.

---

## 📂 Project Structure

```text
SewaPath/
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── seed/
│   ├── server.js
│   └── package.json
│
└── README.md
```

> The exact folder structure may evolve as the project continues to be developed.

---

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

* Node.js
* npm
* MongoDB or a MongoDB connection string
* Git

---

### 1. Clone the repository

```bash
git clone https://github.com/bipesh369/SewaPath.git

cd SewaPath
```

---

### 2. Setup the frontend

```bash
cd frontend
npm install
```

Create a `.env` file if the frontend requires environment variables:

```env
VITE_API_URL=your_backend_api_url
```

Start the development server:

```bash
npm run dev
```

The frontend will normally be available at:

```text
http://localhost:5173
```

---

### 3. Setup the backend

Open another terminal:

```bash
cd backend
npm install
```

Create a `.env` file:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

Start the backend:

```bash
npm run dev
```

For production:

```bash
npm start
```

---

## 🔐 Environment Variables

Never commit your `.env` file or secret credentials to GitHub.

Example:

```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/sewapath
JWT_SECRET=your_secure_secret
```

Use environment-specific values when deploying the application.

---

## 🧪 Development & Testing

The backend includes scripts for development, seeding, and testing.

```bash
npm run dev
```

```bash
npm run seed
```

```bash
npm test
```

The project uses Jest for backend testing.

---

## 🎯 What I Learned Building SewaPath

SewaPath was built as a practical full-stack project and helped me strengthen several areas of development:

### Frontend

* Building reusable React components
* Managing application state
* Creating responsive interfaces
* Integrating REST APIs
* Working with interactive maps
* Building user-focused navigation flows

### Backend

* Designing REST APIs with Express
* Structuring Node.js applications
* Working with MongoDB and Mongoose
* Implementing authentication
* Validating API requests
* Handling backend errors and middleware

### Full-Stack

* Connecting React applications with REST APIs
* Managing frontend and backend development separately
* Working with environment variables
* Designing data models
* Debugging client-server communication
* Using Git throughout development

---

## 🧠 Engineering Focus

While building SewaPath, the main focus has been:

```text
User Experience
      ↓
Reusable React Components
      ↓
REST API Integration
      ↓
Backend Validation & Authentication
      ↓
MongoDB Data Management
```

The project is continuously being improved as I learn more about frontend architecture, backend development, security, and production-ready application design.

---

## 📸 Screenshots

Add 3–5 screenshots here showing the most important parts of the application.

Recommended screenshots:

1. Home page
2. Service discovery/category page
3. Service details
4. Map/location interface
5. Authentication or dashboard

Example:

```md
## 📸 Screenshots

### Home

![SewaPath Home](./screenshots/home.png)

### Service Discovery

![Service Discovery](./screenshots/services.png)

### Service Details

![Service Details](./screenshots/service-details.png)
```

---

## 🌐 Live Demo

**Frontend:**
https://sewapath-frontend.vercel.app/

**Source Code:**
https://github.com/bipesh369/SewaPath

---

## 🔮 Future Improvements

Planned improvements may include:

* Improved service search and filtering
* More comprehensive government service information
* Enhanced accessibility
* Better location-based discovery
* Improved user dashboards
* Additional administrative functionality
* More comprehensive automated testing
* Production-focused performance improvements

---

## 👨‍💻 Developer

**Bipesh Junior Tharu**

Frontend Developer focused on React, JavaScript, TypeScript, and modern web development, with hands-on experience building MERN applications.

<p>
  <a href="https://github.com/bipesh369">GitHub</a> •
  <a href="https://www.linkedin.com/in/bipeshjunior10">LinkedIn</a> •
  <a href="mailto:juniorbipesh@gmail.com">Email</a>
</p>

---

## 📄 License

This project is currently developed as a portfolio and learning project.

---

<p align="center">
  <strong>Built with React, Node.js, Express.js, and MongoDB 🇳🇵</strong>
</p>
