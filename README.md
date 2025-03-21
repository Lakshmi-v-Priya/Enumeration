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
![image](https://github.com/user-attachments/assets/c4b58439-7a22-4b4f-a718-ebf5c654e399)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
![image](https://github.com/user-attachments/assets/da84d773-42a5-41ec-9238-76d501bc7380)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![image](https://github.com/user-attachments/assets/1294e154-149c-4148-a624-e66177d2ea9d)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![image](https://github.com/user-attachments/assets/14c5f733-869f-42d2-bfea-ce5d25e51e34)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![image](https://github.com/user-attachments/assets/289e73e6-7783-43eb-ad6e-e1afb7719018)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/user-attachments/assets/f0c4691b-94d4-45f6-bb90-70719a22905b)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/user-attachments/assets/1259cb18-474c-4987-b2dd-bedd672649a6)

 
# DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
##OUTPUT:
![WhatsApp Image 2025-03-19 at 22 00 38_2d4d8b41](https://github.com/user-attachments/assets/23c5e809-b39e-4fef-9d87-2d35aaeb3ffc)

##dnsenum
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
![WhatsApp Image 2025-03-15 at 13 59 49_1ed61693](https://github.com/user-attachments/assets/0d41a878-c953-4c32-9df8-b58de7de4664)
![WhatsApp Image 2025-03-15 at 14 07 53_bae230ef](https://github.com/user-attachments/assets/c226fcfb-d1b1-4e6f-a742-c12b6ebbd691)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
select any username in the first column of the above file and check the same
![WhatsApp Image 2025-03-15 at 14 08 52_93e7c158](https://github.com/user-attachments/assets/0ae30d9d-3dfd-4c5a-88f5-b320421e0a84)


#Telnet for smtp enumeration:
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
 ##Output:
![WhatsApp Image 2025-03-19 at 22 08 17_2494a517](https://github.com/user-attachments/assets/7a961b5a-a42e-4306-9c4e-48b5e36b1388)
 
## nmap –script smtp-enum-users.nse <hostname>
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
![WhatsApp Image 2025-03-19 at 22 07 36_e2830867](https://github.com/user-attachments/assets/c28b619b-5380-45b5-98eb-ddee3fc2920f)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

