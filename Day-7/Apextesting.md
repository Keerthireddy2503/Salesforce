## Salesforce Apex What is Apex Testing?

### Unit Testing Basics

* Unit testing checks if Apex code works correctly
* Tests are written in **test classes**
* Uses `@isTest` annotation
* Assertions verify expected results

Example:

```apex id="pyrx3o"
System.assertEquals(expected, actual);
```

### Why Salesforce Requires Testing

* Minimum **75% code coverage** needed for deployment
* Ensures code quality and reliability
* Prevents bugs in production
* Helps maintain stable business applications

### Benefits

* Safer deployments
* Better application performance
* Easier maintenance
* Detects issues early
