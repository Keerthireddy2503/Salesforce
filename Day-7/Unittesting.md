## Salesforce Apex What is Apex Testing?

### Unit Testing Basics

Apex testing is the process of checking whether Apex code works correctly.
Developers write **test classes** and **test methods** to test different functionalities.

* Test classes use the `@isTest` annotation
* Tests run automatically before deployment
* Assertions are used to compare expected and actual results

Example:

```apex id="9y1n3g"
@isTest
private class SampleTest {

    static testMethod void testMethod1() {

        Integer result = 5 + 5;

        System.assertEquals(10, result);
    }
}
```

### Why Salesforce Requires Testing

Salesforce requires testing to ensure applications are reliable and error-free.

Main reasons:

* Minimum **75% code coverage** is required for production deployment
* Helps detect bugs before release
* Protects existing functionality from breaking
* Improves application stability and performance

### Benefits of Apex Testing

* Safer deployments
* Better code quality
* Easier maintenance
* Supports enterprise-level reliability
* Ensures smooth business operations

### Important Concepts

* `@isTest` → Marks a class or method as test code
* `System.assert()` → Checks whether results are correct
* Test data should be created inside the test class
* `Test.startTest()` and `Test.stopTest()` help test governor limits and async processes
