![244940873-e7b5be29-844a-45b3-8459-f5bb01d4b2a4](https://github.com/user-attachments/assets/ac9cf93c-aca3-487a-9d23-35cf8f42add3)![244940820-a9219e21-cd20-4821-9bb7-7daf81066222](https://github.com/user-attachments/assets/af7711e3-5846-48a3-b742-f6650e2be50b)# Enumeration
Enumeration Techniques

### Explore Google hacking and enumeration 

## AIM:
To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:
Install kali linux either in partition or virtual box or in live mode

### Step 2:
Investigate on the various Google hacking keywords and enumeration tools as follows:

### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

## OUTPUT:

## site:
![268511062-8c0d1184-141e-4aaa-8a91-3ddd1844f11e](https://github.com/user-attachments/assets/2392125a-a922-487c-93cd-cd31a2658c9b)


## filetype:
![268511094-87e84e7c-5c07-432a-a7d0-8facd35bbc6a](https://github.com/user-attachments/assets/e2a64e98-2a5f-41d3-8afd-fb122bd035f9)


## intext:
![268500545-7665d4b8-c069-42a6-9d3c-302be7aed242](https://github.com/user-attachments/assets/cb192c63-22d6-441e-95ad-9645fe646bb7)


## inurl:
![268501006-28f23bcc-97c2-4dd8-9d14-a20789ed61d9](https://github.com/user-attachments/assets/dd6da26c-6fb4-4d7b-9c68-8dfc7681c9db)



## intitle:
![268501095-7efe8ef6-51e0-4993-bacc-c389a5bd542f](https://github.com/user-attachments/assets/5c8ec331-eaf7-4abd-8f45-b544cea9716b)


## link:
![268501046-fcda5d2e-4435-4e9c-a230-1214593bae8d](https://github.com/user-attachments/assets/1797a309-e23d-45d9-8e5d-a09e97b7527c)



## cache:
![268511866-5e3d7922-10bf-4eb9-ba23-68417a2b84c1](https://github.com/user-attachments/assets/b910c488-cc0d-4e98-8c63-fde4faa3604f)



# DNS Enumeration
## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
## nmap –script smtp-enum-users.nse <hostname>
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
### DNS Recon
![244940826-1a3cc453-2a54-4d24-bc01-a4e3b4e8cc36](https://github.com/user-attachments/assets/d78eb6e0-1d72-4c04-899e-f10f7822ed23)


### dnsenum
![244940820-a9219e21-cd20-4821-9bb7-7daf81066222](https://github.com/user-attachments/assets/1ec20780-88a7-4c06-858c-2baab162da60)


### smtp-user-enum
![244940873-e7b5be29-844a-45b3-8459-f5bb01d4b2a4](https://github.com/user-attachments/assets/35270c13-54ed-4711-b789-f33523093708)


### nmap –script smtp-enum-users.nse 
![244940878-33a55602-856f-419a-b835-bf08376c2138](https://github.com/user-attachments/assets/c895566d-ca5a-4d9c-934c-494d265591a1)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

