# PROMPTHON MASTER PROMPT — DOCUVERIFY AI

## Project Title

**DocuVerify AI – Smart Document Verification & Validation Platform**

## Objective

Build a complete, modern, responsive, and visually impressive **Document Verification & Validation System** for organizations that receive large numbers of documents such as certificates, identity proofs, invoices, applications, licenses, and official records.

The system should reduce manual verification work by automatically extracting information, validating documents, detecting inconsistencies, identifying duplicates, checking expiry dates, maintaining verification history, and providing a centralized dashboard.

The application must be built using:

* **HTML5**
* **CSS3**
* **Vanilla JavaScript**
* **LocalStorage / IndexedDB for browser-based data persistence**
* No PHP
* No MySQL
* No backend server required
* No frameworks such as React, Angular, or Vue

Use JavaScript to simulate backend/API functionality where a real server is not available. Structure the code so that a real REST API/backend can easily replace the mock API layer later.

---

# 1. DESIGN & UI REQUIREMENTS

Create a **premium, futuristic, colorful, creative dashboard** suitable for a Promptathon/Hackathon demonstration.

The interface should NOT look like a basic CRUD website.

Use:

* Glassmorphism
* Gradient backgrounds
* Animated cards
* Soft shadows
* Rounded corners
* Modern typography
* Colorful statistics
* Animated icons
* Micro-interactions
* Smooth transitions
* Hover effects
* Floating elements
* Toast notifications
* Modal popups
* Progress indicators
* Animated verification status
* Skeleton loaders
* Beautiful empty states
* Responsive layouts
* Dark/Light mode

Use a professional color system containing colors such as:

* Blue
* Purple
* Cyan
* Green
* Orange
* Red

Avoid excessive colors that reduce readability.

Create a polished sidebar navigation with:

1. Dashboard
2. Upload Documents
3. All Documents
4. Verification Queue
5. Duplicate Detection
6. Expiring Documents
7. Verification History
8. Reports
9. API Integration
10. Settings

Add a modern top navigation bar containing:

* Global search
* Notifications
* Dark/Light mode
* User profile
* Current date
* Quick Upload button

---

# 2. LANDING / LOGIN SCREEN

Create an attractive login screen for the platform.

Include:

* DocuVerify AI logo
* Animated document/security illustration
* Email input
* Password input
* Remember Me
* Login button
* Demo Login button
* Forgot Password
* Secure verification badge

Add animated background particles or floating document cards.

For demo purposes, allow:

**Email:** [admin@docuverify.com](mailto:admin@docuverify.com)

**Password:** admin123

The login should work completely on the frontend.

After successful login, redirect to the dashboard.

---

# 3. DASHBOARD

Create a highly visual administrative dashboard.

Display animated statistics cards:

### Total Documents

Example:
**1,248**

### Verified

Example:
**936**

### Pending Verification

Example:
**187**

### Rejected

Example:
**82**

### Duplicate Documents

Example:
**43**

### Expiring Soon

Example:
**27**

Each card should contain:

* Icon
* Number
* Percentage change
* Small description
* Animated counter

Add charts using JavaScript/chart library if available.

Display:

### Verification Analytics

Show:

* Verified documents
* Rejected documents
* Pending documents
* Duplicate documents

Use a colorful doughnut/pie chart.

### Monthly Verification Activity

Display a line/bar chart showing document verification activity over time.

### Recent Documents

Create a table containing:

* Document ID
* Document Name
* Document Type
* Submitted By
* Upload Date
* Verification Status
* Risk Score
* Actions

Statuses:

🟢 Verified

🟡 Pending

🔴 Rejected

🟠 Needs Review

---

# 4. DOCUMENT UPLOAD SYSTEM

Create a beautiful drag-and-drop upload interface.

Users should be able to:

* Drag and drop documents
* Click Browse Files
* Upload multiple documents
* Preview supported files
* Remove selected files
* Upload files
* View upload progress

Supported formats:

* PDF
* JPG
* JPEG
* PNG
* DOC
* DOCX

Display:

* File name
* File size
* File type
* Upload progress
* Upload status

Add animated upload progress.

After uploading, automatically start the verification workflow.

Show a popup:

**"Document uploaded successfully!"**

---

# 5. DOCUMENT INFORMATION EXTRACTION

After upload, create a document analysis screen.

Display an animated verification process:

### Step 1

Uploading Document

### Step 2

Reading Document

### Step 3

Extracting Information

### Step 4

Validating Information

### Step 5

Checking Duplicate Records

### Step 6

Checking Expiry

### Step 7

Generating Verification Result

Use an animated progress bar.

