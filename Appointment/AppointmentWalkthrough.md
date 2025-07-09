Our target machine here is 10.129.223.159 – as always, let’s start with our basic nmap scan:

<img src=Images/Appointment1.png>

Let’s see what exploits are potentially available:

<img src=Images/Appointment2.png>

We know this service is running on port 80, let's try a few methods to login:

Attempt 1 Brute Force: username = admin, password= admin was Unsuccessful 

Attempt 2 SQL Injection: username= ‘ OR 1’=1’, password= irrelevant was Unsuccessful 

Attempt 3 SQL Injection: username= admin, password = ‘ OR 1’=1’ was Unsuccessful 

Attempt 4 SQL Injection: username= admin’#, password= irrelevant was Successful


<img src=Images/Appointment3.png>

Another machine down!

<img src=Images/Appointment4.png>
