# 🏥 Hospital Management System (HMS)

<div align="center">

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)

### 🌐 [Live Demo](https://project1.webtlb.it)

*A comprehensive web-based solution for modern hospital administration*

</div>

---

## 📋 Table of Contents
- [Introduction](#-introduction)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Database Setup](#-database-setup)
- [User Roles](#-user-roles)
- [Screenshots](#-screenshots)
- [Future Scope](#-future-scope)
- [Author](#-author)

---

## 📖 Introduction

The **Hospital Management System (HMS)** is a web-based application designed to streamline and automate the administrative and clinical operations of a hospital. It replaces manual, paper-based systems with a digital solution that efficiently manages:

- 👥 Patient information
- 👨‍⚕️ Doctor schedules
- 📅 Appointments
- 📋 Medical records

The system provides a centralized platform for **Admins**, **Doctors**, and **Patients** to interact and perform their respective tasks seamlessly.

---

## ✨ Features

### 🎯 Core Objectives

| Objective | Description |
|-----------|-------------|
| ⚡ **Efficiency** | Reduce time spent on manual record-keeping and appointment scheduling |
| 🌍 **Accessibility** | Allow patients to book appointments and view medical history online from anywhere |
| 🔒 **Data Integrity** | Centralize data storage to minimize errors and ensure consistency |
| 📊 **Management Control** | Provide administrators with comprehensive management tools |

### 🔑 Key Modules

#### 🔐 Admin Module
The Administrator has full control over the system:
- 📊 **Dashboard**: Overview of system statistics (Total Doctors, Users, Appointments)
- 👨‍⚕️ **Doctor Management**: Add, edit, and delete doctor profiles; Manage specializations
- 👥 **User Management**: View and manage registered patients/users
- 📅 **Appointment Management**: View all appointments and their status
- 🔍 **Session Logs**: Monitor user and doctor login logs for security auditing
- 📧 **Inquiries**: Manage "Contact Us" queries

#### 👨‍⚕️ Doctor Module
Doctors can manage their schedules and patient interactions:
- 🏠 **Dashboard**: Personal overview of appointments
- 📅 **Appointment Management**: View log of scheduled appointments
- 🏥 **Patient Management**: Add and manage patient details
- 📋 **Medical History**: Add and view medical history records for patients
- ⚙️ **Profile Management**: Update personal details and consultancy fees

#### 🧑‍🤝‍🧑 User (Patient) Module
Patients can access services without visiting the hospital physically:
- 🔐 **Registration/Login**: Secure account creation and authentication
- 📅 **Book Appointment**: Schedule appointments with doctors based on specialization and availability
- 📜 **Appointment History**: View past and upcoming appointments
- 🩺 **Medical History**: Access personal medical records added by doctors
- 👤 **Profile Management**: Update personal information and password

---

## 🛠️ Tech Stack

### Architecture
The project is built using a standard **LAMP/WAMP** stack:

| Layer | Technology |
|-------|-----------|
| 🎨 **Frontend** | HTML5, CSS3, JavaScript/jQuery, Bootstrap |
| ⚙️ **Backend** | PHP (Core PHP) |
| 🗄️ **Database** | MySQL (RDBMS) |
| 🖥️ **Server** | Apache (via XAMPP/WAMP) |

---

## 💻 Installation

### Prerequisites
- 🖥️ XAMPP/WAMP/LAMP server
- 🌐 Modern web browser
- 📦 PHP 7.4 or higher
- 🗄️ MySQL 5.7 or higher

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/hospital-management-system.git
   ```

2. **Move to server directory**
   ```bash
   # For XAMPP
   mv hospital-management-system C:/xampp/htdocs/

   # For WAMP
   mv hospital-management-system C:/wamp64/www/
   ```

3. **Import the database**
   - Open phpMyAdmin (`http://localhost/phpmyadmin`)
   - Create a new database named `hms`
   - Import the `hms.sql` file from the project root

4. **Configure database connection**
   - Update database credentials in configuration files if needed

5. **Access the application**
   ```
   http://localhost/hospital-management-system/main/index.php
   ```

---

## 🗄️ Database Setup

The database (`hms`) consists of several normalized tables:

| Table | Description |
|-------|-------------|
| 🔑 `admin` | Admin credentials |
| 👥 `users` | Patient registration details |
| 👨‍⚕️ `doctors` | Doctor profiles (Specialization, Fees, Contact) |
| 🏷️ `doctorspecilization` | Lookup table for specializations |
| 📅 `appointment` | Links Users and Doctors with appointment details |
| 🏥 `tblpatient` | Detailed patient records |
| 📋 `tblmedicalhistory` | Medical records (BP, Sugar, Weight, Prescription) |
| 📊 `userlog` / `doctorslog` | Audit tables for login/logout tracking |
| 📧 `tblcontactus` | Contact form messages |

---

## 👥 User Roles

### Default Login Credentials
(Check `Login Details.txt` in the project root)

| Role | Access Level |
|------|--------------|
| 🔐 **Admin** | Full system control |
| 👨‍⚕️ **Doctor** | Patient management & medical records |
| 🧑‍🤝‍🧑 **Patient** | Appointment booking & medical history |

---

## 📸 Screenshots

### 🏠 Home Page
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/9c96ffcb-2bef-484b-a996-548fde802a26" width="600">
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/f960b36c-a726-4e02-8416-0284d2f1f9e9" width="600">
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/4c583894-e124-4606-a971-c9925bdf23ad" width="600">

### 🔐 Admin Login
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/52b69f80-9912-418b-b6e0-df47c4c2447c" width="600">

### 📊 Admin Dashboard
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/439231fb-ee57-4e7f-8625-586436866e1b" width="600">

### 👨‍⚕️ Manage Doctors
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/8909c579-3ac2-46c0-a7d4-f7f323d23ebc" width="600">

### 👥 Manage Users
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/d7e1b1e4-813f-4742-9cbf-32a94a4749ac" width="600">

### 📅 Appointment History
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/b01f5276-f3e7-4318-90a5-3b86b3f77efb" width="600">

### 🔍 Doctor Session Logs
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/78b3771a-8c40-483d-9fc1-e308cf993c63" width="600">

### 📊 User Session Logs
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/da39ced7-edd0-4fd3-b3ee-452f1f29f8c3" width="600">

### 👨‍⚕️ Doctor Login
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/93fcb022-7966-462d-bf74-986fc719da56" width="600">

### 🏥 Doctor Dashboard
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/eae4aaad-e92a-4cce-91f7-a9730eef90a2" width="600">

### 🧑‍🤝‍🧑 Patient Dashboard
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/2e881744-4ad4-4cc3-b5c0-c120e6f86933" width="600">

### 📅 Book Appointment
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/46581076-eaba-4538-a868-8a445642d015" width="600">

### 🧾 Appointment Receipt
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/e054e4de-3775-4c69-8dac-03ca4b45522e" width="600">
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/7e241d03-f6e1-4cca-bcff-69588ab3a206" width="600">
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/481f73a6-a5a1-4f38-87e3-dcab6d5f446b" width="600">
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/07219741-63a4-4702-b7fb-a262a8889079" width="600">

### 📥 Downloaded Receipt
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/ffa17dde-3bea-4b9d-bcd0-982cca0ab6c4" width="600">

### 📄 Receipt Download Feature
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/806626c2-68d8-4bfd-b5e2-6a46c1c107ed" width="600">

### ✏️ Edit Profile
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/d792c517-1fb9-492b-9ebf-7ec940b07c18" width="600">

### 📝 Patient Registration
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/7680678d-cdcb-45ea-a7b3-729d7654dfb9" width="600">

### 🗄️ Database Overview
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/d90bfd30-fbc8-4206-832c-2eb685f43307" width="600">

### 📐 Database Schema Design
<img src="https://github.com/Karthikg1908/Hospital-Management-System/assets/86306862/71e01826-2737-4491-8020-497922f60a3a" width="600">

---

## 🚀 Future Scope

The following features are planned for future releases:

| Feature | Description |
|---------|-------------|
| 💳 **Payment Gateway Integration** | Online payment for consultancy fees |
| 💊 **Pharmacy Module** | Integration with hospital pharmacy for medicine inventory and billing |
| 🔬 **Lab Management** | Managing lab tests and reports |
| 📱 **Mobile Application** | Dedicated mobile app for easier access |
| 🎥 **Telemedicine Integration** | Video consultation features |
| 📊 **Analytics Dashboard** | Advanced reporting and analytics |
| 🔔 **SMS/Email Notifications** | Automated appointment reminders |

---

## 👨‍💻 Author

**Mehdi Talebikatir**  
📧 Email: [your-email@example.com](mailto:your-email@example.com)  
🎓 Matricola: 558948  
🌐 Live Demo: [https://project1.webtlb.it](https://project1.webtlb.it)

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 🙏 Acknowledgments

- Bootstrap for the responsive UI framework
- PHP community for excellent documentation
- All contributors who helped improve this system

---

<div align="center">

### ⭐ If you found this project helpful, please give it a star!

**Made with ❤️ for better healthcare management**

</div>