Extract/display example fields:

* Full Name
* Document Number
* Date of Birth
* Issue Date
* Expiry Date
* Organization
* Address
* Certificate Number
* Invoice Number
* Amount
* Category

Since this is a frontend-only application, create a realistic **mock OCR/extraction engine** that reads demo/sample data based on document type.

Clearly structure this logic so it can later be replaced by a real OCR API.

---

# 6. DOCUMENT VALIDATION ENGINE

Create a JavaScript validation engine.

Validate:

### Required Fields

Check whether mandatory information exists.

### Format Validation

Check:

* Document number format
* Date format
* Email format
* Phone number
* Invoice number
* Certificate number

### Date Validation

Check:

* Expired documents
* Future issue dates
* Invalid date ranges

### Consistency Validation

Compare related fields.

Example:

If issue date is later than expiry date:

**ERROR: Invalid document date range**

### Missing Information

Show:

**Missing Information**

with highlighted fields.

### Invalid Information

Show:

**Invalid Information**

with explanation.

### Suspicious Information

Show:

**Needs Manual Review**

---

# 7. DOCUMENT AUTHENTICITY CHECK

Create an authenticity verification module.

Display:

**Authenticity Score**

Example:

**94% Authentic**

Use a circular animated progress indicator.

Check:

* Document structure
* Required fields
* Metadata
* Verification number
* Issuing organization
* Date validity
* Internal consistency
* Reference database match

Show a verification checklist:

✓ Document structure valid

✓ Required fields available

✓ Date valid

✓ Issuer recognized

✓ Reference number found

✓ No duplicate detected

✓ No major inconsistency

For the frontend demo, use mock organizational records.

---

# 8. FRAUD / ALTERATION DETECTION

Create a visual "Document Integrity Analysis" section.

Detect suspicious characteristics through simulated frontend rules.

Check:

* Missing fields
* Unexpected formatting
* Inconsistent values
* Invalid dates
* Duplicate identifiers
* Suspicious metadata
* Altered-looking values
* Mismatched information

Display a:

### Risk Score

Example:

**12 / 100 – Low Risk**

Use:

🟢 Low Risk

🟡 Medium Risk

🔴 High Risk

If suspicious information is found, display an animated warning card.

Example:

⚠️ **Potential alteration detected**

"Document number format differs from the expected format."

---

# 9. DUPLICATE DOCUMENT DETECTION

Create a dedicated Duplicate Detection page.

Detect duplicates based on:

* Document number
* Certificate number
* Invoice number
* File hash simulation
* Name + date combination
* Similar document metadata

Display:

### Duplicate Match Found

Example:

**92% Similarity**

Show side-by-side comparison:

**Current Document**

vs

**Existing Document**

Highlight matching fields.

Allow:

* View Original
* Compare
* Mark as Duplicate
* Ignore
* Send for Review

---

# 10. EXPIRY DETECTION

Create an Expiring Documents section.

Automatically categorize:

### Expired

Documents whose expiry date has passed.

### Expiring Within 7 Days

### Expiring Within 30 Days

### Valid

Display colorful cards.

Add notifications:

🔴 Document expired

🟠 Document expires soon

🟢 Document valid

Allow users to filter documents by expiry status.

---

# 11. VERIFICATION RESULT PAGE

After verification, show a beautiful result popup.

Example:

## DOCUMENT VERIFIED

🟢

**Verification Successful**

Document:
**Degree Certificate.pdf**

Status:
**Verified**

Authenticity:
**96%**

Risk Score:
**Low**

Verification Date:
**08 August 2026**

Verification ID:
**VER-2026-000128**

Include buttons:

* View Details
* Download Report
* Print Report
* Verify Another Document

For rejected documents display:

🔴

**Verification Failed**

with detailed reasons.

---

# 12. DOCUMENT DETAILS PAGE

When a user clicks a document, display:

### Document Preview

Show document preview area.

### Extracted Information

Display all extracted fields.

### Validation Results

Display:

✓ Passed checks

⚠ Warnings

✕ Failed checks

### Authenticity

Show authenticity score.

### Risk Analysis

Show risk score.

### Verification History

Show every verification event with:

* Date
* Time
* User
* Action
* Status

---

# 13. VERIFICATION HISTORY

Create a complete verification history page.

Table columns:

* Verification ID
* Document ID
* Document Name
* User
* Date
* Time
* Verification Type
* Result
* Risk Score
* Action

Add filters:

* Date
* Status
* Document Type
* User
* Risk Level

Add search functionality.

Allow:

* View
* Export
* Print

Persist history using LocalStorage/IndexedDB.

---

