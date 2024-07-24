
2024-07-14 02:31

Status: #complete

Tags: [[Selenium]]



---

# Broken Links
---

## Notes
> we have find the links present in the webpage and find that the webpage links are working find by using the HttpURLConnection 
>
>  Link tag in the Html page is `<a>` tag with the attribute  `href` where address value is stored.
>  
> if the URL Response status code is 200 the link is working other wise the link is broken. 


Website for Testing : https://bstackdemo.com/

Screenshot: ![[Pasted image 20240714145024.png]]



---
### Question

How to find the whether the Link is working or not in the Webpage 

---

>Code:


```java

List<WebElement> links = driver.findElements(By.tagName("a");
for(WebElement link : links){
	String linkAddress = link.getAttribute("href");
	verifyLink(linkAddress);
	}
public static void  verifyLink(String link){
	try{
		HttpURLConnection httpConnection = (HttpURLConnection) new URL(link).openConnection();
		httpConnection.setRequestMethod("HEAD");
		int responseCode = httpConnection.getResponseCode();
	
		if( responseCode == 200){
			System.out.println("Valid Hyperlink");
		}else{
			System.out.println("Invalid Hyperlink");
		}
	
		
	}catch(Exception e){
		
		System.out.println(e)
	}
		

}

```


---
#### Explanation 

```java
List<WebElement> links = driver.findElements(By.tagName("a");
```

> `driver.findElements`  -> it will fetch all elements present in the HTML DOM and the main criteria to find by locators  

> `By.tagName("a")`  -> we are fetch all the elements by the tag name `a`
 us locator `tagName`

> `List<WebElements> links` -> we are storing the all web elements with tag name `<a>` are stored in the list with type as `WebElements` and names as links`

```java
for(WebElement link : links){
	String linkAddress = link.getAttribute("href");
	verifyLink(linkAddress);
	}
```

> `for(WebElement link : links)` -> we are using the forEach loop to iterate over the list of WebElements ang getting only one element named as link.

> `String linkAddress = link.getAttribute("href");` -> we are using `getAttribute()` method to get the value of the html tag  `href` is the key where our link url us present and we storing the link href string value in the `linkAddress`. 

> `verifyLink(linkAddress);` --> Created a method to verify that the link is working or not 
> | Name | Type | Description |
> | ---- | ---- | ---- |
> | Link Address | String | this String the input of the `verifyLink()` method|

```java
public static void  verifyLink(String link){
	try{
		HttpURLConnection httpConnection = (HttpURLConnection) new URL(link).openConnection();
		httpConnection.setRequestMethod("HEAD");
	int responseCode = httpConnection.getResponseCode();
	
		if( responseCode == 200){
			System.out.println("Valid Hyperlink");
		}else{
			System.out.println("Invalid Hyperlink");
		}
	
		
	}catch(Exception e){
		
		System.out.println(e)
	}
```


> `HttpURLConnection httpConnection = (HttpURLConnection) new URL(link).openConnection();` -> created a object reference for the *HttpURLConnection* and we type casting *URL* to the *HttpURLConnection* and used a method to open the connection *openConnection()*

> `httpConnection.setRequestMethod("HEAD");` -> in the *httpConnection* we are setting a request method `setRequestMethod()` -> method name is *HEAD* we are only getting headers of the given URL link.

> `int responseCode = httpConnection.getResponseCode();` -> we are using *getResponseCode()* to get the status code of the link href and stored in the datatype *int* and stored in variable name *responseCode*

> `try catch blocks` -> Using *try-catch* block because opening a connection to communicate with the links the link may be faulty and it may brake the total code and close the program that the reason we are using the *try-catch* block  
---
## References
- webpage : [Broken Links ](https://www.browserstack.com/guide/how-to-find-broken-links-in-selenium#:~:text=How%20to%20identify%20broken%20links%20in%20Selenium%20WebDriver,for%20all%20links%20captured%20with%20the%20first%20step)
- Textbook : [[Sujay Raghavendra - Java Testing with Selenium_ A Comprehensive Syntax Guide for Automation-Apress (2024).pdf#page=144&selection=32,0,32,18|Sujay Raghavendra - Java Testing with Selenium_ A Comprehensive Syntax Guide for Automation-Apress (2024), page 144]] 
