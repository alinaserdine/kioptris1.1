<h1>
<b>Enumeration:</b>
</h1>

#### Network Discovery:

- Utilized netdiscover to identify active hosts on the network.
- Discovered target machine at IP address 192.168.133.130.
![image](https://github.com/alinaserdine/kioptris1.1/assets/154693839/9ea7faf6-af71-4dc3-b908-c9991faf31b5)
![image](https://github.com/alinaserdine/kioptris1.1/assets/154693839/f6e9c497-86ea-4622-99d4-30e1c1dda33d)

#### Port Scanning:

- Conducted port scan using nmap to identify open ports on the target.
- Identified port 80 as open, indicative of a web server running.

<h1><b>Exploitation:</b></h1>

#### Vulnerability Assessment:

- Utilized searchsploit to search for exploits relevant to CentOS with kernel version 2.6.
- Discovered a potential exploit for further exploitation.
![image](https://github.com/alinaserdine/kioptris1.1/assets/154693839/920cc9ea-f7b6-4eba-a54d-a45cd1fd130b)

#### Web Application Testing:

- Discovered a web application running on port 80.
- Detected authentication bypass vulnerability using SQL injection.
- Successfully logged in as admin to the web application.
![image](https://github.com/alinaserdine/kioptris1.1/assets/154693839/2be8edae-12a6-4820-b065-418674606ff8)

#### Command Injection:
- Exploited command injection vulnerability within the web application.
- Executed commands to gather system information and escalate privileges.
![image](https://github.com/alinaserdine/kioptris1.1/assets/154693839/fa0c190a-c9ed-4239-8966-f2982d19f3d5)
![image](https://github.com/alinaserdine/kioptris1.1/assets/154693839/ffbaabb7-c565-4a75-aff1-50207a07e02c)

<h1><b>Post-Exploitation:</b></h1>

#### Reverse Shell:
- Established reverse shell connection using netcat.
- Monitored listening port using nc -lvp 1337.
  
![image](https://github.com/alinaserdine/kioptris1.1/assets/154693839/4f74e5a9-1abb-403a-b5bf-6a6ea386b8aa)

#### Exploit Delivery and Execution:
- Set up an HTTP server to host the exploit payload.
- Delivered the exploit to the target system using wget.
- Executed the exploit to gain root privileges on the target system.
![image](https://github.com/alinaserdine/kioptris1.1/assets/154693839/519602da-a53e-43ff-8f90-22f1e6f30d0c)
![image](https://github.com/alinaserdine/kioptris1.1/assets/154693839/f2c653da-9dd3-4765-9573-fbcb44f65f26)
![image](https://github.com/alinaserdine/kioptris1.1/assets/154693839/df4acb2b-3e68-4452-846a-a648452c257f)
![image](https://github.com/alinaserdine/kioptris1.1/assets/154693839/8cfa6c39-87b6-4e9d-ab82-063173c07fc3)

#### Recommendations:

- Patch vulnerable software and update system packages regularly.
- Implement strong authentication mechanisms and input validation in web applications.
- Conduct regular security assessments and penetration testing to identify and mitigate vulnerabilities.

<h1>Conclusion:</h1> The penetration test revealed significant vulnerabilities within the target system, including authentication bypass, command injection, and privilege escalation. It is imperative that appropriate remediation measures are taken to secure the system and prevent potential exploitation by malicious actors.
