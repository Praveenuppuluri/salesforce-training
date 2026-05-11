Day 3 - Data Modeling in Salesforce
1. Difference Between App, Object, Record, and Field
App

An app is a collection of tabs, objects, and features designed for a specific business process.

Example: College Management App

Object

An object is similar to a database table that stores related information.

Example: Student Object

Record

A record is a single row or entry inside an object.

Example:

Student Name: Surya Reddy
Roll No: 23PA1A0502
Field

A field stores a particular piece of information in a record.

Examples:

Name
Email
Department
GPA
2. Difference Between Standard Objects and Custom Objects
Standard Objects

Standard objects are pre-built objects provided by Salesforce for common business processes.

Examples:

Account
Contact
Lead
Opportunity

Purpose: Used for CRM and sales-related activities.

Custom Objects

Custom objects are user-created objects based on specific organizational requirements.

Examples:

Student
Faculty
Course
Attendance

Purpose: Used for custom business needs and specialized data management.

3. My College Data Model
Objects
Student
Faculty
Course
Department
Attendance
Relationships
Department → Course

One department can have many courses.

Course → Student

One course can have many students.

Faculty → Course

One faculty can teach many courses.

Student → Attendance

One student can have many attendance records.

Data Model Diagram
Department
   |
   |----< Course >---- Faculty
             |
             |
          Student
             |
             |
        Attendance
