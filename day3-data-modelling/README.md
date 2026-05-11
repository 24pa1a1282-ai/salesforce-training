# Salesforce Summer Program – Day 3

## Data Modeling, Relationships, Formula Fields and Validation Rules

Today I learned how Salesforce stores and manages business data using objects, fields, records and relationships. I also understood how Formula Fields and Validation Rules help automate business logic without writing code.

---

# Difference Between App, Object, Record and Field

| Concept | Meaning | Example |
|---|---|---|
| App | Collection of related tools and objects | Sales App |
| Object | Stores a specific type of data | Student Object |
| Record | Single entry inside an object | One student’s details |
| Field | Individual piece of information | Student Name |

---

# Standard vs Custom Objects

## Standard Objects
Standard objects are already available in Salesforce and are used for common business processes.

Examples:
- Account
- Contact
- Opportunity
- Lead

## Custom Objects
Custom objects are created based on specific business requirements.

Examples:
- Student
- Faculty
- Course
- Department
- Offer
- Property

Custom objects help companies build systems based on their own workflow instead of depending only on default Salesforce objects.

---

# College Management System Data Model

## Objects Created

- Student
- Faculty
- Course
- Department

---

# Relationships Between Objects

## Department → Faculty
One department can contain multiple faculty members.

Relationship Type:
- Lookup Relationship

Reason:
Faculty members belong to a department, but they can still exist independently.

---

## Department → Course
One department can offer many courses.

Relationship Type:
- Lookup Relationship

Reason:
Courses are connected to departments for academic organization.

---

## Student ↔ Course
Many students can enroll in many courses.

Relationship Type:
- Many-to-Many Relationship

Reason:
A single student can join multiple courses, and a course can contain multiple students.

This can be implemented using a junction object called:
- Enrollment

---

# Simple Relationship Diagram

```text
Department
   |
   |---- Faculty
   |
   |---- Course
              |
              |---- Enrollment ---- Student

Formula Fields
Formula Fields automatically calculate values instead of requiring manual updates.
1. Full Name
Combines First Name and Last Name automatically.
Why use it?
Avoids repetitive typing
Maintains consistency
Reduces human errors
2. Remaining Seats
Calculates available seats in a course.
Formula Logic: Remaining Seats = Total Seats - Enrolled Students
Why use it?
Shows real-time availability
Helps students know seat status instantly
Reduces manual calculations
3. Percentage
Calculates percentage based on obtained marks.
Why use it?
Prevents calculation mistakes
Saves time for faculty
Updates automatically whenever marks change
Validation Rules
Validation Rules prevent users from entering incorrect or incomplete data.
1. Email Cannot Be Empty
Purpose: Prevents saving student records without contact information.
Problem Prevented: Incomplete student records and communication issues.
2. Student Age Cannot Be Negative
Purpose: Blocks impossible age values.
Problem Prevented: Invalid or unrealistic data entries.
3. Course Seats Cannot Exceed Limit
Purpose: Prevents enrolling students beyond course capacity.
Problem Prevented: Overbooking and resource management problems.
Why Structured Data is Important
Large organizations cannot manage operations efficiently using random spreadsheets because data becomes duplicated, inconsistent and difficult to track.
Structured systems like Salesforce organize data into connected objects and relationships. This helps companies:
Maintain accurate records
Prevent invalid data
Automate calculations
Improve reporting
Track business activities properly
Scale operations efficiently
Relationships between objects make enterprise systems more organized and reliable compared to disconnected spreadsheets.
What I Learned Today
Difference between Objects, Fields and Records
Standard vs Custom Objects
Lookup and Many-to-Many Relationships
Schema Builder basics
Formula Fields
Validation Rules
Importance of structured enterprise data
