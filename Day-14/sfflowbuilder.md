## Introduction to Salesforce Flow Builder | Day 1
### What is Flow Builder?

Salesforce Flow Builder is a point-and-click automation tool in Salesforce used to automate business processes without writing code. It can create records, update data, send emails, and guide users through screens. ([Apex Hours][1])

---

## Flow Builder Basics

Flow Builder helps users create automation visually using elements and connections.

Common flow types:

* Screen Flow
* Record-Triggered Flow
* Scheduled Flow
* Autolaunched Flow

Salesforce Flow is considered one of the most powerful automation tools in Salesforce. ([Apex Hours][1])

---

## Flow Structure

A flow usually contains:

1. **Start** → Defines how the flow begins.
2. **Elements** → Actions performed in the flow.
3. **Connectors** → Connect flow steps together.
4. **End** → Finishes the process.

Basic structure:
Start → Logic → Action → End

([Apex Hours][1])

---

## Resources and Logic

### Resources

Resources store and manage data inside flows.

Examples:

* Variables
* Formulas
* Constants
* Collections

### Logic

Logic controls decision-making in flows.

Examples:

* Decision elements
* Loops
* Conditions
* Assignment elements

Flows use logic to automate tasks based on specific conditions. ([Trailhead][2])

| Component  | Purpose          |
| ---------- | ---------------- |
| Variables  | Store data       |
| Decision   | Apply conditions |
| Loop       | Repeat actions   |
| Assignment | Update values    |

---

## Key Points

* Flow Builder is a no-code automation tool.
* Used for automating business processes.
* Includes logic, resources, and flow elements.
* Commonly used by Salesforce admins and developers.

[1]: https://www.apexhours.com/introduction-to-salesforce-flows/?utm_source=chatgpt.com "Introduction to Salesforce Flows - Apex Hours"
[2]: https://trailhead.salesforce.com/content/learn/modules/flow-concepts-quick-look/meet-variables-paths-and-loops?utm_source=chatgpt.com "Introduction to Flow Builder: Variables and Loops"
