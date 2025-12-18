# Medislot

## A Full Stack Doctor Appointment Booking and Payment System

---

## 1. Introduction

Medislot is a full stack web application created to make the process of booking doctor appointments easier and more efficient. In many small clinics and hospitals, appointment booking is still handled manually, which often leads to confusion, long waiting times, and poor record keeping. This project was developed to address these problems by providing a simple and organized digital solution.

The application allows users to register, log in, choose doctors, book available time slots, and make payments online. The main purpose of this project is academic learning. It focuses on understanding how real-world web applications are built using frontend, backend, database, and payment gateway integration.

---

## 2. Problem Statement

The traditional methods of arranging an appointment are highly manual and inefficient. Patients have no concept of the availability of the doctors, and the organizing of the schedule is not apt at the clinics.Because of this paitents faced lots of issues.
The problem being solved by the project is the fact that there is no digital platform that can handle appointments, store data safely, and enable payments to be made from the internet conveniently.

---

## 3. Objectives of the Project

The goals of this project are:

* Designing and implementing a web application using the full stack approach.
* For a seamless process of scheduling an appointment
* To prevent conflicting appointment slots
* For secure user authentication flow
* To incorporate online payment systems
* To have hands-on experience with the latest web technology

---

## 4. Scope of the Project

This system is centered on appointment booking and payment. This system is best suited for small clinics or can be developed by students. The system does not incorporate advanced functionalities such as management of personnel, prescription, or medical reports.

The purpose of this project has limitations to educational and demo projects.

---

## 5. System Architecture

Medislot has a pretty straightforward client-server-based design. The frontend is involved in user interaction, while the backend performs the functions of authentication, database, payment gateways, and all business processes.

### Architecture Components

* **Frontend**: User interface built using React
* **Backend**: REST API built using Node.js and Express
* **Database**: MongoDB for storing application data
* **External API integration**:

  * Stripe for online card payments
  * Razorpay for order-based payments
  * Cloudinary for storing profile images

---

## 6. Technology Stack

### Frontend

* React (Vite)
* HTML, CSS, JavaScript
* Axios for API communication

### Backend

* Node.js
* Express.js
* MongoDB
* JWT for authentication

### Payment Gateways

* Stripe
* Razorpay

---

## 7. Functional Modules

### User Module

Users can register, login, edit their profile, schedule an appointment, view history of appointments, and pay.

### Doctor Module

The doctor has slots of availability predefined. These slots get automatically updated when an appointment is canceled or made.

### Appointment Management Module

This module deals with bookings, validation of time slots, and cancelling appointments.

### Payment Module

Appointments payments can be done through Stripe payment and Razorpay payment. Once the payment is successful, the appointment status is updated.

---

## 8. Data Flow Description

### Appointment Booking Process

1. User chooses the doctor and the preferred time slot
2. Request is sent to backend
3. Backend checks the slot availability
4. Appointment is saved into the database
5. Slot RTSV = Slot booked

### Payment Process

1. Payment is made by the user
2. Backend payment session or order creation
3. User completes payment on gateway page
4. The backend checks the payment
5. Appointment payment status is updated
---

## 9. Database Design

This project uses MongoDB database.The key collections in the project are:

* **Users**: Stores user details and login information
* **Doctors**: Stores doctor information and availability
* **Appointments**: Stores appointment details and payment status

This design helps in maintaining data consistency and easy retrieval.

---

## 10. Security Implementation

Basic security practices have been adopted to safeguard user information. Passwords are encrypted before saving them into the database.The JWT system is used as a middleware to protect and verify the some private endpoint and required credencial are stored in enviroment file.

The verification of payments has been simplified and is meant or educational prupose.

---

## 11. Software and Hardware Requirements

### Software Requirements

* Node.js (version 16 or above)
* MongoDB (Local or Atlas)
* Any modern web browser (Chrome)
* Code editor such as VS Code

### Hardware Requirements

* Minimum 4GB RAM
* Stable internet connection

---

## 12. How to Run the Project
###Step 1: Clone the GitHub Repository
```
git clone https://github.com/banteepandey2004-del/MediSlot.git
cd Medislot
```
### Backend Setup

```bash
cd backend
npm install
npm start
```

Create a `.env` file with the following details:

```
ADMIN_EMAIL = "admin@gmail.com"
ADMIN_PASSWORD = "Admin@123"
MONGODB_URI="mongodb+srv://appointmentbookingDB:Welcome100@cluster0.q1dfpow.mongodb.net/?appName=Cluster0"
CLOUDINARY_NAME=djsqsbfee
CLOUDINARY_API_KEY=838291777251164
CLOUDINARY_SECRET_KEY=IAaLnj_aEwmF0APdQ5Gxg8N1Sew
JWT_SECRET=bantee123456
CURRENCY=EUR
RAZORPAY_KEY_SECRET = 7N9FNiAg2hl2uGS0nUgj8n0D
RAZORPAY_KEY_ID = rzp_test_RrbAKsiP9Lf51t 

STRIPE_PUBLIC_KEY = pk_test_51SeK7tPOlcsm14bKbMlWix0ZiE1EifBUOJczBiFXnv4K5Jp5zKKiILpFGt3aRNEKFaweLbCOKKLtUdDQsR83PrHl000um6e3Mz
STRIPE_SECRET_KEY = sk_test_51SeK7tPOlcsm14bKTic48Xjuxx2lWZYbe2V9wSjrwvJ6xV3lHkl50Gnrf942Y1xNyciApl6Mubcj5DPv3ICDeaQe00UlqAXUDR
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

### Create .env file in frontend folder and add this
```
VITE_BACKEND_URL = http://localhost:4000
VITE_RAZORPAY_KEY_ID = razorpay_key_id
```
---
### Demo card credentials for stripe and Razorpay
```
Stripe_card_number = 4242424242424242
date = any future  cvv = any number

RazarPay_card_number = 4386 2894 0766 0153
date = any future  cvv = any number
```
### 13. Demo Credentials (For Academic Use Only)

```text
Admin Email: admin@example.com
Admin Password: admin123
```
###also create a env file admin folder and add backend url as a enviorment variable
```
VITE_BACKEND_URL = "http://localhost:4000"
```
---  

## 14. Limitations

* Payment verification is basic and not production-ready
* No advanced role management
* Limited scalability

---

## 15. Future Enhancements

* Proper payment verification using webhooks
* Admin dashboard for better control
* Notification system for appointments
* Improved security features

---

## 16. Conclusion

Medislot: Medislot is a learning-oriented full-stack project, which showcases the functionality of modern web applications. Medislot assisted the understanding of the integration of the frontend and backend, the concepts of database management, authentication, and payment systems. The project accomplished the academic aims.

---

## 17. References

* Stripe Official Documentation
* Razorpay Official Documentation
* MongoDB Documentation
* Node.js Documentation
