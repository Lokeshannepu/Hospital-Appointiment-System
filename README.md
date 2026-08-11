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

📷 Screenshots
AppEngine Studio
<img width="1915" height="912" alt="App Engine Studio" src="https://github.com/user-attachments/assets/5b00eb9e-49ba-4bdb-84cf-9948b6fea82c" />
<img width="1901" height="876" alt="Dashboard" src="https://github.com/user-attachments/assets/0cc1e232-7ffb-41d0-b5bb-fe17290cd5ce" />
<img width="1816" height="837" alt="Appointment Record" src="https://github.com/user-attachments/assets/7bab99a8-41a9-451e-b3ee-7803a92b5b14" />
<img width="1370" height="772" alt="Hospital_Appointment_System_Architecture" src="https://github.com/user-attachments/assets/094c29b8-0bc6-4032-9e3a-260adf5fe863" />
<img width="987" height="636" alt="Flow" src="https://github.com/user-attachments/assets/a7a1e9ea-63b6-43bc-b2b4-918db529b8d9" />
<img width="1823" height="882" alt="Client Script" src="https://github.com/user-attachments/assets/26c14fc0-428f-485f-b97b-8c014bb4777e" />
<img width="1465" height="847" alt="Doctor Schedule" src="https://github.com/user-attachments/assets/24f72742-f745-40de-a30c-cfdc0f10241f" />
<img width="1458" height="690" alt="Doctor" src="https://github.com/user-attachments/assets/e63c375c-2a54-4ad1-abc6-f689b9b418ee" />
<img width="1466" height="710" alt="Patient" src="https://github.com/user-attachments/assets/f540a6fb-4884-4a6d-9a3b-5fe62456f4d0" />




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




