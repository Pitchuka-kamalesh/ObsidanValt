---
date: 2024-07-22
Topic: Selenium
Subtopics: fluent wait,
tags:
  - "#adult"
Links:
  - "[[Selenium]]"
Task:
---


---

# Wait for File Download
---

> [!important]
>  Question wait for the file to download and then perform the action 
>  - We have give file location where to save and file name 
>  - Then we have use fluent wait class and then we have check the condition and if file can read and file exists  




---


```java
String downloadPath = "/Users/Downloads";
String fileName = "jenkins.msi"
File file = new File(downloadPath,fileName);

FluentWait<File> wait = new FluentWait<File>(file)
						.withTimeout(Duraction.ofMinitus(5))
						.pollingEvery(Duraction.ofSeconds(50))
						.ignoring(Exception.class)
						.withMessage("File is not downloded");

boolean isDownloaded = wait.until(f -> f.canRead() && f.exists());

if(isDownloaded){
	System.out.println("File is downloaded");
}else System.out.println("File is not downloaded");

```


---

### Explanation
 `File file = new File(downloadPath,fileName)` here we are opening a new file with parameters like downloadPath and fileName as String 
 `FluentWait<File> wait = new FluentWait<File>(file)` here creating wait object with type File and parameter as file and the we are used timeout as 5min and polling period as 50 seconds and we are ignoring the Exception class and with a message  file is not downloaded
 `boolean isDownloaded = wait.until(f -> f.exists() && f.canRead());` here we are checking file is present in particular  and file can be readable  if both conditions are true then it will return true and file is downloaded and if one condition is false then the file is not downloaded.





## References
- Webpage :
- Books   :
- Videos  :https://www.youtube.com/watch?v=Qb3EZYGnono
