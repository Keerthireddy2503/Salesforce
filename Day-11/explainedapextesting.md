## Apex Testing Explained


### What is Apex Testing?

Apex testing is the process of testing Apex code in Salesforce using test classes and test methods. Salesforce requires testing to ensure code works correctly before deployment to production.

Test classes are written using:

* `@isTest`
* Test methods
* Assertions

---

## Test Classes

A test class contains test methods that verify Apex logic.

Example:

```apex
@isTest
private class AccountTest {
    
    @isTest
    static void testAccountCreation() {
        Account acc = new Account(Name='Test Account');
        insert acc;

        System.assertNotEquals(null, acc.Id);
    }
}
```

Important concepts:

* Test classes do not count against organization limits.
* Test methods use sample test data.
* Assertions verify expected results.

---

## Enterprise Reliability

Testing improves enterprise application reliability by:

* Detecting bugs early
* Preventing deployment issues
* Validating business logic
* Improving code quality

Large Salesforce applications depend on automated testing for stable deployments and safe updates. Enterprise systems use testing to ensure features continue working after changes.

---

## Why Salesforce Requires Tests

Salesforce requires at least **75% Apex code coverage** before deployment to production.

Reasons:

* Ensures code quality
* Prevents broken functionality
* Maintains platform stability
* Encourages reliable development practices

Without sufficient test coverage, Salesforce blocks deployment to production.

| Concept       | Purpose              |
| ------------- | -------------------- |
| Test Class    | Tests Apex logic     |
| Assertion     | Verifies results     |
| Code Coverage | Measures tested code |

---

## Key Points

* Apex testing validates Salesforce code functionality.
* Test classes improve enterprise reliability.
* Salesforce requires testing before deployment.
* Minimum 75% code coverage is mandatory.
