A ServiceNow workflow automation project for hospital appointment management using Client Scripts and Platform Analytics.

 🚀 Hospital Appointment System using ServiceNow

A workflow automation project developed using **ServiceNow Studio**, **Client Scripts**, and **Platform Analytics** to automate patient registration and doctor appointment scheduling[span_0](start_span)[span_0](end_span)[span_1](start_span)[span_1](end_span).


📌 Project Overview

The **Hospital Appointment System** is a custom ServiceNow application that automates the appointment scheduling process[span_2](start_span)[span_2](end_span)[span_3](start_span)[span_3](end_span). Patients or receptionists can submit appointment requests, automated scripts validate dates in real-time, and administrators can monitor appointments using an interactive dashboard[span_4](start_span)[span_4](end_span)[span_5](start_span)[span_5](end_span).


✨ Features

* ✅ Patient Registration & Appointment Request Form[span_6](start_span)[span_6](end_span)[span_7](start_span)[span_7](end_span)
* ✅ Dynamic Client-Side Date Validation Script[span_8](start_span)[span_8](end_span)[span_9](start_span)[span_9](end_span)
* ✅ Real-Time Appointment Status Tracking[span_10](start_span)[span_10](end_span)[span_11](start_span)[span_11](end_span)
* ✅ Custom Data Model Architecture[span_12](start_span)[span_12](end_span)[span_13](start_span)[span_13](end_span)
* ✅ Platform Analytics Dashboard[span_14](start_span)[span_14](end_span)[span_15](start_span)[span_15](end_span)
* ✅ Analytics & Reporting Visualizations[span_16](start_span)[span_16](end_span)[span_17](start_span)[span_17](end_span)

 🛠️ Technologies Used

* ServiceNow[span_18](start_span)[span_18](end_span)[span_19](start_span)[span_19](end_span)
* ServiceNow Studio[span_20](start_span)[span_20](end_span)[span_21](start_span)[span_21](end_span)
* JavaScript (GlideForm API & Client Scripts)[span_22](start_span)[span_22](end_span)[span_23](start_span)[span_23](end_span)
* Platform Analytics[span_24](start_span)[span_24](end_span)[span_25](start_span)[span_25](end_span)
* Reports[span_26](start_span)[span_26](end_span)[span_27](start_span)[span_27](end_span)
* Dashboards[span_28](start_span)[span_28](end_span)[span_29](start_span)[span_29](end_span)
* Custom Tables[span_30](start_span)[span_30](end_span)[span_31](start_span)[span_31](end_span)

 🔄 Workflow

Patient / Receptionist ⬇️

Submit Appointment Request ⬇️

Client Script Validation Trigger ⬇️

Past Date Intercepted & Blocked ⬇️

Appointment Saved as Pending ⬇️

Dashboard & Reports Updated


 📊 Dashboard Components

* 📌 Total Appointments (Single Score)[span_32](start_span)[span_32](end_span)[span_33](start_span)[span_33](end_span)
* 📌 Appointments Status Distribution (Donut Chart)[span_34](start_span)[span_34](end_span)[span_35](start_span)[span_35](end_span)
* 📌 Appointments by Doctor (Bar Chart)[span_36](start_span)[span_36](end_span)[span_37](start_span)[span_37](end_span)
* 📌 Active Patients Overview (List View)[span_38](start_span)[span_38](end_span)[span_39](start_span)[span_39](end_span)


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

* 📩 **Automated Email & SMS Notifications:** Integrate Flow Designer to send automatic confirmation and reminder alerts to patients prior to their scheduled time[span_0](start_span)[span_0](end_span)[span_1](start_span)[span_1](end_span).
* 🗓️ **Doctor Calendar & Slot Availability View:** Implement a dynamic visual calendar interface so patients can view open time slots in real time.
* 🤖 **AI-Powered Virtual Assistant (Virtual Agent):** Deploy a ServiceNow Virtual Agent chatbot allowing patients to book, reschedule, or cancel appointments via conversational AI.
* 💳 **Payment & Billing Integration:** Connect payment gateway APIs to handle pre-consultation fee processing directly within the patient portal.
* 📱 **ServiceNow Mobile App Access:** Configure Mobile Studio views to enable doctors and medical personnel to manage daily appointments from mobile devices.


 🎯 Business Rules & Logic

* **Client-Side Validation (`onChange` Client Script):**
  * Triggers when the user selects an appointment date[span_26](start_span)[span_26](end_span)[span_27](start_span)[span_27](end_span).
  * Compares input against current date and time[span_28](start_span)[span_28](end_span)[span_29](start_span)[span_29](end_span).
  * Displays a field error and clears input if a past date is chosen[span_30](start_span)[span_30](end_span)[span_31](start_span)[span_31](end_span).

* **Server-Side Automation (Business Rule):**
  * Executes `before` insert/update on the `x_1959100_hospit_0_appointment` table.
  * Auto-generates unique appointment identifiers (e.g., `APP0001011`)[span_32](start_span)[span_32](end_span).
  * Sets initial appointment status to `Pending` if left empty[span_33](start_span)[span_33](end_span)[span_34](start_span)[span_34](end_span).
  * Sanitizes input data before writing directly to the database.

* **Real-Time Data Propagation:**
  * Saved appointments update relational counts across `Patients` and `Doctors` tables[span_35](start_span)[span_35](end_span)[span_36](start_span)[span_36](end_span).
  * Real-time metrics flow into the Platform Analytics Dashboard automatically[span_37](start_span)[span_37](end_span)[span_38](start_span)[span_38](end_span).





