# 🛡️ Auth Dashboard

A **role-based access control dashboard** built with React, Node.js, Express, and PostgreSQL.  
This project features **two main roles** — **Admin** and **User** — each with distinct permissions and dashboards.  
Admins can manage users, approve requests, and control access, while users can manage their own profiles.

---

## 🚀 Features

### 👤 User Features
- View and update profile information (except email)
- Request email change (approved or rejected by admin)
- Access a clean, modern dashboard UI
- See request status updates in real time

### 🧑‍💼 Admin Features
- View all registered users in a tabular dashboard
- Approve or reject email change requests
- Promote a user to admin or demote an admin back to user
- Delete users from the database
- Block users via email ID
- Temporarily deactivate user accounts (prevent login)
- Update any user’s profile information

---

## 🧠 Tech Stack

**Frontend:** React.js  
**Backend:** Node.js, Express.js  
**Database:** PostgreSQL (hosted on [Neon.tech](https://neon.tech))  
**ORM:** Sequelize ORM  

---

## ⚙️ Installation & Setup

1. **Clone the repository**
   
   ```bash
   git clone https://github.com/Dev-Garg-1/Auth-Dashboard.git
   cd Auth-Dashboard

2. **Install Dependencies**
   
   ```bash
   # For backend
   cd backend
   npm install

   # For frontend
   cd ../frontend
   npm install
   
3. **Configure environment variables**
   
    Create a .env file in the backend folder and include:
     ```bash
     ACCESS_TOKEN_SECRET= 
     ACCESS_TOKEN_EXPIRY=
     REFRESH_TOKEN_SECRET=
     REFRESH_TOKEN_EXPIRY=
     PORT=
     NEON_DB_URI=
     CORS_ORIGIN=
    ```
  
    Create a .env file in the frontend folder and include:
     ```bash
     VITE_AUTH_URL=
     VITE_FRONTEND_URL=
    ```

4. **Run the development servers**

    ```bash
    # Backend
    npm run dev
    
    # Frontend
    npm start
    ```
