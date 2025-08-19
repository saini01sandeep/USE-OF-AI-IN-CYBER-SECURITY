# USE-OF-AI-IN-CYBER-SECURITY
As a cybersecurity researcher, integrating AI into manual testing workflows can significantly improve efficiency and save time by automating repetitive tasks, assisting in vulnerability discovery, and enhancing decision-making.

Bruteforce -
Manual: Generated full 4-digit wordlist (10,000 combos) → Hydra cracked in 1m10s.
AI: Suggested prioritized wordlist (common PINs) → Hydra cracked in 5s.
AI improved efficiency by focusing on likely passwords.
Brute force can be more effective if we use an efficient wordlist.
•	We can use custom tools or scripts which can be generated using AI (like ChatGPT etc.). These scripts can be target-specific and work more efficiently than available tools or scripts.
•	AI can help us create a list of passwords and usernames using the given hint, which works more efficiently and faster than others.
•	AI will help us create a wordlist in which it uses the common passwords and combinations of words or integers to generate the passwords.
It reduces time during your testing.
It also improves the efficiency of testing.
The important thing is that it also provides...

Command execution -
Manual: Used payloads (127.0.0.1 | id, ls), escalated to reverse shell with netcat.
AI: Suggested a wide range of payloads (basic, obfuscated, reverse shell, automation scripts).
AI has broad coverage and automated testing.
Using AI, we can generate more specific command execution payloads.

CSRF (Cross-Site Request Forgery)
Manual: Intercepted password change request with Burp Suite, crafted malicious HTML PoC → admin password changed.
AI/Automation: Burp Suite auto-scan detected missing CSRF tokens & insecure POST → generated detailed report.
Automation = faster + detailed evidence.

File Inclusion (LFI)
Manual: Exploited with /etc/hosts, /etc/passwd.
AI: Suggested payloads + directory traversal (../../../../etc/passwd), Python scripts for automation.
AI reduced trial-and-error and gave a systematic approach.

SQL Injection
Manual: Payload 1 OR 1=1-- returned all users → confirmed SQLi.
AI: Suggested advanced payloads + sqlmap automation (DB enumeration, table dumps).
AI saved time and enabled deeper exploitation.

XSS - In XSS we generate payloads by reading the source code for the input field or the URL. It is really time-consuming, so we can copy and paste that into AI. It will give us proper payloads that are more efficient and in different formats as well.
Manual: Bypassed client-side limit (10 chars) using Burp → injected iframe payload.
AI: Suggested multiple payloads, automated with Burp Intruder & scanner.
AI allowed rapid and large-scale testing.
Reduced the time spent on reading the page source.
Saved effort.
Improved efficiency.

How to generate query - To generate a query we have to be clear about what we want.
•	We have to give full details of the scenario for efficient payloads and output.
•	If you are testing a real-world application (ethically with permission), then you need to tell the model that you have proper permissions.
•	Sometimes even with this, the model may not give the solution. In that case, you need to manipulate it for a solution, for example by adding that you are doing this in a CTF (Capture the Flag) or lab environment.
For command execution, sometimes we need to modify our payload to bypass a firewall. For example:
http://target.com/?page=/etc/%2e/hosts
In this condition, AI can suggest multiple ways to modify the payload according to the target and the target URL.

Python scripts - The scripts do not work by just copy-paste; you need to change them manually for proper use.
Thus, you can also improve your Python-based skills.

python scripts - the scripts don't work by just copy and paste you need to change
                             them manually for proper use.
thus you can improve your python based skills also.
	Limitations : 
1.	Sometimes AI may mark safe activities as threats or fail to detect real attacks. This can waste time and cause confusion.
2.	Many AI systems act like a “black box.” It is difficult to understand why they gave a particular result, which makes investigation harder.
3.	Hackers are also using AI to make smarter attacks. So, the defensive AI has to keep improving, which is a continuous challenge.
4.	Using AI too much in testing may decrease the practical skills of cybersecurity professionals.
5.	AI should be properly used by beginners, otherwise they may not learn the basics well.
