# EX 5 Metasploit-for-reconnaissance
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

```
ifconfig
```

## OUTPUT:
![Screenshot 2025-04-19 133832](https://github.com/user-attachments/assets/786a6daa-34fa-44f8-a46d-ab40b7aef5c9)


```
msfconsole
```
## OUTPUT:
![Screenshot 2025-04-19 133854](https://github.com/user-attachments/assets/505059e3-0fa5-4eec-a983-1bcec4de2524)


```
help
```
## OUTPUT:
![Screenshot 2025-04-19 133903](https://github.com/user-attachments/assets/6ad185c0-bbdd-422c-8e2d-98c332a8d14b)




```
nmap -sT <default IP gateway>/24 -p1-1000
```
## OUTPUT:
![Screenshot 2025-04-19 133916](https://github.com/user-attachments/assets/a988f3f4-a5cc-485d-84ae-d5530ea2d6b2)


```
db_nmap <default IP gateway>/24
```
## OUTPUT:
![Screenshot 2025-04-19 133934](https://github.com/user-attachments/assets/c9bef022-ea9d-48db-9869-65082217b52d)


![Screenshot 2025-04-19 133944](https://github.com/user-attachments/assets/7b98a558-03b6-4f82-8813-f21efc4cd2d4)


```
cd /usr/share /metasploit-framework/modules/auxiliary
```
```
 ls -l
 ```

## OUTPUT: 
![Screenshot 2025-04-19 134000](https://github.com/user-attachments/assets/4fdffd28-66e5-4b7f-b427-7665e5dd3316)


```
search name:Microsoft type:exploit
```
## OUTPUT: 
![Screenshot 2025-04-19 134016](https://github.com/user-attachments/assets/d9999f61-dafc-4f2e-96f6-79ffdc1a7bc6)


```
db_nmap -sV -sC -p 3306 <metasploitable_ip_address>
```
## OUTPUT: 
![Screenshot 2025-04-19 134026](https://github.com/user-attachments/assets/26b2b5ad-75a2-47d9-a179-ca9f5cc80559)


```
search type:auxiliary mysql
```
## OUTPUT: 
![Screenshot 2025-04-19 134043](https://github.com/user-attachments/assets/1c10aaed-122f-42b0-a85d-d8f01133dd0d)


```
use 11
```
## OUTPUT: 
![Screenshot 2025-04-19 134053](https://github.com/user-attachments/assets/402210f1-1abc-49d6-88b3-9abd7a2f0893)

```
set RHOSTS <IP>
```
## OUTPUT: 
![Screenshot 2025-04-19 134103](https://github.com/user-attachments/assets/a6335604-c8bf-4da4-abc0-44aeb754dbe2)


```
use auxiliary/scanner/mysql/mysql_login
```
## OUTPUT: 
![Screenshot 2025-04-19 134113](https://github.com/user-attachments/assets/fb09471e-ebb6-49b6-bd08-b22cbde2fa10)


```
set PASS_FILE /usr/share/wordlists/rockyou.txt
```
```
set RHOSTS <metasploitable-ip-address>
```
```
set BLANK_PASSWORDS true
```
```
set verbose no
```
```
run
```
## OUTPUT: 
![Screenshot 2025-04-19 134122](https://github.com/user-attachments/assets/0c35ebac-cb43-4b58-9f2f-9d596db58d42)



## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
