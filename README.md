🚀 IT Access Management System (Power Automate)
🧭 Overview

This project is an automated IT Access Request and Approval System built using Microsoft Power Platform.

It simulates a real-world Identity and Access Management (IAM) workflow, where employees request access to corporate systems and managers approve or reject requests through an automated process.

🏗️ Architecture

Microsoft Lists → Power Automate → Approvals → Outlook Email → List Update

⚙️ Technologies Used
Microsoft Lists (SharePoint-based data storage)
Power Automate (workflow automation)
Microsoft Outlook (email notifications)
Microsoft Approvals (approval workflow)
Microsoft 365 ecosystem
📊 Data Structure (Microsoft Lists)

The system uses the following fields:

Employee Name
Email
Requested System
Justification
Manager
Status
ApprovedBy
ResponseDate
🔄 Workflow Overview
1. Request Creation

An employee submits a new access request in Microsoft Lists.

2. Flow Trigger

Power Automate automatically detects the new item and starts the workflow.

3. Approval Process

The assigned manager receives an approval request and can:

✅ Approve the request
❌ Reject the request
4. System Update

After the decision, the system automatically updates:

Request Status
Approver Name
Response Date
5. Email Notification

The requester receives an automated email with the result.

📧 Notifications
✅ Approved Request
Status updated to Approved
Email confirmation sent to requester
❌ Rejected Request
Status updated to Rejected
Email sent with rejection details
🧪 Testing Process

The system was validated using the following steps:

Create a new item in Microsoft Lists
Fill all required fields
Trigger Power Automate flow automatically
Approve or reject the request
Verify list update (Status, Approver, Date)
Confirm email notification delivery
Check run history in Power Automate
💡 Key Features
End-to-end automated approval workflow
Corporate IT access simulation (IAM concept)
Email notification system
Audit trail (approver + timestamp)
Integration with Microsoft 365 services
🎯 Business Value

This solution demonstrates how organizations can:

Automate access request workflows
Reduce manual IT approvals
Improve security and traceability
Standardize access management processes
🚀 Future Improvements
Integration with Microsoft Entra ID (Azure AD)
Multi-level approval workflow
Power BI dashboard for analytics
Microsoft Teams notifications
SLA tracking for requests
Advanced audit logging
👨‍💻 Author

Developed by Luiz Henrique
Focus: Cloud Computing | Automation | IT Infrastructure | Microsoft Azure Ecosystem

📌 Project Status

✔ Fully Functional
✔ End-to-End Automated Workflow
✔ Portfolio Ready (Junior Cloud / Power Platform Role)
