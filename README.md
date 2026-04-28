# QR-Based Lost & Found Management System

# 📌 Project Overview
The QR-Based Lost & Found Management System is a full-stack web application designed to modernize traditional lost and found systems using QR technology.
Each registered item generates a unique QR code. When scanned, it directs the finder to a secure public page where the owner can be notified via email.

# 🎯 Objectives

- Implement secure user authentication
- Maintain structured database relationships
- Generate unique QR codes per item
- Enable role-based admin access
- Send automated email notifications
- Maintain data integrity and validation

# 🏗 System Architecture

## Frontend:

- EJS
- Bootstrap 5
- Backend:
- Node.js
- Express.js

## Database:

- MongoDB

## Other Integrations:

- QR Code generator
- Nodemailer for email notifications
- Session-based authentication

## 🗂 Database Design
### Entities
- Users
- user_id (Primary Key)
- name
-   email (Unique)
- password
- role

### Items

- item_id (Primary Key)
- item_name
- description
- status
- owner_id (Foreign Key → Users)

### Reports

- report_id (Primary Key)
- item_id (Foreign Key → Items)
- reporter_email
- timestamp

### Relationships:

- One User → Many Items
- One Item → Many Reports

# 🔐 Role-Based Access

## User Role:

- Add items
- Mark lost/found
- View personal items

## Admin Role:

- View all users
- Promote/Demote users
- Delete users
- View analytics

# 📧 Email Notification System

## When:
- Item marked as lost
- Item marked as found

## Then:

- Owner receives automated email notification

# ⚙️ Key Features

- Secure login & signup
- QR-based item identification
- Public scan view (limited info)
- Admin dashboard
- Data validation
- Clean responsive UI

# 🚀 Future Enhancements

- Cloud deployment (AWS/Render)
- SMS integration
- Mobile app version
- Advanced analytics dashboard
- Security hardening

# 👨‍💻 Authors

VALABOJU SHIVA KUMAR CHARY, DIVYA SAI SUKANYA INDALA, SUSHMITHA SANA, SATVICK YADLAPALLI
DBMS 4560/5560 Semester Project

# Github Link : https://github.com/2000031041-ShivaChary196/DBMS_Class
