
2024-07-14 03:45

Status: #adult 

Tags: [[Selenium]]


---

# Broken Images
---
> [!NOTE] 
>  - From the web development when the when the naturalWidth of the image  and it will give pic width  actual width of the image 



---


```java
List<WebElement> images = driver.findElements(By.tagName("img"));
for(WebElement image:images){
	if(image.getAttribute("naturalWidth").equals("0")){
		System.out.println(img.getAttribute("outerHTML") + " is broken.");
      iBrokenImageCount++; 
	}
}

```

---

### Explanation
> Here we can use one more method is call naturalWidth 








## References
- Webpage : [Broken Images](https://www.lambdatest.com/blog/find-broken-images-using-selenium-webdriver/)
- Textbook : [[Sujay Raghavendra - Java Testing with Selenium_ A Comprehensive Syntax Guide for Automation-Apress (2024).pdf#page=147&selection=103,0,103,23|Sujay Raghavendra - Java Testing with Selenium_ A Comprehensive Syntax Guide for Automation-Apress (2024), page 147]]
- mdn refrence : [naturalWidth](https://developer.mozilla.org/en-US/docs/Web/API/HTMLImageElement/naturalWidth)