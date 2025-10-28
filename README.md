# Google Docs Automation using Make (Integromat)

This project automates document creation and delivery using **Google Sheets + Google Docs + Gmail + Make**.

---

## ✅ Workflow Summary
When a new row is added in Google Sheets:
1. Make detects the new request
2. Finds the matching Google Docs template
3. Creates a personalized document
4. Saves it in Google Drive
5. Sends it to the client by email
6. Updates the Google Sheet with a **"SENT"** status

---

## ✅ Tools Used
- Make (Integromat)
- Google Sheets
- Google Docs
- Google Drive
- Gmail

---

## ✅ Google Sheet Setup
Create a Google Sheet with these column headers:

Client Name | Case Type | Email | Document Type Requested | Status

yaml
Copy code

Make sure `Status` is empty initially. The automation will update it.

---

## ✅ Google Docs Template Setup
Create a Google Docs template in Google Drive with placeholders like:

Client Name: {{ClientName}}
Case Type: {{CaseType}}
Email: {{Email}}
Document Type: {{DocumentType}}

Dear {{ClientName}},
Your document for {{CaseType}} is now ready.

yaml
Copy code

Save it inside a folder named `Automation/Templates`.

---

## ✅ Make Scenario Modules (Flow)
Build this scenario in Make:

1. **Google Sheets – Watch Rows**
2. **Google Drive – Search Files** (finds template)
3. **Google Docs – Create a Document from Template**
4. **Google Drive – Move a File** (organizes output)
5. **Gmail – Send an Email**
6. **Google Sheets – Update a Row** (sets status to `SENT`)

---

## ✅ Output
- Customized Google Docs are created automatically
- Each document is emailed to the client
- Requests are marked as `SENT` in the sheet
- No manual work required ✅

---

## ✅ Folder Structure (Google Drive)
Automation/
├── Templates/
│ └── Legal_Template.docx
└── Generated/
└── (Created documents will appear here)

yaml
Copy code

---

## ✅ Example Row
| Client Name | Case Type | Email | Document Type Requested | Status |
|-------------|-----------|--------|--------------------------|--------|
| John Doe | Lease Agreement | john@email.com | Lease Template | SENT ✅ |

---

## ✅ How to Run
1. Create Google Sheet and template
2. Build scenario in Make using modules above
3. Turn ON the scenario
4. Add a new row in Google Sheets to test

---

## ✅ Screenshots Included
- Google Sheet
- Google Docs Template
- Make Scenario Workflow
- Output Document
- Sent Email

---

Feel free to use or improve this automation 🔥
If you want, I can also:
✅ Add a Project Description for GitHub
✅ Add Usage Instructions
✅ Add Installation and Setup section
✅ Add License and Author Info
