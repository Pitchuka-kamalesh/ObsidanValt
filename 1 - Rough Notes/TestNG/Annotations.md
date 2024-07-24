
2024-07-14 05:30

Status: #baby 

Tags: [[TestNG]]


---

# Annotations
---
TestNG has multiple Annotations here are the list of testNG Annotations

| Annotation   | Description                                                                                                                                                                              | Notation        |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------- |
| BeforeSuite  | The annotated method will be run before all tests in this suite have run.                                                                                                                | `@BeforeSuite`  |
| BeforeTest   | The annotated method will be run before any test method belonging to the classes inside the <test> tag is run.                                                                           | `@BeforeTest`   |
| BeforeGroups | The list of groups that this configuration method will run before. This method is guaranteed to run shortly before the first test method that belongs to any of these groups is invoked. | `@BeforeGroups` |
| BeforeClass  | The annotated method will be run before the first test method in the current class is invoked.                                                                                           | `@BeforeClass`  |
| BeforeMethod | The annotated method will be run before each test method.                                                                                                                                | `@BeforeMethod` |
| Test         |                                                                                                                                                                                          | `@Test`         |
| AfterMethod  | The annotated method will be run after each test method.<br>                                                                                                                             | `@AfterMethod`  |
| AfterClass   | The annotated method will be run after all the test methods in the current class have been run.                                                                                          | `@AfterClass`   |
| AfterGroups  | The list of groups that this configuration method will run after. This method is guaranteed to run shortly after the last test method that belongs to any of these groups is invoked.    | `@AfterGroups`  |
| AfterTest    | The annotated method will be run after all the test methods belonging to the classes inside the <test> tag have run.                                                                     | `@AfterTest`    |
| AfterSuite   | The annotated method will be run after all tests in this suite have run.                                                                                                                 | `@AfterSuite`   |




---
TestNG.XML file


```xml
<!DOCTYPE suite SYSTEM "https://testng.org/testng-1.0.dtd">

<suite name="Suite1" verbose="1">
  <test name="Nopackage">
    <classes>
       <class name="NoPackageTest"/>
    </classes>
  </test>

  <test name="Regression1">
    <classes>
      <class name="test.sample.ParameterSample"/>
      <class name="test.sample.ParameterTest"/>
    </classes>
  </test>
</suite>
```




output:



---

### Explanation








## References
https://testng.org/