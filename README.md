# **Job Portal Application**

A full-stack job portal connecting job seekers with employers, built using **Node.js, Express, MySQL, and EJS**.

---

## **Project Structure**
```
job-portal-main/
│── config/              # Configuration files (e.g., database settings)
│   └── config.js
│── controllers/         # Controller functions for handling requests
│── middleware/          # Middleware for authentication and validation
│── migrations/          # Sequelize migrations for database setup
│── models/              # Database models using Sequelize
│── node_modules/        # Dependencies (excluded via .gitignore)
│── public/              # Static files (CSS, JS, Images)
│── routes/              # API and web routes
│── views/               # EJS templates for frontend rendering
│   ├── adminDashboard.ejs
│   ├── companyRegister.ejs
│   ├── employerDashboard.ejs
│   ├── home.ejs
│   ├── jobDashboard.ejs
│   ├── jobseekerDashboard.ejs
│   ├── login.ejs
│   ├── register.ejs
│── .env                 # Environment variables (excluded via .gitignore)
│── .gitignore           # Files and directories to ignore in Git
│── app.js               # Main entry point of the application
│── package.json         # Project dependencies and scripts
│── package-lock.json    # Lockfile for package dependencies
│── README.md            # Project documentation
```

---

## **Features**
- Secure authentication for **Job Seekers** and **Employers**
- Job posting and application management
- Resume upload functionality
- User role-based dashboards (Admin, Employer, Job Seeker)
- Application tracking system
- Secure password hashing and session-based authentication
- Responsive user interface with EJS templating

---

## **Technologies Used**

### **Frontend**
- **HTML5**
- **CSS3**
- **EJS** (Embedded JavaScript Templates)

### **Backend**
- **Node.js**
- **Express.js**

### **Database**
- **MySQL**
- **Sequelize ORM**

### **Dependencies**
- **bcrypt** (Password hashing)
- **cookie-parser** (Session management)
- **dotenv** (Environment variables)
- **express-session** (Session handling)
- **jsonwebtoken** (JWT authentication)
- **multer** (File uploads)
- **mysql2** (MySQL connection)
- **nodemon** (Development server auto-restart)

---

## **Installation and Setup**

### **1. Clone the Repository**
```bash
git clone https://github.com/Shishir1008/JobPortalElevateWorkforceSolutions.git
cd JobPortalElevateWorkforceSolutions
```

### **2. Install Dependencies**
```bash
npm install
```

### **3. Configure Database**
- Create a MySQL database:
```sql
CREATE DATABASE job_portal;
```
- Update database credentials in `config/config.js`
- Run migrations to set up tables:
```bash
npx sequelize-cli db:migrate
```

### **4. Set Up Environment Variables**
Create a `.env` file in the root directory:
```env
PORT=3000
JWT_SECRET=your_jwt_secret_key
```

### **5. Start the Server**
```bash
npm start
```

### **6. Access the Application**
Open a browser and visit:
```
http://localhost:3000
```

---

## **Future Improvements**
- Implement real-time job notifications
- Add profile picture upload functionality
- Improve UI with modern frontend frameworks like React

---

