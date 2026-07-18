# 🏨 Hotel Guest Feedback Processing Agent using Zapier

## 📌 Project Overview

The **Hotel Guest Feedback Processing Agent** is an intelligent workflow automation solution built using **Zapier**, **Google Forms**, **Google Sheets**, and **Gmail**.

The project automates the complete hotel guest feedback process by collecting guest responses, analyzing ratings and comments, classifying the overall sentiment, updating a centralized Google Spreadsheet, and sending personalized acknowledgement emails automatically.

The solution eliminates manual effort, ensures timely communication with guests, and helps hotel management improve customer satisfaction through automated feedback processing.

---

# 🎯 Business Problem

Hotels receive numerous guest feedback submissions every day. Manually reviewing feedback, updating records, identifying dissatisfied guests, and responding to each guest is time-consuming and prone to delays.

This project automates the entire workflow by:

- Collecting guest feedback automatically
- Classifying guest sentiment
- Updating hotel records
- Sending personalized acknowledgement emails
- Notifying hotel management through email BCC
- Maintaining an audit trail of every submission

---

# 🎯 Project Objectives

- Automate hotel guest feedback processing
- Eliminate manual data entry
- Improve customer response time
- Classify customer satisfaction automatically
- Maintain a centralized feedback repository
- Enhance guest engagement through personalized communication
- Ensure every submission is processed without modifying historical records

---

# ✨ Key Features

- 📝 Google Form integration
- 📊 Automatic response storage in Google Sheets
- 🤖 Intelligent sentiment classification
- 📧 Personalized acknowledgement emails
- 📬 Automatic BCC to hotel administrator
- 📈 Centralized guest feedback tracking
- ⚡ Fully automated workflow
- ☁️ Cloud-based automation using Zapier
- 🔒 Existing records remain unchanged

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|---------|
| Zapier | Workflow Automation |
| Google Forms | Guest Feedback Collection |
| Google Sheets | Feedback Repository |
| Gmail | Automated Email Notifications |
| Conditional Logic | Sentiment Classification |

---

# 🏗 Workflow Architecture

```
Guest
   │
   ▼
Google Form
   │
   ▼
Google Spreadsheet
(Store Guest Feedback)
   │
   ▼
Zapier Trigger
(New Form Response)
   │
   ▼
Read Ratings & Comments
   │
   ▼
Analyze Guest Sentiment
   │
   ▼
Decision Logic
────────────────────────────────────
│             │                   │
│             │                   │
Positive     Neutral          Negative
│             │                   │
│             │                   │
▼             ▼                   ▼
Update       Update            Update
Action        Action            Action
│             │                   │
▼             ▼                   ▼
Send Email   Send Email       Send Email
│             │                   │
└─────────────┴───────────────────┘
                │
                ▼
Guest Receives Personalized Email
                │
                ▼
BCC to Hotel Administrator
```

---

# 🔄 Workflow Process

## Step 1 – Guest Submission

A guest submits hotel feedback through a Google Form.

The form captures:

- Timestamp
- Guest Name
- Email Address
- Cleanliness Rating
- Comfortability Rating
- Maintenance Rating
- Amenities Rating
- Housekeeping Rating
- Overall Experience
- Recommendation
- Comments

---

## Step 2 – Store Response

Every submission is automatically appended as a **new row** in Google Sheets.

The workflow:

- Never overwrites existing records
- Never deletes previous responses
- Maintains a complete feedback history

---

## Step 3 – Analyze Guest Feedback

The workflow evaluates both:

- Guest ratings
- Guest comments

to determine the overall customer sentiment.

### Positive Feedback

Conditions:

- Excellent
- Good
- Satisfied
- Very Satisfied

Example Comments

- Great Service
- Wonderful Experience
- Friendly Staff
- Excellent Stay
- Very Clean Room

Action Column

```
Positive Comments
```

---

### Neutral Feedback

Conditions

- Average Ratings
- Neutral Ratings
- Suggestions for Improvement

Example

- Food could be improved
- Average Stay
- Room was okay

