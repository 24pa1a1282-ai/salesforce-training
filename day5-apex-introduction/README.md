# Day 5 – Apex Introduction

---

# 1. What is Apex?

Apex is Salesforce’s programming language used to build custom business logic on the Salesforce platform.

It is similar to Java and is used when declarative tools like Flows and Process Builder are not enough to handle complex requirements.

Apex allows developers to:

- Automate business processes
- Validate business rules
- Integrate external systems
- Perform complex calculations
- Handle large-scale operations
- Create custom automation

Apex runs directly on Salesforce servers and is tightly integrated with Salesforce data and security.

---

# 2. Difference Between Flow vs Apex

| Flow (Declarative) | Apex (Programmatic) |
|---|---|
| No-code / low-code | Full coding |
| Faster to build simple automation | Better for complex logic |
| Easy for admins | Used by developers |
| Limited flexibility | Highly flexible |
| Good for approvals and notifications | Good for integrations and advanced processing |
| Hard to manage for large logic | Easier to structure enterprise-scale systems |

---

# Difference Between Configuration vs Coding

| Configuration | Coding |
|---|---|
| Uses clicks and setup | Uses programming |
| Faster for simple tasks | Better for advanced logic |
| Easier maintenance initially | More control and scalability |
| Limited customization | Unlimited customization possibilities |
| Mostly used by admins | Mostly used by developers |

---

# 3. Real Examples Where Apex Is Needed

## Example 1 – Complex Fee Calculation

A university system may calculate fees based on:

- Scholarship percentage
- Attendance
- Hostel allocation
- Lab usage
- Course type

This logic becomes too complex for Flow alone.

Apex is needed because:
- Multiple conditions exist
- Complex calculations are required
- Better maintainability is needed

---

## Example 2 – External Payment Gateway Integration

A college portal may connect with:

- Razorpay
- Stripe
- PayPal

Flows alone cannot handle advanced API integration, authentication, retries, and error handling properly.

Apex is needed for:
- REST API callouts
- Secure integrations
- Exception handling
- Custom response processing

---

## Example 3 – Advanced Student Eligibility Logic

Suppose eligibility depends on:

- Attendance above 75%
- No pending fees
- Minimum GPA
- Department approval
- Internship completion

This logic contains multiple validations and dependencies.

Apex helps by:
- Handling complex conditional logic
- Creating reusable methods
- Improving scalability

---

# 4. Integrated College Management System Design

## CRM Concept

Salesforce CRM stores and manages all student-related information in a centralized system.

The CRM helps manage:

- Admissions
- Student records
- Faculty
- Courses
- Fees
- Attendance
- Notifications

---

## Objects

### Standard/Custom Objects

| Object | Purpose |
|---|---|
| Student__c | Stores student information |
| Course__c | Stores course details |
| Faculty__c | Stores faculty details |
| Enrollment__c | Connects students with courses |
| Attendance__c | Tracks attendance |
| Payment__c | Tracks fee payments |

---

## Relationships

| Relationship | Type |
|---|---|
| Student ↔ Enrollment | Lookup/Master-Detail |
| Course ↔ Enrollment | Lookup/Master-Detail |
| Faculty ↔ Course | Lookup |
| Student ↔ Payment | Master-Detail |

Relationships help connect records and build a complete student ecosystem.

---

## Validation Rules

Validation rules ensure data quality.

Examples:

- Email cannot be blank
- Attendance cannot exceed 100%
- Fee amount cannot be negative
- Student ID must be unique

---

## Flows

Flows automate simple business processes.

Examples:

- Send admission confirmation email
- Notify students about due fees
- Create attendance reminders
- Auto-assign faculty approvals

---

## Apex Usage

Apex handles advanced business logic.

Examples:

- Scholarship calculation
- Eligibility checking
- Bulk student processing
- Payment gateway integration
- Advanced automation
- API integration with external systems

---

# 5. Pseudocode Examples

## Example 1 – Seat Availability

```text
IF available_seats <= 0
THEN block_registration
ELSE allow_registration
```

---

## Example 2 – Attendance Warning

```text
IF attendance < 75%
THEN send_warning_notification
```

---

## Example 3 – Scholarship Eligibility

```text
IF GPA >= 8.5
AND attendance >= 85%
THEN approve_scholarship
ELSE reject_request
```

---

# 6. Reflection – Why Enterprise Systems Eventually Need Programming

Enterprise systems become extremely complex over time.

Declarative tools like Flows are useful for:
- Simple automation
- Quick business processes
- Basic notifications

However, large organizations eventually require:

- Complex calculations
- External integrations
- Scalable architecture
- Advanced security
- Reusable business logic
- Better performance optimization

Using only clicks and configuration creates limitations when business rules become complicated.

Programming with Apex provides:
- Flexibility
- Scalability
- Maintainability
- Better architecture
- Greater control over logic

Apex is important because enterprise software must adapt to constantly changing business requirements.
