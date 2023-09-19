# Soap UI
Useful info for using Soap UI.

[Download](https://www.soapui.org/)

## Properties

Properties can be set at Global, Project, Test Suite, Test Case, and Test Step levels.

To reference them, use the following syntax:

```
${#Global#<property-name>}
${#Project#<property-name>}
${#TestSuite#<property-name>}
${#TestCase#<property-name>}
${TestStepName#<property-name>}
```

To get the value of a property inside a Groovy script, use the following syntax:

```Groovy
context.expand('${#Global#<property-name>}')
context.expand('${#Project#<property-name>}')
context.expand('${#TestSuite#<property-name>}')
context.expand('${#TestCase#<property-name>}')
context.expand('${TestStepName#<property-name>}')
```

or 
    
```Groovy
com.eviware.soapui.SoapUI.globalProperties.getPropertyValue('<property-name>')
testRunner.testCase.testSuite.project.getPropertyValue('<property-name>')
testRunner.testCase.testSuite.getPropertyValue('<property-name>')
testRunner.testCase.getPropertyValue('<property-name>')
testRunner.testCase.getTestStepByName('<test-step-name>').getPropertyValue('<property-name>')
```

Can use setPropertyValue(Name, Value) to add/update the value of a property. Use addProperty(Name) to add a new property.

## Groovy Scripts
Add jars to soapui-X.X.X/bin/ext folder and "import" them in the script

To list all methods on an object:

```Groovy
log.info object.metaClass.methods*.name.unique().sort()
```

## Tests

Setup and Teardown scripts run before and after the tests

Use the Property Transfer test step to transfer properties from the response of one API call to the request of another API call.

## References
[Soap-ui - Property and scripting samples](https://www.soapui.org/scripting-properties/property-and-scripting-samples/)
