# 🚗 WhatsNext Vision Motors – Shaping the Future of Mobility with Innovation and Excellence

Elevating Customer Experience & Operational Excellence in Automotive Retail

This project demonstrates a Salesforce-powered digital transformation for WhatsNext Vision Motors, a leader in automotive innovation. The solution is designed to streamline operations, automate workflows, and deliver a seamless customer journey from inquiry to delivery.

---

## 🚀 Project Overview

WhatsNext Vision Motors leverages Salesforce to:

- **Centralize and manage** vehicle, dealer, and customer data
- **Automate workflows** for order processing, dealer assignment, and stock validation
- **Enable real-time insights** for sales, service, and inventory teams
- **Enhance customer experience** with proactive communication and transparency

The goal: **A frictionless, efficient, and customer-centric automotive retail experience.**

---

## 🛠️ Key Features

✅ **Automated Dealer Assignment**  
Orders are auto-assigned to the nearest dealer based on customer address.

✅ **Stock Validation**  
Prevents orders for out-of-stock vehicles, ensuring only available inventory is sold.

✅ **Order Status Automation**  
Bulk order statuses are updated nightly based on real-time stock, keeping customers informed.

✅ **Proactive Email Notifications**  
Automated reminders for scheduled test drives and stock replenishment.

✅ **Efficient Test Drive & Service Tracking**  
Track bookings and service requests with ease.

---

## Folder Structure for Screenshots


```
WhatsNext Vision Motors/
│
├── Data Management-Objects/
├── Data Management-Tabs/
├── Data Management-App Manager/
├── Data Management-Fields/
├── Automation-Flows/
└── Apex and Batch Class/ 
```

---


## 📐 Data Model Highlights

**Custom Objects:**

| Object Name                  | Purpose                        | Relationships                        |
|------------------------------|--------------------------------|--------------------------------------|
| Vehicle__c                   | Stores vehicle details         | Related to Dealer & Orders           |
| Vehicle_Dealer__c            | Stores dealer info             | Related to Orders                    |
| Vehicle_Customer__c          | Stores customer details        | Related to Orders & Test Drives      |
| Vehicle_Order__c             | Tracks vehicle purchases       | Related to Customer & Vehicle        |
| Vehicle_Test_Drive__c        | Tracks test drive bookings     | Related to Customer & Vehicle        |
| Vehicle_Service_Request__c   | Tracks service requests        | Related to Customer & Vehicle        |

---

## 🏷️ Fields & Relationships

**1️⃣ Vehicle__c**
- Vehicle_Name__c (Text)
- Vehicle_Model__c (Picklist: Sedan, SUV, EV, etc.)
- Stock_Quantity__c (Number)
- Price__c (Currency)
- Dealer__c (Lookup to Dealer__c)
- Status__c (Picklist: Available, Out of Stock, Discontinued)

**2️⃣ Vehicle_Dealer__c**
- Dealer_Name__c (Text)
- Dealer_Location__c (Text)
- Dealer_Code__c (Auto Number)
- Phone__c (Phone)
- Email__c (Email)

**3️⃣ Vehicle_Order__c**
- Customer__c (Lookup to Customer__c)
- Vehicle__c (Lookup to Vehicle__c)
- Order_Date__c (Date)
- Status__c (Picklist: Pending, Confirmed, Delivered, Canceled)

**4️⃣ Vehicle_Customer__c**
- Customer_Name__c (Text)
- Email__c (Email)
- Phone__c (Phone)
- Address__c (Text)
- Preferred_Vehicle_Type__c (Picklist: Sedan, SUV, EV, etc.)

**5️⃣ Vehicle_Test_Drive__c**
- Customer__c (Lookup to Customer__c)
- Vehicle__c (Lookup to Vehicle__c)
- Test_Drive_Date__c (Date)
- Status__c (Picklist: Scheduled, Completed, Canceled)

**6️⃣ Vehicle_Service_Request__c**
- Customer__c (Lookup to Customer__c)
- Vehicle__c (Lookup to Vehicle__c)
- Service_Date__c (Date)
- Issue_Description__c (Text)
- Status__c (Picklist: Requested, In Progress, Completed)

---

## ⚙️ Technologies & Tools Used

| Tool / Feature            | Purpose                                         |
|---------------------------|-------------------------------------------------|
| Salesforce Lightning App  | Custom UI and layout creation                   |
| Record-Triggered Flows    | Real-time automation (dealer assignment, emails) |
| Apex Triggers             | Custom logic (stock validation, assignment)     |
| Batch Apex                | Nightly bulk order/status updates               |
| Validation Rules          | Data integrity at the UI level                  |
| Scheduled Apex            | Automate nightly updates for inventory/orders   |

---

## 📚 What I Learned

- Designing scalable, normalized data models in Salesforce
- Automating business logic with Flows and Apex
- Ensuring data consistency with validation rules and error handling
- Building modular Lightning apps for streamlined user experience
- Implementing batch and asynchronous Apex operations

---

## 👨‍💻 Author

**[Sidhant Kaistha]**
-Graphic Era Deemed To Be University
-B.Tech in Computer Science with Specialization in Artificial Intelligence  
-Email: [sidhantkaistha2004@gmail.com] 

---

## 🔗 Project Links

- 💻 GitHub Repository: [https://github.com/sidhantkaistha2004/Salesforce---WhatNext-Vision-Motors-Shaping-the-Future-of-Mobility-with-Innovation-and-Excellence]
- 🎥 Demo Video: Uploaded the link at the skillwallet Salesforce.

---

## 📄 License

This project is developed for educational and portfolio purposes.  
Feel free to fork, adapt, or reference it for learning.
