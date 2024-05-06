# 4.Execution_of_NetworkCommands
## AIM :Use of Network commands in Real Time environment
## Software : Command Prompt And Network Protocol Analyzer
## Procedure: To do this EXPERIMENT- follows these steps:
<BR>
In this EXPERIMENT- students have to understand basic networking commands e.g cpdump, netstat, ifconfig, nslookup ,traceroute and also Capture ping and traceroute PDUs using a network protocol analyzer 
<BR>
All commands related to Network configuration which includes how to switch to privilege mode
<BR>
and normal mode and how to configure router interface and how to save this configuration to
<BR>
flash memory or permanent memory.
<BR>
This commands includes
<BR>
• Configuring the Router commands
<BR>
• General Commands to configure network
<BR>
• Privileged Mode commands of a router 
<BR>
• Router Processes & Statistics
<BR>
• IP Commands
<BR>
• Other IP Commands e.g. show ip route etc.
<BR>

## CODE
## SERVER
```
import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True: 
    ip=input("Enter the website you want to ping ") 
    s.send(ip.encode()) 
    print(s.recv(1024).decode())
```
## TRACEROUTE COMMAND
```
from scapy.all import* 
target = ["www.google.com"] 
result, unans = traceroute(target,maxttl=32) 
print(result,unans)
```
## SERVER
```
import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True: 
    ip=input("Enter the website you want to ping ") 
    s.send(ip.encode()) 
    print(s.recv(1024).decode())
```
## OUTPUT
## PING COMMAND
## CLIENT:

![image](https://github.com/Mahavidyajp/4.Execution_of_NetworkCommends/assets/144870914/e1243c89-f58d-4507-bb82-d7b4cf6a7fa7)

## SERVER:

![image](https://github.com/Mahavidyajp/4.Execution_of_NetworkCommends/assets/144870914/d77685e0-f036-45b7-8a2b-f42106c9ba67)

## TRACEROUTE COMMAND

![image](https://github.com/Mahavidyajp/4.Execution_of_NetworkCommends/assets/144870914/da66cd96-4f11-45f0-be8a-bc6a60c33470)

## Result
Thus Execution of Network commands Performed 