Action Column

```
Neutral Feedback
```

---

### Negative Feedback

Conditions

Any Poor Ratings OR comments mentioning:

- Dirty Room
- Maintenance Issues
- Noise
- Complaint
- Poor Housekeeping
- Delay in Service
- Bad Experience
- Broken Facilities

Action Column

```
Negative Feedback
```

---

# 📧 Automated Email Notification

After sentiment classification, Zapier automatically sends a personalized acknowledgement email.

### Email Details

**Sender**

```
prashanth.qa@gmail.com
```

**Recipient**

Guest Email Address

**BCC**

```
prashanth.qa@gmail.com
```

**Subject**

```
Thank You for Sharing Your Hotel Experience
```

---

## Positive Email

Guest receives:

- Appreciation
- Thank You Message
- Invitation to Visit Again

---

## Neutral Email

Guest receives:

- Thank You
- Appreciation for Suggestions
- Assurance of Continuous Improvement

---

## Negative Email

Guest receives:

- Apology
- Acknowledgement of Concerns
- Commitment to Corrective Actions
- Assurance of Better Service

---

# ⚠ Error Handling

If the guest email address is missing or invalid:

- Store the response
- Update the Action column
- Skip email notification
- Continue workflow successfully

No workflow interruption occurs.

---

# 📊 Google Spreadsheet Structure

| Timestamp | Name | Email | Cleanliness | Comfortability | Maintenance | Amenities | Housekeeping | Overall Experience | Recommendation | Comments | Action |

Every new guest response is appended below the last existing row.

---

# 🚀 Workflow Execution

For every new Google Form submission:

1. Detect new response
2. Read guest details
3. Append data to Google Spreadsheet
4. Analyze ratings
5. Analyze comments
6. Determine guest sentiment
7. Update Action column
8. Generate personalized email
9. Send email to guest
10. Send BCC to administrator
11. Complete workflow successfully

---

# 📂 Repository Structure

```
Hotel-Guest-Feedback-Processing-Agent/
│
├── README.md
├── Zapier_Workflow.pdf
├── Project_Documentation.pdf
├── Workflow_Screenshot.png
├── Google_Form.png
├── Google_Sheet.png
├── Email_Templates/
│      ├── Positive_Email.png
│      ├── Neutral_Email.png
│      └── Negative_Email.png
└── Assets/
       └── Workflow_Diagram.png
```

---

# 📈 Benefits

- Reduces manual effort
- Improves guest satisfaction
- Provides faster responses
- Centralizes customer feedback
- Standardizes communication
- Improves service quality
- Enables continuous improvement
- Supports better customer relationship management

---

# 🔮 Future Enhancements

- AI-powered sentiment analysis using OpenAI
- Dashboard for guest satisfaction metrics
- Complaint ticket creation
- SMS notifications
- WhatsApp integration
- Power BI reporting dashboard
- Multi-language email templates
- Hotel CRM integration
- Analytics for guest trends

---

# 🎓 Learning Outcomes

This project demonstrates hands-on experience with:

- Zapier Workflow Automation
- Google Workspace Integration
- Business Process Automation
- Customer Experience Management
- Conditional Workflow Logic
- Automated Email Notifications
- Data Management using Google Sheets
- End-to-End No-Code Automation

---

# 👨‍💻 Author

**Prasanth Rasam**

- Certified Data Scientist
- AI & Automation Enthusiast
- Zapier Developer
- Langflow Developer
- Python Developer
- IT Service Management Professional

---

# ⭐ Project Highlights

- End-to-End Guest Feedback Automation
- Intelligent Sentiment Classification
- Personalized Email Communication
- Google Forms Integration
- Google Sheets Automation
- Gmail Automation
- Business Process Automation
- Cloud-Based Workflow
- Zero Manual Intervention
- Scalable No-Code Solution

---

## 📄 License

This project is created for educational, portfolio, and demonstration purposes.

---

## 🙏 Acknowledgements

- Zapier
- Google Forms
- Google Sheets
- Gmail
- OpenAI Community