# 14. SEARCH & FILTER SYSTEM

Create global search.

Users can search by:

* Document name
* Document ID
* Document number
* Certificate number
* Invoice number
* Person name
* Organization
* Verification ID

Add advanced filters:

* Status
* Document type
* Date
* Risk score
* Expiry status

Search results should update dynamically without refreshing the page.

---

# 15. NOTIFICATION CENTER

Create a notification dropdown.

Notifications should include:

🔴 Expired document

🟠 Document requires review

🟡 Duplicate detected

🟢 Verification completed

🔵 New document uploaded

Allow:

* Mark as read
* Mark all as read
* Delete notification

Display notification count on the top navigation bar.

---

# 16. REPORT GENERATION

Create a Reports page.

Generate:

### Verification Summary

Show:

* Total documents
* Verified
* Rejected
* Pending
* Duplicates
* Expired

### Risk Report

Show:

* Low risk
* Medium risk
* High risk

### Verification Activity

Show daily/monthly statistics.

Add buttons:

* Print Report
* Download Report
* Export CSV

Use JavaScript to generate downloadable CSV reports.

If possible, generate printable PDF-style reports using browser print functionality or a client-side PDF library.

---

# 17. API INTEGRATION CENTER

Create an API Integration page.

Explain that organizations can connect external systems.

Display sample API endpoints:

POST /api/documents/upload

POST /api/documents/verify

GET /api/documents/{id}

GET /api/verification/history

GET /api/verification/status/{id}

POST /api/duplicates/check

Create a visual API configuration form:

* API Base URL
* API Key
* Organization ID
* Environment
* Webhook URL

Buttons:

**Test Connection**

**Save Configuration**

Since the application is frontend-only, create a JavaScript mock API service.

Use functions such as:

* uploadDocument()
* verifyDocument()
* getDocument()
* checkDuplicate()
* getVerificationHistory()

Keep the API layer separated from UI code so it can easily be connected to a real backend later.

---

# 18. ADMIN SETTINGS

Create Settings page.

Sections:

### Organization

* Organization Name
* Organization ID
* Email
* Phone

### Verification Settings

* Automatic verification
* Duplicate detection
* Expiry alerts
* Risk threshold

### Notification Settings

* Email notifications
* Dashboard notifications
* Expiry alerts
* Duplicate alerts

### Appearance

* Light Mode
* Dark Mode
* Compact Mode

Save all settings using LocalStorage.

---

# 19. DATA STORAGE

Because the project must work using HTML, CSS and JavaScript only, implement browser-based persistence.

Use:

**LocalStorage**

for:

* Login session
* Documents
* Verification history
* Notifications
* Settings
* Dashboard statistics

Use sample seed data when the application is opened for the first time.

The application must retain data after refreshing the browser.

---

# 20. DEMO DATA

Preload realistic sample documents.

Examples:

1. Aadhaar-style identity document
2. PAN-style identity document
3. College Degree Certificate
4. Employee ID
5. GST Invoice
6. Experience Certificate
7. Driving License
8. Income Certificate

Do not use real personal information.

Use fictional demo information.

Create different statuses:

* Verified
* Pending
* Rejected
* Duplicate
* Expired
* Needs Review

---

# 21. ANIMATIONS & POPUPS

Add attractive animations throughout the application.

Examples:

* Upload popup
* Verification progress popup
* Success popup
* Error popup
* Duplicate warning popup
* Document details modal
* Delete confirmation modal
* Logout confirmation modal

Use:

* Fade-in
* Slide-in
* Scale
* Progress animation
* Counter animation
* Pulse effects

Animations should remain smooth and not make the application difficult to use.

---

# 22. TOAST NOTIFICATIONS

Create a reusable toast system.

Examples:

**✓ Document uploaded successfully**

**✓ Verification completed**

**⚠ Duplicate document detected**

**⚠ Document expires in 5 days**

**✕ Verification failed**

**✓ Report generated**

---

# 23. SECURITY-STYLE UI

Create visual security indicators.

Display:

🔐 Secure Verification

🛡 Data Protected

✓ Validation Completed

✓ Integrity Checked

✓ Duplicate Scan Completed

This is a frontend demo, so do not falsely claim real encryption or real-world security that has not been implemented.

---

# 24. RESPONSIVE DESIGN

The application must work perfectly on:

* Desktop
* Laptop
* Tablet
* Mobile

On mobile:

* Sidebar becomes a hamburger menu
* Tables become responsive cards
* Modals fit the screen
* Dashboard cards stack vertically
* Charts resize automatically

Do not allow horizontal scrolling.

---

# 25. ACCESSIBILITY

