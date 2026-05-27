## Building Advanced Flows with Choices, Loops, and Apex


### Advanced Flow Logic

Advanced Salesforce Flows help automate complex business processes using logic, decisions, loops, and Apex integration. These flows reduce manual work and improve automation efficiency. ([Developer][1])

Common advanced flow features:

* Decisions
* Loops
* Assignments
* Collections
* Apex Actions

---

## Choices and Loops

### Choices

Choices allow users to select options in Screen Flows using:

* Picklists
* Radio buttons
* Checkboxes

Flow Builder supports:

* Manual Choices
* Record Choice Sets
* Picklist Choice Sets

Choices help collect user input and control automation paths. ([Developer][1])

### Loops

Loops process multiple records one by one inside a flow.

Example:

* Update multiple contacts
* Process account records
* Handle collection variables

Best practice:

* Avoid DML operations inside loops.
* Store updated records in a collection and update later. ([Developer][1])

---

## Multi-Step Automation

Advanced flows can perform multiple actions in sequence.

Basic structure:
Start → Decision → Loop → Action → End

Examples:

* Create records
* Update related records
* Send emails
* Run approvals
* Process collections

Flows are widely used for enterprise automation because they combine visual design with business logic. ([Udemy][2])

---

## Invocable Apex

Invocable Apex allows Flow Builder to call Apex classes for complex operations.

Important annotations:

* `@InvocableMethod`
* `@InvocableVariable`

Used when:

* Logic becomes too complex for Flow
* Bulk processing is needed
* External integrations are required

Invocable Apex helps combine low-code Flow automation with custom Apex functionality. ([Salesforce][3])

| Component   | Purpose             |
| ----------- | ------------------- |
| Choice      | User selection      |
| Loop        | Process collections |
| Apex Action | Run custom logic    |

---

## Key Points

* Advanced Flows support complex automation.
* Loops process multiple records efficiently.
* Choices help collect user input.
* Invocable Apex extends Flow capabilities with custom code.

[1]: https://developer.salesforce.com/blogs/2019/08/building-advanced-flows-with-choices-loops-and-new-apex-defined-types?utm_source=chatgpt.com "Building Advanced Flows with Choices, Loops, and New Apex-Defined Types | Salesforce Developers Blog"
[2]: https://www.udemy.com/course/salesforce-lightning-flow-builder-building-advanced-flows/?utm_source=chatgpt.com "Salesforce Flows : Building Advanced Lightning Flows"
[3]: https://help.salesforce.com/s/articleView?id=platform.flow_build_extend_apex.htm&language=en_US&type=5&utm_source=chatgpt.com "Let Flows Execute Apex Actions"
