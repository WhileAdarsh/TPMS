# 🚀 Training and Placement Management System (TPMS) – NIT Jamshedpur

## 📑 Table of Contents
- [📌 Introduction](#-introduction)
- [✨ Features](#-features)
- [🛠️ Tech Stack](#-tech-stack)
- [📂 Project Structure](#-project-structure)
- [👥 User Roles](#-user-roles)
- [⚙️ Installation](#-installation)
  - [🔗 Backend Setup](#-backend-setup)
  - [🎨 Frontend Setup](#-frontend-setup)

---

## 📌 Introduction
The **Training and Placement Management System (TPMS)** is a comprehensive web-based solution built for **NIT Jamshedpur** to efficiently manage and streamline the placement process. This platform reduces manual work, increases transparency, and provides real-time data for students, Training and Placement Officers (TPO), and management.

Developed with ❤️ by:
- **Adarsh Kumar**
- **Chandan Pandey**
- **Gangadhar Kumar**

---

## ✨ Features

### 👨‍🎓 Student Features
- 🔐 Secure registration and login
- 📄 Profile creation and resume upload
- 💼 View eligible job postings
- 📝 Apply for job opportunities
- 🔍 Check application and interview status

### 🏢 TPO/Admin Features
- 🆕 Post job listings and manage companies
- 👥 Approve or reject student applications
- 📅 Schedule interviews and events
- 📜 Upload and distribute offer letters

### 📊 Management Features
- 📈 View placement statistics and reports
- 🗂️ Access student data and company analytics
- 🔍 Monitor overall placement progress

### 🛡️ Super Admin Features
- 🔧 System configuration management
- 👤 Manage and onboard TPO/Admin users
- 🗂️ Full access to all data and reports

### ☁️ File Storage
- ✅ Secure cloud storage via **Cloudinary** for:
  - 📄 Resumes
  - 📜 Offer letters
  - 📷 Profile pictures

---

## 🛠️ Tech Stack
| Technology | Description        |
|-------------|--------------------|
| ⚛️ React.js (Vite) | Frontend Framework |
| 🎨 Tailwind CSS + Bootstrap | Styling |
| 🟩 Node.js + 🚂 Express.js | Backend Framework |
| 🍃 MongoDB | NoSQL Database |
| 🔐 JSON Web Token (JWT) | Authentication |
| ☁️ Cloudinary | File Storage |

---

## 📂 Project Structure
```plaintext
├── frontend
│   ├── public
│   ├── src
│   │   ├── api
│   │   ├── assets
│   │   ├── components
│   │   │   ├── LandingPages
│   │   │   └── students
│   │   ├── config
│   │   │   └── backend_url.js
│   │   ├── context
│   │   ├── hooks
│   │   ├── pages
│   │   ├── styles
│   │   ├── utility
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── .gitignore
│   ├── vite.config.js
├── backend
│   ├── config
│   ├── controllers
│   ├── middleware
│   ├── models
│   ├── routes
│   ├── .env (🔐 Required)
│   ├── index.js
│   ├── package.json
└── README.md
```

## User Roles
- **Students**: View and apply for jobs, update profile, track status, and upload resumes.
- **TPO Admin**: Post jobs, manage applications, upload offer letters, and schedule interviews.
- **Management Admin**: Access dashboards and reports for data-driven decision making.
- **Super Admin**: Manage system settings, and create/manage TPO and Management users.

## Installation

### Prerequisites
- Node.js and npm installed
- MongoDB installed and running
- Cloudinary account for file uploads

### Clone the Repository
```bash
git clone https://github.com/moinmn/college-placement-management-system.git
cd college-placement-management-system
```

### Backend Setup
1. Navigate to the `backend` folder:
   ```bash
   cd backend
   ```
2. Install the necessary packages:
   ```bash
   npm install
   ```
3. Create a `.env` file for environment variables:
   ```env
   PORT=4518
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   SMTP_USER="your_email_id"
   SMTP_PASS="your_app_password_to_be_generate_via_google_settings"
   ```
4. Start the backend server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to the `frontend` folder:
   ```bash
   cd frontend
   ```
2. Install the necessary packages:
   ```bash
   npm install
   ```
3. Change backend URL for local testing:
   Go to `src/config/backend_url.js` and update:
   ```js
   export const BASE_URL = 'http://localhost:4518';
   ```
4. Start the frontend development server:
   ```bash
   npm run dev
   ```


