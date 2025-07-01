# 🏥 Hospital Management System

A responsive and user-friendly web application built with PHP and MySQL to streamline hospital workflows — including patient registration, appointment booking, medical records, billing, and admin/doctor management.

---

## 🎯 Features 🎯

- **Role‑based Access**  
  - **Admin**: Manage doctors, patients, appointments, payments, and feedback.  
  - **Doctor**: Approve/reject appointments, view patient history.  
  - **Patient**: Register, login, book/cancel appointments, view history, send messages.

- **Appointment Management**  
  Patients book → Admin/Doctor approve → Monitor status and cancellations.

- **Electronic Medical Records**  
  Diagnosis, prescription history, and documentation via TCPDF-generated PDFs.

- **Billing & Payments**  
  Auto-generate invoices and receipts.

- **Contact & Feedback Form**  
  Patients can directly message the admin.

- **Search & Filter**  
  Quickly find users, appointments, and records.

---

## 🛠️ Tech Stack

- **Backend**: PHP  
- **Database**: MySQL  
- **Frontend**: HTML5, CSS3, JavaScript, Bootstrap  
- **PDF**: TCPDF  
- **Local Server**: XAMPP / WAMP / LAMP  

---

## 📁 Project Structure

Hospital-management-system/
│
├── css/ # Stylesheets (Bootstrap + custom)
├── js/ # JavaScript and validation scripts
├── images/ # Icons, logos, and UI assets
├── include/ # Reusable PHP files (header, footer, authentication)
│ ├── config.php
│ ├── functions.php
│ └── db_connect.php
├── vendor/ # TCPDF and third-party dependencies
├── admin/ # Admin dashboard & management pages
│ ├── manageDoctors.php
│ ├── managePatients.php
│ ├── manageAppointments.php
│ └── billing.php
├── doctor/ # Doctor portal pages
│ ├── appointments.php
│ └── patientHistory.php
├── patient/ # Patient portal pages
│ ├── bookAppointment.php
│ ├── myAppointments.php
│ └── medicalHistory.php
├── contact.php # Feedback/contact form
├── myhmsdb.sql # Database schema & seed data
├── index.php # Homepage / login interface
├── dashboard.php # Login redirection logic
└── logout.php # Session destruction and logout
---

## 🚀 Setup & Installation

### Prerequisites

- PHP (7.x+), MySQL, Apache (via XAMPP/WAMP/LAMP)  
- TCPDF library included

### Steps

1. **Clone the repository**  
   ```bash
   git clone https://github.com/DeepakGaut/Hospital-management-system.git
Move files to your server folder (htdocs on XAMPP).

Start Apache & MySQL via XAMPP control panel.

Create database

Open http://localhost/phpmyadmin

Create: myhmsdb

Import myhmsdb.sql.

Access app:

Go to http://localhost/Hospital-management-system/

🔄 Workflow Overview
Patients: Register → Book/cancel appointments → View history → Contact admin

Doctors: Review appointment requests → Approve/reject → View patient history

Admins: Oversee all users → Manage medical records/payments → Respond to feedback

🚧 Planned Enhancements
✅ Unique email validation

🔐 Password encryption (PHP password_hash)

📄 Paginated lists (patients, doctors, appointments)

📊 Enhanced invoice formatting (Excel export support)

🔎 Advanced search filters

🛡️ Security & Validation
Basic form validation and CSRF token usage (if implemented)

Goal: improve input sanitization, role-access checks, secure file handling

💡 Contribution
Fork this repo

Create branch: feature/your-feature-name

Commit changes with clear messages

Open Pull Request for review

📞 Contact
Deepak Gaut
📧 Email: imdeepakgautam@gmail.com
🔗 GitHub: github.com/DeepakGaut
