Apex Programming Crash Course

Apex is Salesforce’s programming language used for creating custom business logic and automation. It supports object-oriented programming concepts like collections, conditions, classes, and exception handling. (trailhead.salesforce.com)


---

Collections in Apex

Collections are used to store multiple values in a single variable. Apex mainly provides three collection types:

List

Set

Map


(salesforcefaqs.com)

1. List

Stores ordered values and allows duplicates.

List<String> names = new List<String>();
names.add('Keerthi');
names.add('Ravi');

Example

Store multiple student names.


---

2. Set

Stores unique values only.

Set<Integer> marks = new Set<Integer>();
marks.add(90);
marks.add(90);

Duplicate values are automatically removed.

Example

Store unique roll numbers.


---

3. Map

Stores data in key-value pairs.

Map<Integer, String> students = new Map<Integer, String>();
students.put(101, 'Keerthi');

Example

Roll Number → Student Name

Collections help developers manage large amounts of data efficiently. (developer.salesforce.com)


---

Logic Building in Apex

Logic building means writing code step-by-step to solve business problems.

Common Logic Tools

Variables

Loops

Conditions

Methods

Collections


Example

Check student marks and assign result status.

Integer marks = 80;

if(marks >= 35) {
    System.debug('Pass');
}
else {
    System.debug('Fail');
}

Real-World Example

If attendance is below 75%:

Send warning email

Update status

Notify admin


Logic building helps convert business requirements into working code.


---

Exception Handling in Apex

Exception handling is used to manage errors without stopping the entire program. (developer.salesforce.com)

Common Exceptions

DMLException

NullPointerException

QueryException

MathException


(salesforceblue.com)

Try-Catch Example

try {
    Integer result = 10/0;
}
catch(Exception e) {
    System.debug('Error Occurred');
}

Explanation

try → Code that may produce error

catch → Handles the error

Prevents program crash


Real Example

If database insert fails, Apex can show an error message instead of stopping execution.

Exception handling improves system reliability and user experience. 


---

Salesforce CLI Basics

Salesforce CLI (Command Line Interface) is a tool used by developers to interact with Salesforce through commands.

It helps in:

Creating projects

Deploying code

Running Apex

Managing orgs

Retrieving metadata


Common Commands

Login to Salesforce

sf org login web

Create Project

sf project generate

Run Apex Code

sf apex run

Advantages

Faster development

Easy deployment

Better project management

Useful with VS Code


Example

Developers use Salesforce CLI to deploy Apex classes from VS Code to Salesforce orgs.


---

Simple Working Flow

User Action → Apex Logic → Exception Handling → Database Update


---

Conclusion

Collections store multiple values efficiently.

Logic building helps solve business problems using code.

Exception handling manages errors safely.

Salesforce CLI helps developers work faster and manage Salesforce projects easily.
