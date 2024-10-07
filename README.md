# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

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

![Screenshot from 2024-09-21 18-15-49](https://github.com/user-attachments/assets/906b34ea-3ec6-442f-9754-85f81d661591)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

### Output:

![eh](https://github.com/user-attachments/assets/cf761a27-2d17-4676-9688-d41708fbbdfd)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

### Output:

![Screenshot from 2024-09-21 18-19-04](https://github.com/user-attachments/assets/fb3d097f-0a27-4cc4-b864-8159e72a00c3)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

### Output:

![Screenshot from 2024-09-21 18-19-52](https://github.com/user-attachments/assets/1f855bee-0bc2-443a-a816-04a0eaafa4d4)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

### Output:

![eh1](https://github.com/user-attachments/assets/a54a8535-749b-4b8e-8b07-305250af66d1)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

### Output:

![Screenshot from 2024-09-21 18-22-02](https://github.com/user-attachments/assets/6b838977-500d-45e4-9afe-c3574974aae5)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
### Output:
![Screenshot from 2024-09-21 18-22-30](https://github.com/user-attachments/assets/119c8d0d-ef5a-4f0c-92d8-3db9f70e672b)

 
# DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![Screenshot from 2024-09-21 18-23-09](https://github.com/user-attachments/assets/a03181d8-2bbc-4fff-a263-d7113d43b449)






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
## Output:
![Screenshot from 2024-09-21 18-23-23](https://github.com/user-attachments/assets/2ab84079-fd50-4f0c-a63b-988ac7d89e55)

![Screenshot from 2024-09-21 18-23-37](https://github.com/user-attachments/assets/116b53dd-fac1-4bf4-8de4-f2f56dd33bec)


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
  
  ![Screenshot from 2024-09-21 18-25-12](https://github.com/user-attachments/assets/37e92783-0233-48a6-b9e0-31f8ab163965)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![Screenshot from 2024-09-21 18-25-34](https://github.com/user-attachments/assets/22d045a6-0ca5-4bf5-9190-e5a4a1f3b602)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

