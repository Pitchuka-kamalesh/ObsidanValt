---
date: 2024-07-15
Topic: Selenium
Subtopics: Alerts
tags:
  - adult
Links:
  - "[[Selenium]]"
Task:
---

---

# Alerts
---

 How to handle the Alerts using selenium 

   - We have to check whether the alert is present or not before switching the to alert
   - if alert is present then switch to alert  to perform the action.
   - there are 4 action to perform the action in the alerts.
   - ***sendKeys()***
   - ***accept()***
   - ***dismiss()***
   - ***getText()***
```java
 driver.switchTo().alert();
 Alert alert = driver.switchTo().alert();
 String alertText = alert.getText();
 alert.dismiss();
 alert.accept();
 alert.sendKeys();
```




## References
- Webpage : [Selenium | Alerts](https://www.selenium.dev/documentation/webdriver/interactions/alerts/)
- Books   :
- Videos  :
