Salesforce Apex Tutorial for Beginners

Apex is Salesforce’s programming language used to create custom logic and automation. It is similar to Java and runs on Salesforce servers. 


---

Variables in Apex

Variables are used to store data values.

Syntax

datatype variableName = value;

Example

Integer marks = 90;
String name = 'Keerthi';
Boolean result = true;

Common Data Types

Integer → Stores numbers

String → Stores text

Boolean → Stores true/false

Decimal → Stores decimal values


Variables help store and process information in Apex programs.


---

Loops in Apex

Loops are used to repeat code multiple times. Apex supports different loop types like for, while, and do-while. 

For Loop Example

for(Integer i = 1; i <= 5; i++) {
    System.debug(i);
}

Output

1 2 3 4 5

Use

Used when we know how many times the code should run.

Real Example

Loop through all student records and send notifications.


---

Conditions in Apex

Conditions help make decisions in programs.

If-Else Example

Integer marks = 75;

if(marks >= 35) {
    System.debug('Pass');
}
else {
    System.debug('Fail');
}

Use

Checks whether a condition is true or false.

Real Example

If attendance is below 75%, send a warning message.

Logical statements like if, else if, and switch are commonly used in Apex. 


---

Classes in Apex

A class is a blueprint containing variables and methods.

Example

public class StudentInfo {

    public static void display() {
        System.debug('Welcome Student');
    }
}

Explanation

class → Defines the class

method → Performs an action

System.debug() → Prints output


Classes help organize code properly. Salesforce stores Apex mainly in classes and triggers. 


---

Triggers Overview

Triggers are Apex code that runs automatically when records are created, updated, deleted, or undeleted. 

Trigger Syntax

trigger StudentTrigger on Student__c (before insert) {

    for(Student__c s : Trigger.new) {
        s.Status__c = 'Active';
    }
}

What This Does

Before saving a student record:

Trigger runs automatically

Status becomes “Active”



---

Types of Triggers

Before Trigger

Runs before data is saved.

After Trigger

Runs after data is saved.

Common Events

before insert

before update

after insert

after delete





---

Simple Apex Working Flow

User Action → Apex Code/Trigger → Processing → Database Update


---

Conclusion

Variables store data.

Loops repeat tasks.

Conditions make decisions.

Classes organize code.

Triggers automate actions when records change.


These are the basic building blocks of Apex programming in Salesforce.
