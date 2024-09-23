# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

## AIM:

To use Google for gathering information and perform enumeration of targets

### STEPS:

#### Step 1:

Install kali linux either in partition or virtual box or in live mode

#### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


#### Step 3:
Open terminal and try execute some kali linux commands

### Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

### Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

#### site:
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain youtube.com
![244940886-3f662fef-1bfb-4ada-846b-58e2f02205e0](https://github.com/user-attachments/assets/e711219a-599a-498a-814f-4d2ae11dd2bb)


#### filetype: 
![244940827-8766c43e-431e-4153-a40d-6029bc53a2a8](https://github.com/user-attachments/assets/0310781d-1f4c-4e69-8174-2ee624ba4191)

This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

#### intext:
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![244940830-47678407-b0b8-4964-8181-7c63fc06c5d8](https://github.com/user-attachments/assets/8e6d7fd0-20e5-4cd0-a4e8-8fb2103ea66d)



#### inurl:
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![244940838-489b09da-e059-4a7d-8b87-d38846e4a629](https://github.com/user-attachments/assets/96bf3c52-efd2-4bcd-a54c-74349ecb077a)


#### intitle:
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![244940834-88596beb-c754-4557-bab8-4c235740e33f](https://github.com/user-attachments/assets/dba672f1-521c-46bd-b0a5-257e5374fce9)



#### link:
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![244940813-738671f4-299e-418d-9cbb-506f5dd9b3fd](https://github.com/user-attachments/assets/d507fb7a-042a-4da5-84b6-20f00780358e)


#### cache:
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![244940813-738671f4-299e-418d-9cbb-506f5dd9b3fd](https://github.com/user-attachments/assets/ddc93184-2819-484d-9ca5-00ecda40c3f7)

 
### DNS Enumeration


#### DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
#### OUTPUT:
![244940826-1a3cc453-2a54-4d24-bc01-a4e3b4e8cc36](https://github.com/user-attachments/assets/310f4f9c-15aa-4888-8bee-d38ddc9a31b4)


#### dnsenum
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
![244940820-a9219e21-cd20-4821-9bb7-7daf81066222](https://github.com/user-attachments/assets/5518e032-103f-43b8-9646-e26bb0c7fdec)


#### smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploitble list all the usernames using head /etc/passwd or cat /etc/passwd:
![244940873-e7b5be29-844a-45b3-8459-f5bb01d4b2a4](https://github.com/user-attachments/assets/8220fe30-2e73-4775-9490-dca982bec5a8)


select any username in the first column of the above file and check the same
![244940887-fa58d74f-1f73-4a59-90ef-4b9233bb0872](https://github.com/user-attachments/assets/94b96c23-b967-467d-9bde-cee320c6ba00)



#### Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
#### Output
  ![244940888-cb422b5a-acac-4e09-9b89-76fdc3ba0242](https://github.com/user-attachments/assets/60e3e981-5ca5-4144-9216-ce0a2473ec1d)


#### nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


#### OUTPUT:
 ![244940878-33a55602-856f-419a-b835-bf08376c2138](https://github.com/user-attachments/assets/0e2f74b0-bc81-498c-909b-f582302fcfa7)


### RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
 
