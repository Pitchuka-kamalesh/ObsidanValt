---
date: 2024-07-19
Topic: File Upload
Subtopics: 
tags:
  - 🦋
  - adult
Links:
  - "[[Selenium]]"
Task:
  - complete the notes and add the cards
---




---

# File Upload using Selenium Java
---

> File upload in web page using selenium are mainly 3 types 
>  - Using sendKeys() method
>  - Using autoit application 
>  - Using Robot class in java 

~~~tabs
tab: sendKeys Method
Basic we are selenium method sendKeys to send path of the file to the webpage.
```java
public class Testers {  
    public static void main(String[] args) throws AWTException, InterruptedException {  
        WebDriver driver = new ChromeDriver();  
        driver.get("https://opensource-demo.orangehrmlive.com/");  
        driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(20));  
        Wait<WebDriver> wait = new WebDriverWait(driver,Duration.ofSeconds(20));  
  
        final WebElement  login_username_input = driver.findElement(By.name("username"));  
  
        final WebElement login_password_input = driver.findElement(By.name("password"));  
  
        final WebElement login_submit_button = driver.findElement(By.xpath("//button[@type ='submit']"));  
  
  
        login_username_input.sendKeys("Admin");  
        login_password_input.sendKeys("admin123");  
        login_submit_button.click();  
  
        final WebElement Navgaction_PIM = driver.findElement(By.xpath("//*[text() = 'PIM']"));  
        Navgaction_PIM.click();  
  
        final WebElement Add_button = driver.findElement(By.xpath("//button[normalize-space()='Add']"));  
        Add_button.click();  
  
        final WebElement loader = driver.findElement(By.xpath("//div[@class='oxd-form-loader']"));  
  
        if(loader.isDisplayed()){  
            System.out.println("loader is present");  
            System.out.println(wait.until(ExpectedConditions.invisibilityOf(loader)));  
            if (wait.until(ExpectedConditions.invisibilityOf(loader))){ 
             driver.findElement(By.xpath("//input[@type='file']")).sendKeys("Filepath"); 
            }  
        }  
  
```
> [!IMPORTANT] here we have find the input tage for the file upload and take action and send keys with the particular file location which you want to send don't click any add button to upload because it will popup windows or linux Explorer to upload file.

tab: Robot Class 
In the robot class we are using inbuild method for performing the keyboard actions and systemclipboard to perform the actions. all the method and class  are avalible in `import java.awt.*` package.
```java
  
Robot robot = new Robot();  
  
StringSelection str = new StringSelection("C:\\Users\\kamal\\Downloads\\issue.jpg");  
Toolkit.getDefaultToolkit().getSystemClipboard().setContents(str,null);  
Thread.sleep(2000);  
  
robot.keyPress(KeyEvent.VK_CONTROL);  
robot.keyPress(KeyEvent.VK_V);  
  
robot.keyRelease(KeyEvent.VK_CONTROL);  
robot.keyRelease(KeyEvent.VK_V);  
  
  
robot.keyPress(KeyEvent.VK_ENTER);  
robot.keyRelease(KeyEvent.VK_ENTER);

```
> [!IMPORTANT] here we will use ROBOT class and perform the action the windows or linux or mac Explorer here we are using the keyboard and mouse action to copy the file path  and copy it into system clipboard and then use use robot class to copy paste it. 

tab: AutoIt
We have to install AutoIt software from the software into the system amd install by using the link [AUTOIT](https://www.autoitscript.com/site/autoit/downloads/) and install and we have to install in the system we have to use 3 tools to excuite the script

- Autoit Window info  it used to get the locatue for the windows pop up 
- Scite editor where we have to create to script to automate 
-  We have to create a exuite file and 
 
```java

```
~~~


![[Pasted image 20240719231326.png]]

>[!ERROR] while doing file upload in orange HRM found an error that can't be clickable then found that form loading is displaying when network is slow first need to check  

> [!IMPORTANT] then checked the loader location and found that check it is visible then it wait until it is invisible to then and the form is present and then perform the action.

## References
- Webpage :[OrangeHRM (orangehrmlive.com)](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login)
- Books   :
- Videos  :


https://youtu.be/szb7hmv6kG4?si=d1iG6RRaIwzB1J_w

 

