# Project 8 - Pentesting Live Targets

Time spent: **5** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each color is vulnerable to only 2 of the 6 possible exploits. First discover which color has the specific vulnerability, then write a short description of how to exploit it, and finally demonstrate it using screenshots compiled into a GIF.

## Blue

Vulnerability #1: SQL Injection

Description:

<img src="https://i.imgur.com/kfcarvH.gif">

Inserting the bit at the end caused the query to fail, whereas on the other colored websites adding it would have done nothing.

Vulnerability #2: Session Hijacking/Fixation 

Description:
<img src="https://i.imgur.com/dqMC9ya.gif">

Changing the session id on a browser that wasn't logged in, to the session id of a browser that was logged in allowed instant access to the contents of the website.

## Green

Vulnerability #1: Username Enumeration

Description:

<img src="https://i.imgur.com/ZiINKfm.gif">

When trying to login with jmonroe99, the unsuccessful login error was bolded, indicating a correct user but wrong password. 
When trying to login with an account that does not exist, in this case Nisha, the error was NOT bolded.

Vulnerability #2: Cross Site Scripting (XSS)

Description:

<img src="https://i.imgur.com/EwVth76.gif">

Inserting the alert into the feedback caused the alert to pop up whenever the admin checked the feedback tab.


## Red

Vulnerability #1: Insecure Direct Object Reference (IDOR)

Description:

<img src="https://i.imgur.com/eDyymBG.gif">

By manually changing the # of the page, we were able to gain access to a page that was yet to be made public.

Vulnerability #2: Cross-Site Request Forgery (CSRF) (Assumption)

Description:

I did not have the time to find the second vulnerability for the red website. Due to the other 5 vulnerabilities being found, I can
only assume that the remaining vulnerability, cross-site request forgery, is the second one for the red website.


## Notes

Due to this being assigned amidst multiple midterms, I did not find ample time to fully finish this assignment, and thus had to leave it incomplete. 
What I did do, however, was very fun to experiment with and I hope to complete this assignment in my own time in the near future. 

