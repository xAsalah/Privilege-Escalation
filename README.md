# Privilege-Escalation
  <h3> # Kernel Version Exploit! </h3>
Exploit kernel vulnerabilities in order to execute arbitrary code with elevated permissions. 
<br>
<b>Workflow</b>


```
whoami
```
```
Uname –a
```
```
Searchsploit version
```

```
Download exploit
```

```
Run it on the target machine.
```
<h3> # Exploiting Sudo</h3>
Sometime administrators allow users to run specific commands with root privilege. However, if there is, it could be utilised to escalate the privilege. 
<br>
<b>Workflow</b>
<br>

```
sudo -l
```
Search for the found directory in (https://gtfobins.github.io/gtfobins/find/)
<br>
Try to exploit it using commands found in previous website.
<h3> # Exploiting SUID Executables </h3>

<b>Workflow</b>
<br>

```
find / -perm /4000 2>/dev/null 
```
Look for suspicious one
<br>
Open (https://gtfobins.github.io/) and look for the file you have found previously.
Try for shell/su in your shell until you become a root. 
<h3> # Exploit services running as a Root</h3>
Check whether web, mail, database servers are running as a root. 
<br>
<b>Workflow</b>
<br>

```
ps aux | grep root 
```




