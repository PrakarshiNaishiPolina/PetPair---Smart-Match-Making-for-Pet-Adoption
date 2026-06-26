# 🐾 PetPair – Smart Pet Adoption Platform

PetPair is a full-stack pet adoption platform that connects potential adopters with pets based on their lifestyle and preferences. Instead of browsing endless listings, users receive personalized pet recommendations and can easily submit adoption requests. The platform also provides an admin dashboard for managing pets and adoption requests.

---

# 📌 Table of Contents

- Project Overview
- Features
- Technology Stack
- System Architecture
- Folder Structure
- Installation
- Environment Variables
- Running the Project
- Usage
- API Endpoints
- Database Models
- Authentication
- Future Enhancements
- Screenshots
- Author

---

# 📖 Project Overview

PetPair aims to simplify the pet adoption process by matching users with suitable pets based on compatibility factors such as:

- Living space
- Activity level
- Experience with pets
- Budget
- Family type
- Preferred pet type

The application provides separate interfaces for users and administrators while maintaining secure authentication and dynamic data management.

---

# ✨ Features

## 👤 User Features

- User Registration
- Secure Login using JWT Authentication
- Personalized User Profile
- Browse Available Pets
- View Pet Details
- Smart Pet Recommendation System
- Submit Adoption Requests
- View Adoption Request Status
- Cancel Approved Adoptions
- Contact Form
- Responsive User Interface

---

## 👨‍💼 Admin Features

- Secure Admin Login
- Admin Dashboard
- Add New Pets
- Upload Pet Images
- Assign Maintenance Cost
- View Adoption Requests
- Approve Adoption Requests
- Reject Adoption Requests
- Manage Available Pets

---

## 🐶 Pet Features

- Dynamic Pet Listings
- Image Upload Support
- Breed Information
- Maintenance Cost
- Age
- Gender
- Vaccination Details
- Availability Status

---

# 🛠 Technology Stack

## Frontend

- HTML5
- CSS3
- JavaScript (ES6)

## Backend

- Node.js
- Express.js

## Database

- MongoDB
- Mongoose

## Authentication

- JSON Web Tokens (JWT)

## File Upload

- Multer

---

# 🏗 System Architecture

```
Frontend (HTML/CSS/JS)
          │
          │ HTTP Requests
          ▼
Express.js Server
          │
 ┌────────┴─────────┐
 │                  │
Authentication   Pet APIs
 │                  │
 └────────┬─────────┘
          │
     MongoDB Database
```

---

# 📁 Folder Structure

```
PetPair/
│
├── frontend/
│   ├── index.html
│   ├── login.html
│   ├── signup.html
│   ├── pets.html
│   ├── profile.html
│   ├── admin.html
│   ├── petform.html
│   ├── contact.html
│   ├── css/
│   ├── js/
│   └── images/
│
├── backend/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── uploads/
│   ├── server.js
│   ├── package.json
│   └── .env
│
└── README.md
```

---

# ⚙ Installation

## Clone the Repository

```bash
git clone https://github.com/yourusername/PetPair.git
```

Move into the project directory.

```bash
cd PetPair
```

Install backend dependencies.

```bash
npm install
```

---

# 🔐 Environment Variables

Create a `.env` file inside the backend folder.

```env
PORT=5000

MONGO_URI=your_mongodb_connection_string

JWT_SECRET=your_secret_key
```

---

# ▶ Running the Project

Start the backend server.

```bash
node server.js
```

or

```bash
npm start
```

Open the frontend in your browser (or use Live Server in VS Code).

Backend runs on:

```
http://localhost:5000
```

Frontend:

```
http://127.0.0.1:5500
```

---

# 🚀 Usage

## User Workflow

1. Register a new account.
2. Login securely.
3. Browse available pets.
4. Fill the Pet Preference Form.
5. Receive pet recommendations.
6. Submit an adoption request.
7. Wait for admin approval.
8. Track adoption status.
9. Cancel adoption if needed.

---

## Admin Workflow

1. Login as Administrator.
2. Open Admin Dashboard.
3. Add pets.
4. Upload pet images.
5. Set maintenance cost.
6. Review adoption requests.
7. Approve or reject requests.

---

# 🌐 API Endpoints

## Authentication

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/signup | Register User |
| POST | /api/login | Login User |

---

## Pets

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | /api/pets | Get All Pets |
| POST | /api/pets | Add New Pet |

---

## Pet Suggestions

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/suggest-pet | Get Matching Pet Suggestions |

---

## Adoption Requests

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/request | Submit Adoption Request |
| GET | /api/request | View Requests |
| PUT | /api/request/:id | Approve or Reject Request |

---

## Adoptions

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | /api/adoptions | View Approved Adoptions |
| DELETE | /api/adoptions/:id | Cancel Adoption |

---

# 🗄 Database Models

## User

- Name
- Email
- Password (Hashed)
- Role

---

## Pet

- Name
- Breed
- Age
- Gender
- Image
- Maintenance Cost
- Description

---

## Adoption Request

- User ID
- Pet ID
- Status
- Date

---

## Adoption

- User ID
- Pet ID
- Approval Date

---

# 🔒 Authentication

PetPair uses **JSON Web Tokens (JWT)** for secure authentication.

Features include:

- Protected Routes
- Role-Based Authorization
- Secure Password Storage
- Token Verification Middleware

---

# 💡 Future Enhancements

- AI-Based Pet Recommendation
- Email Notifications
- Real-Time Chat
- Online Adoption Appointment Booking
- Payment Gateway Integration
- Veterinary Consultation
- Donation Portal
- Pet Health Records
- Wishlist
- Search & Advanced Filters
- Dark Mode
- Mobile Application

---

# 📷 Screenshots

Add screenshots of:

- Home Page
- Login Page
- Signup Page
- Pet Listings
- Pet Recommendation Form
- User Profile
- Admin Dashboard
- Adoption Requests

Example:

```
screenshots/
│
├── home.png
├── login.png
├── signup.png
├── pets.png
├── profile.png
├── admin.png
```

---

# 🎯 Learning Outcomes

This project demonstrates practical knowledge of:

- Full Stack Web Development
- RESTful API Development
- MongoDB Database Design
- Authentication using JWT
- File Upload using Multer
- CRUD Operations
- Role-Based Access Control
- Frontend-Backend Integration
- Responsive Web Design



