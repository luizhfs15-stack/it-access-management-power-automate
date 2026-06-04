# 🚀 IT Access Management System (Power Automate)

## 🧭 Overview

This project is an automated IT Access Request and Approval system built using Microsoft Power Platform.

It simulates a real Identity and Access Management (IAM) scenario commonly found in enterprise environments, where employees request access to corporate systems and managers are responsible for approving or rejecting those requests.

The entire process is fully automated, improving control, traceability, and efficiency in IT operations.

---

## 🏗️ Architecture

The solution follows a simple but realistic enterprise workflow:

Microsoft Lists → Power Automate → Approval Engine → Outlook Notifications → SharePoint Update


Each component plays a specific role in the automation lifecycle:

- **Microsoft Lists** → stores access requests and status tracking  
- **Power Automate** → orchestrates the workflow automation  
- **Approvals** → handles manager decision-making  
- **Outlook** → delivers automated notifications  
- **SharePoint List** → persists final request status  

---

## ⚙️ Technologies Used

- 🗂️ Microsoft Lists (data storage layer)
- ⚡ Power Automate (workflow engine)
- 📩 Microsoft Outlook (email notifications)
- ✅ Microsoft Approvals (decision layer)
- 📁 SharePoint Lists (data management)
- ☁️ Microsoft 365 ecosystem
- 🔐 Identity & Access Management Concepts

---

## 📊 Solution Stack

<div align="center">

![Power Automate](https://img.shields.io/badge/Power_Automate-0066FF?style=for-the-badge&logo=powerautomate&logoColor=white)

![SharePoint](https://img.shields.io/badge/SharePoint-03787C?style=for-the-badge&logo=microsoftsharepoint&logoColor=white)

![Microsoft Lists](https://img.shields.io/badge/Microsoft_Lists-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)

![Microsoft 365](https://img.shields.io/badge/Microsoft_365-D83B01?style=for-the-badge&logo=microsoftoffice&logoColor=white)

</div>

---

## 📊 Data Structure (Microsoft Lists)

The system uses a structured data model to ensure traceability and governance:

- Employee Name  
- Email  
- Requested System  
- Justification  
- Manager  
- Status  
- ApprovedBy  
- ResponseDate  


Each field supports:

- Auditability
- Process transparency
- Access governance

---

## 🔄 Workflow Execution

### 1. Request Creation

An employee submits a new access request in Microsoft Lists, providing all required details such as justification and target system.

<p align="center">
  <img src="./images/fluxo-1.png" width="700"/>
</p>

📌 Alternative view (direct GitHub file access):

https://github.com/luizhfs15-stack/it-access-management-power-automate/blob/main/fluxo-1.png


---

### 2. Flow Trigger

Power Automate automatically detects the new entry and initiates the approval workflow without manual intervention.

<p align="center">
  <img src="./images/fluxo-2.png" width="700"/>
</p>

📌 Alternative view:

https://github.com/luizhfs15-stack/it-access-management-power-automate/blob/main/fluxo-2.png


---

### 3. Approval Process

The assigned manager receives a structured approval request and decides whether access should be granted or denied.

Possible outcomes:

- ✅ Approved  
- ❌ Rejected  

---

### 4. System Update

Once a decision is made, the system automatically updates the request record with:

- Final Status  
- Approver Name  
- Response Timestamp  

---

### 5. Notification Delivery

The requester receives an automated email informing the final decision and relevant details.

<p align="center">
  <img src="./images/sharepoint.png" width="700"/>
</p>

📌 Alternative view:

https://github.com/luizhfs15-stack/it-access-management-power-automate/blob/main/sharepoint.png


---

## 📬 Notification Scenarios

### ✅ Approved Requests

- Status updated to “Approved”
- Confirmation email sent to requester
- Request logged for audit tracking


### ❌ Rejected Requests

- Status updated to “Rejected”
- Email sent with decision notification
- Request preserved for governance tracking


---

## 🧪 Validation Process

The solution was validated through multiple end-to-end test scenarios:

- Creation of access requests in Microsoft Lists
- Automatic trigger execution in Power Automate
- Approval and rejection flows
- Data consistency validation in SharePoint
- Email notification delivery confirmation
- Execution tracking via flow run history

---

## 💡 Key Features

- End-to-end automated approval workflow
- Real-world IT access management simulation (IAM model)
- Power Automate workflow orchestration
- SharePoint integration
- Automated email notification system
- Full audit trail
- Approval history tracking
- Microsoft 365 native integration

---

## 🎯 Business Value

This solution demonstrates how organizations can modernize IT operations by:

- Reducing manual approval workload
- Improving security and access governance
- Standardizing access request processes
- Increasing operational efficiency
- Ensuring traceability and compliance


---

## 🚀 Future Enhancements

Planned improvements to extend enterprise capabilities:

- Microsoft Entra ID (Azure AD) integration
- Automated identity provisioning
- Multi-level approval workflows
- Power BI analytics dashboard
- Microsoft Teams notifications
- SLA tracking and monitoring
- Advanced audit and compliance logging


---

## 👨‍💻 Author

Developed by Luiz Henrique

Cloud Computing | Automation | IT Infrastructure | Microsoft Azure Ecosystem


---

## 📌 Project Status

✔ Fully operational  
✔ End-to-end automated workflow  
✔ Power Automate + SharePoint implemented  
✔ Enterprise-style implementation  
✔ Portfolio-ready for Cloud / Power Platform roles
