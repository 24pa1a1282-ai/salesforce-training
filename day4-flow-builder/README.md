# Day 4 - Flow Builder

## What is Flow Builder?

Flow Builder is a no-code automation tool in Salesforce used to automate business processes. It allows users to create workflows visually without writing code.

Businesses use Flow Builder to:
- Reduce manual work
- Improve productivity
- Save time
- Reduce human errors
- Automate repetitive tasks

Flow Builder helps organizations automate processes like sending emails, updating records, assigning tasks, and routing approvals.

---

# Types of Flows

## 1. Screen Flow

Screen Flow is used when user interaction is required.

Features:
- Displays screens to users
- Accepts user input
- Guides users step-by-step
- Used for forms and data entry

Example:
A student registration form where users enter details and submit information.

---

## 2. Record-Triggered Flow

Record-Triggered Flow runs automatically when a record is created, updated, or deleted.

Features:
- Fully automated
- No user interaction needed
- Executes in background
- Used for automatic updates and notifications

Example:
Automatically sending an email when a new student registers.

---

# 5 Automation Ideas for College Management System

## 1. Auto Email After Student Registration

When a student registers:
- Send confirmation email automatically
- Share course details and student ID

Why automation helps:
- Saves staff time
- Instant communication
- Improves student experience

---

## 2. Auto Update Remaining Seats

When a student enrolls:
- Reduce available seat count automatically

Why automation helps:
- Prevents overbooking
- Maintains accurate data
- Eliminates manual calculations

---

## 3. Notify Faculty When Course is Full

When course capacity reaches maximum:
- Automatically notify faculty members

Why automation helps:
- Faster communication
- Better planning
- Reduces monitoring effort

---

## 4. Generate Student ID Automatically

When admission is approved:
- Create unique student ID automatically

Why automation helps:
- Ensures consistency
- Reduces errors
- Faster onboarding process

---

## 5. Send Fee Payment Reminder

Before fee deadline:
- Automatically send reminder emails or SMS

Why automation helps:
- Improves fee collection
- Reduces missed payments
- Saves administrative effort

---

# Flow Design Thinking

## Selected Process:
Auto Email After Student Registration

## Flow Structure

### Trigger
Student registration record is created.

### Steps
1. Capture student details
2. Generate confirmation message
3. Send email automatically
4. Update registration status

### Decision Point
Check whether student email exists.

- If YES → Send email
- If NO → Skip email action

### Final Action
Student receives registration confirmation email.

---

# Manual vs Automated Process

## Process:
Fee Payment Reminder

### Manual Process

- Staff manually checks due dates
- Staff sends reminders individually
- Students may miss notifications
- High workload for administration

### Problems in Manual Process

- Time consuming
- Human errors
- Delayed reminders
- Inconsistent communication

### Automated Process Using Salesforce

- System automatically tracks due dates
- Reminder emails sent automatically
- Notifications sent on time
- Less manual work

### Benefits of Automation

- Faster communication
- Better productivity
- Accurate reminders
- Improved efficiency

---

# Reflection

## Why should companies automate repetitive business processes?

Companies automate repetitive business processes to improve efficiency, reduce manual work, and increase accuracy.

Automation helps businesses:
- Save time
- Reduce operational costs
- Improve consistency
- Eliminate repetitive tasks
- Increase employee productivity
- Deliver faster customer service

Automation is important in enterprise systems because businesses handle large amounts of data and processes daily. Manual handling becomes slow and error-prone. Salesforce automation helps organizations work faster and more efficiently without requiring heavy coding knowledge.

---

# Reflective Questions

## 1. Why do companies automate workflows?

Companies automate workflows to save time, improve productivity, reduce errors, and speed up business operations.

---

## 2. What problems happen with manual processes?

Manual processes are slow, repetitive, error-prone, and difficult to scale.

---

## 3. Difference between Screen Flow and Record Triggered Flow?

Screen Flow requires user interaction, while Record Triggered Flow runs automatically in the background.

---

## 4. Why is no-code automation powerful?

No-code automation allows businesses to automate processes quickly without needing advanced programming skills.

---

## 5. When should automation be avoided?

Automation should be avoided when processes require human judgment, creativity, or complex decision-making.

---

## 6. How does automation improve consistency and productivity?

Automation follows predefined rules every time, reducing errors and completing tasks faster and more consistently.
