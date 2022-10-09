# README.md

## What is a Cross site scripting (XSS) Attack?
Cross-Site Scripting (XSS) attacks are a type of injection, in which malicious scripts are injected into otherwise benign and trusted websites. XSS attacks occur when an attacker uses a web application to send malicious code, generally in the form of a browser side script, to a different end user. Flaws that allow these attacks to succeed are quite widespread and occur anywhere a web application uses input from a user within the output it generates without validating or encoding it.  

BUG(XSS): Redirection to  different site 

# Steps to reproduce the mentioned bug:
1) First login into site
        
2) then go to more section and popups folder
        
3) there you will see prompt box
       
4) you can put xss payload in the prompt box(some certain payload work not all of them 
    like prompt() , print()
