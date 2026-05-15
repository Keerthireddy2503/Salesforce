What is Record-Triggered Flow?

A Record-Triggered Flow is a type of Flow in Salesforce that runs automatically when a record is created, updated, or deleted.

It is mainly used for automation without writing code.

It can run:

When a new record is created

When an existing record is updated

When a record is deleted


Example

When a student’s attendance becomes less than 75%, Salesforce automatically sends a warning email using a Record-Triggered Flow.


---

When Flows Execute

Flows execute automatically when specific conditions or actions occur in Salesforce.

Main Execution Times

1. Before Save Flow

Runs before the record is saved in the database.

Used for:

Updating field values quickly

Validations

Simple changes


Example

Automatically setting student status as “Active” before saving the record.


---

2. After Save Flow

Runs after the record is saved.

Used for:

Sending emails

Creating related records

Notifications

Complex automation


Example

After creating a student record, Salesforce sends a welcome email automatically.


---

Real-World Examples

College Management System

Send attendance warning emails automatically.

Create fee reminder notifications.

Update student status automatically.


Hospital System

Notify doctors when a patient record is created.

Send appointment reminders to patients.


E-Commerce System

Send order confirmation emails.

Update delivery status automatically.


Employee Management

Create onboarding tasks when a new employee joins.

Send leave approval notifications.



---

Simple Flow Working

Record Created/Updated → Flow Executes → Action Performed



