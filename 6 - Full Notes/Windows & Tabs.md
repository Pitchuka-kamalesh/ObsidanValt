---
date: 2024-07-22
Topic: Selenium
Subtopics: windows
tags:
  - adult
  - 🦋
  - complete
Links:
  - "[[Selenium]]"
Task: 
Modified: 2024-07-28T03:20:00
---


---

# Windows
---

##### Why we use windows and Tabs in Selenium 
 - tabs are used to open the multiple webpages to do multitasking in one window
 - Window are used to create a separate instances of the browser.

##### In selenium how to get the windows details

- it will give current window handle.
```java
	String window = driver.getWindowHandle();
```
- How to get Multiple Windows handles.
```java
Object[] windows = driver.getWindowHandles().toArray();
```

##### How to switch between windows in selenium.
- We use switchTo().window()
```java
	driver.switchTo().window((String)windows[1]);
	driver.quit();
	driver.switchTo().window(window);
```

##### How to create a new window & new Tab 
- creating a new Window 
```java
	driver.switchTo().newWindow(WindowType.WINDOW);
```
- creating a new TAB 
```java
	driver.switchTo().newWindow(WindowType.TAB);

```

##### How to maximize, minimize and Full screen the windows
- Maximize the window
```java
	 driver.manage().window().maximize();
```
- Minimize the window
```java
	driver.manage().window().minimize();
```
- Full Screen the window
```java
	driver.manage().window().fullscreen();
```


## References
- Webpage :[Working with windows and tabs | Selenium](https://www.selenium.dev/documentation/webdriver/interactions/windows/)
- Books   :
- Videos  :
