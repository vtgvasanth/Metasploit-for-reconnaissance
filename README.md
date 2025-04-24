# Metasploit-for-reconnaissance
# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:
Find out the ip address of the attackers system
## OUTPUT:
![image](https://github.com/user-attachments/assets/02d3b593-356c-4a6f-bd66-92f6f7945c2b)


Invoke msfconsole:
## OUTPUT:


![image](https://github.com/user-attachments/assets/33f17cb8-d8bd-466d-9cae-770f2e9182dc)


Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

## OUTPUT:
![image](https://github.com/user-attachments/assets/8caf5a45-c625-4843-81a4-d971723886a1)


![image](https://github.com/user-attachments/assets/ad8e716a-1521-474d-b4f3-24087291b8de)


![image](https://github.com/user-attachments/assets/e2151644-cb45-47b0-b5d6-52dfffd540ae)

![image](https://github.com/user-attachments/assets/50317f1f-c1d7-4b07-aa2e-b87138bdb182)

![image](https://github.com/user-attachments/assets/3676ec8f-8c68-4638-a1a6-bf0be0f55d91)

Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000).
msf >  nmap -sT 192.168.228.34/24 -p1-1000
## OUTPUT:

![image](https://github.com/user-attachments/assets/f6107d55-b6be-419d-ac33-70ab3f5c98ae)


use the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.

scan the targets with the command db_nmap as follows.
msf > db_nmap 192.168.228.34/24
## OUTPUT:

![image](https://github.com/user-attachments/assets/50dea356-0ae7-43f9-83ae-81f7b8666acb)

![image](https://github.com/user-attachments/assets/fabc5012-4f11-4958-820b-3540e66da0cf)

Metasploit has a multitude of scanning modules built in. If we open another terminal, we can navigate to Metasploit's auxiliary modules and list all the scanner modules.
cd /usr/share /metasploit-framework/modules/auxiliary
kali > ls -l
## OUTPUT:

![image](https://github.com/user-attachments/assets/f786a914-c3b4-4315-9d50-493b922e7625)


Search is a powerful command in Metasploit that you can use to find what you want to locate. 
msf >search name:Microsoft type:exploit
## OUTPUT:
![image](https://github.com/user-attachments/assets/0b427bc1-c9a4-4b64-a7c9-b9af195742d5)



The info command provides information regarding a module or platform,
## OUTPUT:
![image](https://github.com/user-attachments/assets/322ff570-5172-4403-9e47-b8fee1f3b2ba)


##MYSQL ENUMERATION
Find the IP address of the Metasploitable machine first. Then, use the db_nmap command in msfconsole with Nmap flags to scan the MySQL database at 3306 port.
db_nmap -sV -sC -p 3306 <metasploitable_ip_address>
## OUTPUT:
![image](https://github.com/user-attachments/assets/094acac8-1f90-4925-94cb-786ca8c3b9bc)



![image](https://github.com/user-attachments/assets/aa2da112-d11c-4b3b-92cd-ab4f5b832bbd)


![image](https://github.com/user-attachments/assets/de1a7e8e-365f-4ec3-b935-8f787efbbc2d)


![image](https://github.com/user-attachments/assets/1b838876-bbbe-4b76-b862-7db49b93a6cb)


## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
