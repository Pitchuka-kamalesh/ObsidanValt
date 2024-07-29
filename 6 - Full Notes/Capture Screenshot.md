---
Created: 2024-07-28T03:51:00
Topic: Selenium
Subtopics: Screenshot
tags:
  - 🦋
  - adult
  - complete
Links:
  - "[[Selenium]]"
Task: 
Modified: 2024-07-28T05:08:00
---


---

# Capture Screenshot
---

##### Why we capture a Screenshot.

 Screenshot are used to capture the activity what has failed or bug in the system.

##### How to Capture a Screenshot.
 we can capture in two ways full page screenshot element screenshot

- fullpage screenshot
```java

	File srcFile = ((TakesScreenshot) driver).getScreenshotAs(OutputType.FILE);
	FileUtils.copyFile(srcFile,"outputFilepath");
	
```
- TakeElementScreenshot
```java
	WebElement ele = driver.findElement(By.tag("a"));
	File src = ele.getScreenshotAs(OutputType.FILE);
	FileUtils.copyFile(src,"outputPath");
```





## References
- Webpage : [Scrennshot](https://www.selenium.dev/documentation/webdriver/interactions/windows/#:~:text=Copy-,TakeScreenshot,-Used%20to%20capture)
- Books   :
- Videos  :
