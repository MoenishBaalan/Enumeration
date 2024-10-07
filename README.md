# ARP-Attack-and-Network-Sniffing
# Explore Network Sniffing and ARP Attacks

# AIM:

To explore network sniffing and ARP Attacks

## STEPS:

- `Step 1:` Install kali linux either in partition or virtual box or in live mode
- `Step 2:` Investigate on the various categories of tools as follows.
-  `Step 3:` Open terminal and try execute some kali linux commands

## ARP Attacks:  
ARP spoofing: A hacker sends fake ARP packets that link an attacker's MAC address with an IP of a computer already on the LAN. 
Boot kali and Windows7 virtual machines.
In windows 7 give the command arp -a
## OUTPUT:
![1](https://github.com/user-attachments/assets/c6634bd1-db53-4426-af49-cffb804507a9)


From kali linux issue the command :
sudo arpspoof -i eth0 -t <target system> <gateway>
## OUTPUT:
![2](https://github.com/user-attachments/assets/edc15c18-9c17-466a-8857-88cb7bf98846)


 dsniff:In Metasploit open the ftp console as below. Also you can try other ftp websites ftp.vim.org
## OUTPUT:
![3](https://github.com/user-attachments/assets/0197312f-fdbf-4ae4-bb2b-5cb2e2fb5a1b)


In Kali issue the following commands:
sudo dsnifff
## OUTPUT:
![4](https://github.com/user-attachments/assets/63d4aba4-f844-40bb-add4-471b93d39fa4)


Invoke the wireshark and examine the various menus  and controls of the tool:
![5](https://github.com/user-attachments/assets/d2fbe44c-df2d-42b2-9444-cfc730f521ac)

## RESULT:
The kali linux tools for ARP Attack and Network Sniffing were identified successfully
