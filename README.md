A ServiceNow workflow automation project for hospital appointment management using Client Scripts and Platform Analytics.

 🚀 Hospital Appointment System using ServiceNow

A workflow automation project developed using **ServiceNow Studio**, **Client Scripts**, and **Platform Analytics** to automate patient registration and doctor appointment scheduling


📌 Project Overview

The **Hospital Appointment System** is a custom ServiceNow application that automates the appointment scheduling process. Patients or receptionists can submit appointment requests, automated scripts validate dates in real-time, and administrators can monitor appointments using an interactive dashboard.


✨ Features

* ✅ Patient Registration & Appointment Request Form
* ✅ Dynamic Client-Side Date Validation Script
* ✅ Real-Time Appointment Status Tracking
* ✅ Custom Data Model Architecture
* ✅ Platform Analytics Dashboard
* ✅ Analytics & Reporting Visualizations

 🛠️ Technologies Used

* ServiceNow
* ServiceNow Studio
* JavaScript 
* Platform Analytics
* Reports
* Dashboards
* Custom Tables

 🔄 Workflow

Patient / Receptionist ⬇️

Submit Appointment Request ⬇️

Client Script Validation Trigger ⬇️

Past Date Intercepted & Blocked ⬇️

Appointment Saved as Pending ⬇️

Dashboard & Reports Updated


 📊 Dashboard Components

* 📌 Total Appointments 
* 📌 Appointments Status Distribution (Donut Chart)
* 📌 Appointments by Doctor (Bar Chart)
* 📌 Active Patients Overview 

📁 Project Structure

Hospital Appointment System
│
├── Appointment Request Form
├── Custom Tables (Patients, Doctors, Appointments)
├── Client Scripts (Prevent Past Dates)
├── Reports
├── Dashboard
└── Platform Analytics

🚀 Future Enhancements

* 📩 **Automated Email & SMS Notifications:** Integrate Flow Designer to send automatic confirmation and reminder alerts to patients prior to their scheduled time.
* 🗓️ **Doctor Calendar & Slot Availability View:** Implement a dynamic visual calendar interface so patients can view open time slots in real time.
* 🤖 **AI-Powered Virtual Assistant (Virtual Agent):** Deploy a ServiceNow Virtual Agent chatbot allowing patients to book, reschedule, or cancel appointments via conversational AI.
* 💳 **Payment & Billing Integration:** Connect payment gateway APIs to handle pre-consultation fee processing directly within the patient portal.
* 📱 **ServiceNow Mobile App Access:** Configure Mobile Studio views to enable doctors and medical personnel to manage daily appointments from mobile devices.


 🎯 Business Rules & Logic

* **Client-Side Validation (`onChange` Client Script):**
  * Triggers when the user selects an appointment date
  * Compares input against current date and time.
  * Displays a field error and clears input if a past date is chosen.

* **Server-Side Automation (Business Rule):**
  * Executes `before` insert/update on the `x_1959100_hospit_0_appointment` table.
  * Auto-generates unique appointment identifiers (e.g., `APP0001011`)
  * Sets initial appointment status to `Pending` if left empty
  * Sanitizes input data before writing directly to the database.

* **Real-Time Data Propagation:**
  * Saved appointments update relational counts across `Patients` and `Doctors` tables.
  * Real-time metrics flow into the Platform Analytics Dashboard automatically.

📷 Screenshots



