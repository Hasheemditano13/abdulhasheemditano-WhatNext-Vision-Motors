# abdulhasheemditano-WhatNext-Vision-Motors

# 🚗 WhatNext Vision Motors
### Shaping the Future of Mobility with Innovation and Excellence

**Developer:** Abdul Hasheem O. Ditano  
**Institution:** Asia Pacific College  
**Course:** BS – Information Technology (MI-222)

---

## 📘 Overview

**WhatNext Vision Motors** is a Salesforce-based application designed to streamline vehicle management for automotive businesses.  
The system manages vehicles, dealers, customers, test drives, and service requests efficiently, leveraging **Salesforce Lightning**, **Apex triggers**, **batch jobs**, and **automation flows**.

This project demonstrates Salesforce development capabilities through **custom objects**, **automations**, and **scheduled batch processes** for data handling and business process optimization.

---

## ⚙️ Features

### 1. **Custom Objects**
The system includes several custom objects for managing business entities:
- **Vehicle__c** – Stores vehicle details such as model, type, and stock quantity.
- **Vehicle_Dealer__c** – Contains dealership information.
- **Vehicle_Order__c** – Manages customer vehicle purchase records.
- **Vehicle_Customer__c** – Stores customer details.
- **Vehicle_Test_Drive__c** – Tracks customer test drive activities.
- **Vehicle_Service_Request__c** – Records maintenance or service requests.

### 2. **Lightning App Creation**
A dedicated **Lightning App** was created to provide an integrated interface for managing vehicles, orders, and services.  
Each custom object is accessible through the app’s navigation for seamless interaction.

### 3. **Automation Flows**
Salesforce Flows were implemented to enhance user experience and automate manual tasks:
- **Auto Assign Dealer** – Automatically assigns the appropriate dealer to a vehicle or order.
- **Test Drive Reminder** – Sends reminders or notifications for upcoming test drives.

### 4. **Apex Classes and Triggers**
Custom Apex code was written to handle specific logic and background processes.

#### 🔹 Apex Components
| Component | Description |
|------------|-------------|
| `VehicleOrderTriggerHandler` | Contains reusable methods for handling vehicle order trigger logic. |
| `VehicleOrderTrigger` | Trigger that invokes the handler when records in `Vehicle_Order__c` are created or updated. |
| `VehicleOrderBatch` | Batch Apex job that processes large volumes of vehicle order data efficiently. |
| `VehicleOrderBatchScheduler` | Schedules batch jobs at defined intervals to automate data updates. |

### 5. **Batch and Trigger Jobs**
These Apex jobs ensure that processes such as stock updates, dealer assignment, and service reminders run automatically without manual intervention.

---

## 🧠 Business Logic Example

**Scenario:**  
When a vehicle order is created, the system checks the stock quantity.  
- If the **stock quantity is 0**, appropriate handling is triggered to prevent over-ordering or to initiate restocking workflows.  
- Batch jobs can also handle periodic checks and updates to ensure stock accuracy.

---

## 🧩 Technology Stack

- **Platform:** Salesforce (Lightning Experience)
- **Language:** Apex
- **Automation:** Salesforce Flows & Scheduled Batch Jobs
- **Database:** Salesforce Object Storage (Custom Objects)
- **Interface:** Lightning App

---

## 🚀 How to Run

1. Log in to your Salesforce Developer Org.
2. Create the required **Custom Objects** (`Vehicle__c`, `Vehicle_Dealer__c`, `Vehicle_Order__c`, etc.).
3. Create the **Lightning App** and include the related object tabs.
4. Upload and deploy the following **Apex Classes**:
   - `VehicleOrderTriggerHandler`
   - `VehicleOrderTrigger`
   - `VehicleOrderBatch`
   - `VehicleOrderBatchScheduler`
5. Set up the **Flows**:
   - Auto Assign Dealer
   - Test Drive Reminder
6. Deploy and test automation using sample records.

---

## 📅 Future Enhancements

- Integration with third-party APIs for real-time vehicle data.
- Enhanced reporting dashboards for sales and service analytics.
- Custom notifications via email or SMS for test drive and service updates.

---

## 📜 Author

**Abdul Hasheem O. Ditano**  
Bachelor of Science in Information Technology  
Asia Pacific College – MI-222

---

