# Honeypot Assignment

**Time spent:** **2** hours spent in total

**Objective:** Create a honeynet using MHN-Admin. Present your findings as if you were requested to give a brief report of the current state of Internet security. Assume that your audience is a current employer who is questioning why the company should allocate anymore resources to the IT security team.

### MHN-Admin Deployment (Required)

**Summary:** How did you deploy it? Did you use GCP, AWS, Azure, Vagrant, VirtualBox, etc.?
I used GCP to deploy it.

<img src="https://i.imgur.com/VR8rowg.gif">

### Dionaea Honeypot Deployment (Required)

**Summary:** Briefly in your own words, what does dionaea do?
Dionaea aims to trap malware that exploits vulnerabilites and obtain a copy of said malware. 

<img src="https://i.imgur.com/QUGk1tl.gif">

### Database Backup (Required) 

**Summary:** What is the RDBMS that MHN-Admin uses? What information does the exported JSON file record?

The RDBMS uses SQL and the exported JSON file contains attacks and their time stamps.


## Notes

I had to log in and out of MHN-Admin multiple times as I was getting permission denied issues even when running the sudo commands. Other than that, no other issues. 
