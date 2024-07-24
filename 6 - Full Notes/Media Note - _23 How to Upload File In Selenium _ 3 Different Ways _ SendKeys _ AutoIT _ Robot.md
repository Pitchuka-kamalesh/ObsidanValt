---
media: https://www.youtube.com/watch?v=szb7hmv6kG4
---
- sendkeys method 
- autoit
- Robot class 

-  using the sendKeys method to upload a file 
```java
 public class UploadFile(){
	 public static void main(String[] args){
		System.setProperty("webdriver.chrome.driver","driver-path");
		WebDriver driver = new ChromeDriver();
		driver.manage().window().maximize();
		driver.get("https://www.monsterindia.com/seeker/registracton");
		driver.findElement(By.xpath("")).sendKeys("");
	 
	 }
 
 
 }

```

- Second method is using the 
- [06:44](https://www.youtube.com/watch?v=szb7hmv6kG4&t=405#t=06:44.54) 
- AutoIt  
- ![[_23 How to Upload File In Selenium _ 3 Different Ways _ SendKeys _ AutoIT _ RobotPT7M40.837S.webp|#23 How to Upload File In Selenium | 3 Different Ways | SendKeys | AutoIT | Robot - 07:40|50]] [07:40](https://www.youtube.com/watch?v=szb7hmv6kG4&t=461#t=07:40.84) 
- it is used to automate the windows application.
-  -> download and install autoit
-  -> write to script 
-  -> another to locate element 
-  -> we compile script to generate .exe file
-  -> then we are going to excite the exe file 

- -> then we have locate the  

//button[@class='oxd-icon-button oxd-icon-button--solid-main employee-image-action']