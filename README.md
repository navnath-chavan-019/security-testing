# security-testing

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: NAVNATH VISHNU CHAVAN

*INTERN ID*: CT08THZ

*DOMAIN*: SOFTWARE TESTING

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH

## DISCRIPTION OF PROJECT:

**Task: TO CONDUCT SECURITY TESTING TO IDENTIFY VULNERABILITIES LIKE SQL INJECTION OR XSS IN A SAMPLE WEB APPLICATION.**

To perform this acction I used a open-source project (https://demo.testfire.net/login.jsp).
In this project on the login page I try to login without valid credentiols and the result was fail I was not able to login the application,
but with the SQL injection (" OR 1=1--) I was able to login the application as admin.

**Setup Testing Environment**
Before testing, I ensure that I have:

A test web application (like DVWA, Mutillidae, or a custom-built vulnerable app).
A security testing tool (Burp Suite).
A web browser with developer tools (e.g., Chrome DevTools).

**Test for SQL Injection (SQLi)**

As I already know that SQL Injection occurs when an attacker manipulates SQL queries via input fields.

Basically there was login input field, in which I use " OR 1=1-- SQL injection attack and it was successful.
And then I try to enter SQL payloads like:
' OR '1'='1  -- 
" OR "1"="1" -- 
admin' -- 

And it was a success with each one. And then the database returns sensitive information or bypasses authentication, it was vulnerable.

**Preventive Measures**
Encode and escape user input (use HTML entities).
Implement Content Security Policy (CSP).
Use frameworks like React or Angular, which auto-escape data.

**Final Report**
The web application was vulnerable to SQL attack
