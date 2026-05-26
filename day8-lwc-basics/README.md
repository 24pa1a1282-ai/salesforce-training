# Day 8 – Lightning Web Components (LWC) Basics

## What is LWC?

Lightning Web Components (LWC) is Salesforce’s modern UI framework used to build fast, reusable, and component-based user interfaces.

LWC uses:
- HTML for structure
- JavaScript for logic
- CSS for styling
- XML metadata for configuration

LWC follows modern web standards and improves performance compared to older Aura components.

---

# Why Salesforce Uses LWC

Salesforce uses LWC because it:
- Improves application performance
- Creates reusable UI components
- Makes development modular
- Uses modern JavaScript standards
- Simplifies maintenance
- Provides better user experience
- Reduces duplicate code

LWC helps developers build scalable enterprise applications.

---

# UI Screens for College Management System

## 1. Student Registration Screen
Used for adding new student details.

Features:
- Name input
- Roll number
- Department selection
- Contact details

---

## 2. Course Dashboard
Displays available courses and enrolled subjects.

Features:
- Course cards
- Subject list
- Course progress

---

## 3. Attendance View
Shows student attendance information.

Features:
- Attendance percentage
- Monthly records
- Subject-wise attendance

---

## 4. Faculty Panel
Used by teachers to manage students and courses.

Features:
- Student management
- Marks upload
- Attendance update

---

## 5. Notifications Widget
Displays important announcements.

Features:
- Exam alerts
- Fee reminders
- College announcements

---

# Component Breakdown

## Selected Screen: Student Dashboard

The Student Dashboard can be divided into reusable components.

### 1. Header Component
Displays:
- College logo
- Navigation menu
- Student profile icon

Reusable because:
- Same header can be used across all pages.

---

### 2. Student Info Component
Displays:
- Student name
- Roll number
- Department
- Semester

Reusable because:
- Can be used in profile pages and dashboards.

---

### 3. Attendance Component
Displays:
- Attendance percentage
- Subject attendance

Reusable because:
- Can be reused in student and faculty modules.

---

### 4. Notification Component
Displays:
- Alerts
- Announcements
- Updates

Reusable because:
- Same notification system can be used throughout the application.

---

# Why Reusable Components are Useful

Reusable components:
- Reduce duplicate code
- Improve maintainability
- Increase development speed
- Make applications modular
- Improve scalability
- Ensure consistent UI design

Developers can update one component and changes apply everywhere it is used.

---

# Frontend vs Backend Thinking

## Frontend (UI)

Frontend handles:
- Button clicks
- Displaying data
- Forms
- User interaction
- Navigation
- Notification display

Examples:
- Student registration form UI
- Attendance chart display
- Dashboard design

---

## Backend (Apex)

Backend handles:
- Database operations
- Business logic
- Validation
- Fee calculation
- Security
- Data processing

Examples:
- Saving student records
- Calculating attendance percentage
- Processing fee payments

---

# Reflection

Modern enterprise systems use component-based UI architecture because it improves scalability, maintainability, and reusability.

Large applications contain many screens and features. Reusable components help developers manage complexity efficiently.

Component-based architecture:
- Makes applications easier to maintain
- Improves team collaboration
- Reduces development time
- Creates consistent user interfaces
- Supports modular application design

This architecture is important for enterprise systems because large organizations require scalable and maintainable software solutions.

---

# Revision Questions and Answers

## 1. What is a component?

A component is a reusable part of a user interface that contains its own structure, logic, and styling.

---

## 2. Why are reusable components useful?

Reusable components reduce duplicate code, improve maintainability, and speed up development.

---

## 3. Difference between frontend and backend?

Frontend handles user interaction and UI display, while backend handles business logic, database operations, and security.

---

## 4. Why did Salesforce move toward LWC?

Salesforce moved toward LWC for better performance, modern web standards, and improved scalability.

---

## 5. Why is UI important in enterprise systems?

UI improves user experience, productivity, and system usability.

---

## 6. Why should systems separate UI and business logic?

Separation improves maintainability, scalability, debugging, and security.

---

## 7. What security risks exist in enterprise applications?

Common risks include:
- SOQL injection
- Cross-site scripting (XSS)
- CSRF attacks
- Unauthorized access
- Data exposure

---

## 8. Why should developers think modularly?

Modular thinking helps build scalable, reusable, and maintainable applications.

---

# End of Day Outcome

Today I learned:
- What Lightning Web Components (LWC) are
- Modern Salesforce UI architecture
- Component-based development
- Frontend vs backend separation
- Reusable UI design
- Basic enterprise security concepts
