# Automated Legal Document Workflow using Make (Integromat)

## 🧩 Overview
This project automates the process of generating and sending customized legal documents using **Make (Integromat)**. It integrates **Google Sheets**, **Google Docs**, **Google Drive**, and **Gmail** to streamline client communication.

---

## 🚀 Workflow Steps

### 1️⃣ Google Sheets Trigger
- The automation begins when a new row is added to the Google Sheet.
- Required headers:
  - Client Name
  - Case Type
  - Email
  - Document Type Requested
  - Sent

### 2️⃣ Google Docs Template
- A pre-designed Google Docs template is used.
- Dynamic placeholders like `{{Client Name}}`, `{{Case Type}}`, `{{Email}}`, and `{{Document Type Requested}}` are replaced automatically.

### 3️⃣ Google Drive Download
- The generated document is downloaded from Drive to ensure it's properly formatted before attaching to the email.

### 4️⃣ Gmail Send Email
- Sends an email to the client with:
  - Subject: “Your Legal Document - [Case Type]”
  - Attachment: The generated document.
  - Body: A personalized message.

### 5️⃣ Google Sheets Update
- Once the email is sent successfully, the `Sent` column is updated with “✅ Yes”.

---

## 📂 Tech Stack
- **Automation Platform:** Make (Integromat)
- **Google Services:**
  - Google Sheets
  - Google Docs
  - Google Drive
  - Gmail

---

## 🧠 Benefits
- Fully automated and scalable
- Eliminates manual document creation
- Ensures consistent communication
- Logs and updates client email status in real-time

---

## 📺 Demo Video
A complete walkthrough video will be uploaded soon, demonstrating:
- Workflow setup
- Trigger and execution
- Email verification and final output

---
