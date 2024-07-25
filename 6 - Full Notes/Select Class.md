---
Created: 2024-07-25T11:47:00
Topic: Selenium
Subtopics: Select Class
tags:
  - 🦋
  - adult
  - complete
Links:
  - "[[Selenium]]"
Task:
  - Complete Total Select Class
Modified: 2024-07-25T14:56:00
---


---

# Select Class
---
- ***Select Class*** is used with `<select>` tag and it is used to select the For the Dropdown menu and there are two types of  one and multiple select option are available.
  
  Single Option Select
  
```html

<select name="selectomatic">
    <option selected="selected" id="non_multi_option" value="one">One</option>
    <option value="two">Two</option>
    <option value="four">Four</option>
    <option value="still learning how to count, apparently">Still learning how to count, apparently</option>
</select>

```


Multi Option Select 

```html
<select name="multi" id="multi" multiple="multiple">
    <option selected="selected" value="eggs">Eggs</option>
    <option value="ham">Ham</option>
    <option selected="selected" value="sausages">Sausages</option>
    <option value="onion gravy">Onion gravy</option>
</select>

```

- ##### Creating a Select Object 

  - First we have create an select object using the new keyword and the attribute 

```java
	WebElement selectElement = driver.findElement(By.name("selectomatic"));
	Select select = new Select(selectElement);
```

 - get all the options  :
 ```java
	 List<WebElement> optionsList = select.getOptions();
```

- Get all the selected options:
  
``` java
	 List<WebElement> selectedOptions = select.getAllSelectedOptions();

```

- Select Options :
	- ***selectByValue***
	- ***selectByVisibleText***
	- ***selectByIndex***

 selectByValue
 ```java
 select.selectByValue("two");
```
selectByVisibleText
```java
 select.selectByVisibleText("Two");
```
selectByIndex
```java
	select.selectByIndex(2);
```
- De-select option:
```java
	select.deselectByValue("two");
```


## References
- Webpage : [Select_lists](https://www.selenium.dev/documentation/webdriver/support_features/select_lists/)
- Books   :
- Videos  :