Implement:

* Semantic HTML
* Proper labels
* Keyboard navigation
* Visible focus states
* Alt text
* Good color contrast
* ARIA labels where required

---

# 26. ERROR HANDLING

The application must never break because of invalid user input.

Handle:

* Empty uploads
* Unsupported file formats
* Duplicate uploads
* Missing fields
* Invalid dates
* Invalid form values
* LocalStorage errors
* Invalid document data

Display user-friendly error messages.

Never expose raw JavaScript errors to the user.

---

# 27. PROJECT STRUCTURE

Generate the project with this structure:

docuverify-ai/
│
├── index.html
├── dashboard.html
├── documents.html
├── verification.html
├── history.html
├── reports.html
├── api.html
├── settings.html
│
├── css/
│   ├── style.css
│   ├── dashboard.css
│   ├── responsive.css
│   └── animations.css
│
├── js/
│   ├── app.js
│   ├── auth.js
│   ├── dashboard.js
│   ├── documents.js
│   ├── verification.js
│   ├── validation.js
│   ├── duplicate.js
│   ├── history.js
│   ├── reports.js
│   ├── api.js
│   ├── storage.js
│   ├── notifications.js
│   └── settings.js
│
└── assets/
└── icons/

Make sure all file paths and imports are correct.

---

# 28. CODE QUALITY

Write clean, modular and maintainable code.

Requirements:

* No undefined JavaScript functions
* No broken buttons
* No broken links
* No missing IDs
* No console errors
* No duplicate event listeners
* No unused critical functions
* Validate all forms
* Add comments for important logic
* Use reusable functions
* Use consistent naming conventions

Every navigation item and button should perform a meaningful action.

---

# 29. DEMO MODE

Create a **Demo Mode** button.

When activated, it should automatically demonstrate:

1. Upload a sample document
2. Extract information
3. Validate information
4. Check duplicate records
5. Check expiry
6. Calculate risk score
7. Generate verification result
8. Add the result to verification history
9. Update dashboard statistics

This should make the project impressive during the Promptathon presentation.

---

# 30. FINAL USER FLOW

The complete workflow should be:

LOGIN
↓
DASHBOARD
↓
UPLOAD DOCUMENT
↓
DOCUMENT PREVIEW
↓
INFORMATION EXTRACTION
↓
VALIDATION
↓
AUTHENTICITY CHECK
↓
DUPLICATE CHECK
↓
EXPIRY CHECK
↓
RISK ANALYSIS
↓
VERIFICATION RESULT
↓
SAVE VERIFICATION HISTORY
↓
UPDATE DASHBOARD
↓
GENERATE REPORT

---

# 31. VISUAL HIGHLIGHT

Make the homepage/dashboard immediately communicate:

**"Upload → Analyze → Validate → Verify → Report"**

Create a visual horizontal process indicator showing these five stages.

The main dashboard should feel like an AI-powered enterprise verification platform.

Use a hero message:

**"Verify Documents. Detect Risks. Trust the Data."**

Subtitle:

**"AI-inspired document verification and validation for faster, safer, and smarter organizational workflows."**

---

# 32. IMPORTANT IMPLEMENTATION RULES

The final application must:

✓ Run directly in a browser

✓ Work without PHP

✓ Work without MySQL

✓ Use HTML, CSS and JavaScript

✓ Store demo data locally

✓ Have functional navigation

✓ Have functional forms

✓ Have functional search

✓ Have functional filters

✓ Have functional upload UI

✓ Have functional validation

✓ Have functional duplicate detection simulation

✓ Have functional expiry detection

✓ Have functional verification history

✓ Have functional dashboard statistics

✓ Have functional reports

✓ Have working dark/light mode

✓ Have responsive design

✓ Have animated UI

✓ Have popups/modals

✓ Have toast notifications

✓ Have realistic demo data

✓ Have a working Demo Mode

✓ Have zero console errors

✓ Never use fake buttons that do nothing

---

# 33. FINAL DELIVERABLE

Generate the complete working project.

Provide all required:

* HTML
* CSS
* JavaScript
* Sample data
* Icons
* Components
* Validation logic
* LocalStorage logic
* Mock API layer
* Responsive styling
* Animations
* Dashboard
* Verification workflow
* Reports
* Settings

The final result should look like a **professional SaaS product**, not a basic college project.

Prioritize:

**Functionality + Visual Design + User Experience + Error-Free Execution + Demonstration Value.**

Before completing the project, internally verify every navigation link, button, modal, form, event listener, LocalStorage operation, calculation, filter, search function, and JavaScript import to ensure there are no broken features or console errors.
