# Cloud---Attendance-Management-System
Attendance Management System
🕒 Cloud-Based Employee Attendance Management System

A full-stack, cloud-ready Employee Attendance Management System built using Python (Flask), SQLAlchemy, JWT Authentication, HTML/CSS, Bootstrap, and deployed on AWS EC2 with Gunicorn + Nginx.

This project simulates a real-world enterprise attendance system with role-based access (Admin & Employee), approval workflow, attendance tracking, and analytics dashboards.

🌐 Live Deployment

Deployed on AWS EC2 (Ubuntu 22.04)
🔗 http://<your-ec2-public-ip>

📌 Key Highlights

✔ Role-based Authentication (Admin / Employee)
✔ Secure JWT-based Login System
✔ Admin Approval Workflow for Employees
✔ Daily Check-In / Check-Out Tracking
✔ Monthly Attendance Charts (Chart.js)
✔ Employee Self-View Attendance Dashboard
✔ Dark Mode Support 🌙
✔ Production Deployment with Nginx & Gunicorn
✔ Cloud-Ready Architecture (AWS EC2)

🧱 Tech Stack
Frontend

HTML5

CSS3 (Custom + Dark Mode)

Bootstrap 5

JavaScript (Fetch API)

Chart.js

Backend

Python 3

Flask

Flask-SQLAlchemy

Flask-Migrate

Flask-JWT-Extended

Flask-CORS

Database

SQLite (Local / Demo)

PostgreSQL / MySQL (Cloud Ready)

Cloud & Deployment

AWS EC2

Gunicorn (WSGI Server)

Nginx (Reverse Proxy)

systemd (Service Management)

🔐 Roles & Permissions
👨‍💼 Employee

Register account

Wait for admin approval

Login using User ID + Password

Check-In / Check-Out

View personal attendance history

View monthly attendance percentage

🛡️ Admin

Admin registration

Approve / Reject employees

View all attendance records

View attendance analytics & charts

Manage employee access

📂 Project Structure
attendance-system/
│
├── backend/
│   ├── app.py
│   ├── run.py
│   ├── models.py
│   ├── settings.py
│   ├── routes/
│   │   ├── auth.py
│   │   ├── attendance.py
│   │   └── admin.py
│   ├── templates/
│   │   ├── login.html
│   │   ├── employee_login.html
│   │   ├── employee_register.html
│   │   ├── admin_register.html
│   │   ├── dashboard.html
│   │   ├── admin.html
│   │   ├── my_attendance.html
│   │   └── chart.html
│   ├── static/
│   │   └── style.css
│   ├── migrations/
│   └── requirements.txt
│
└── README.md

⚙️ Features Explained
🔑 Authentication

JWT-based authentication

Role stored inside JWT claims

Secure password hashing (Werkzeug)

🕘 Attendance System

One check-in per day per employee

Optional check-out

Timestamp-based logging

Stored securely in database

📊 Analytics & Reports

Monthly attendance count

Attendance percentage calculation

Bar charts using Chart.js

Admin-only analytics view

🧾 Approval Workflow

Employees start with pending status

Admin can approve / reject

Unapproved employees cannot login

🌙 Dark Mode

Persistent dark mode using localStorage

Toggle available on every page

🚀 Local Setup Instructions
1️⃣ Clone Repository
git clone https://github.com/yourusername/attendance-system.git
cd attendance-system/backend

2️⃣ Create Virtual Environment
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Database Migration
flask db upgrade

5️⃣ Run Application
python run.py


Visit:

http://127.0.0.1:5000

☁️ AWS Deployment (Summary)

EC2 (Ubuntu 22.04)

Gunicorn for Flask execution

Nginx reverse proxy

systemd service for reliability

📄 Full AWS deployment steps included separately

🔒 Security Measures

Password hashing (Werkzeug)

JWT authentication

Role-based access control

CORS protection

Environment variables for secrets

🧠 Learning Outcomes

✔ Full-stack Flask development
✔ REST API design
✔ Authentication & Authorization
✔ Database migrations
✔ Cloud deployment (AWS EC2)
✔ Production-grade architecture
✔ UI/UX improvements with Bootstrap
✔ Real-world workflow implementation

📸 Screenshots (Optional)

Add screenshots here:

Login Page

Employee Dashboard

Admin Dashboard

Attendance Charts

🧾 Resume-Ready Description

Cloud-Based Employee Attendance Management System
Developed a full-stack attendance management system using Flask, SQLAlchemy, JWT authentication, and Bootstrap. Implemented role-based access control, admin approval workflows, real-time attendance tracking, and analytics dashboards. Deployed the application on AWS EC2 using Gunicorn and Nginx following production best practices.

🔮 Future Enhancements

Email notifications for approvals

QR-code based attendance

Mobile responsive PWA

Docker & CI/CD pipeline

AWS RDS integration

Biometric integration simulation

🤝 Contributing

Pull requests are welcome.
For major changes, please open an issue first.

📜 License

This project is licensed under the MIT License.

⭐ Support

If you found this project helpful:

⭐ Star the repo

🍴 Fork it

🧑‍💻 Use it for learning & interviews
