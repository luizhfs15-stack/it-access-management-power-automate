# 🚀 IT Access Management System (Power Automate)

## 🧭 Overview

This project is an automated IT Access Request and Approval system built using Microsoft Power Platform.

It simulates a real Identity and Access Management (IAM) scenario commonly found in enterprise environments, where employees request access to corporate systems and managers are responsible for approving or rejecting those requests.

The entire process is fully automated, improving control, traceability, and efficiency in IT operations.

---

## 🏗️ Architecture

The solution follows a realistic enterprise workflow:

Microsoft Lists → Power Automate → Approval Engine → Outlook Notifications → SharePoint Update → Python Reporting


Each component plays a specific role:

- **Microsoft Lists** → stores access requests and status tracking
- **Power Automate** → orchestrates workflow automation
- **Approvals** → handles manager decisions
- **Outlook** → sends automated notifications
- **SharePoint List** → stores final request information
- **Python Script** → generates operational reports and analysis

---

## ⚙️ Technologies Used

- 🗂️ Microsoft Lists
- ⚡ Power Automate
- 📩 Microsoft Outlook
- ✅ Microsoft Approvals
- 📁 SharePoint
- 🐍 Python Automation
- ☁️ Microsoft 365 Ecosystem


---

## 📊 Data Structure (Microsoft Lists)

The system uses a structured data model:

- Employee Name
- Email
- Requested System
- Justification
- Manager
- Status
- ApprovedBy
- ResponseDate


Each field supports:

- Audit tracking
- Governance
- Process transparency


---

# 🔄 Workflow Execution


## 1. Request Creation

An employee submits an access request through Microsoft Lists.

<p align="center">
<img src="./images/fluxo-1.png" width="700"/>
</p>



---

## 2. Flow Trigger

Power Automate detects the new request automatically.

<p align="center">
<img src="./images/fluxo-2.png" width="700"/>
</p>



---

## 3. Approval Process

The manager receives an approval request.

Possible results:

- ✅ Approved
- ❌ Rejected


---

## 4. System Update

After approval:

The system updates:

- Status
- Approver
- Response date


---

## 5. Notification Delivery


The requester receives the final decision.

<p align="center">
<img src="./images/sharepoint.png" width="700"/>
</p>


---

# 🐍 Python Automation Component

This project includes a Python script that represents a support automation component.

The script is responsible for:

- Generating access reports
- Validating request data
- Supporting operational analysis
- Demonstrating integration between automation tools and custom scripts


Location:
