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
<img width="1539" height="909" alt="image" src="https://github.com/user-attachments/assets/16712051-89b5-4738-9837-cba8e88e3d86" />


site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
<img width="1725" height="908" alt="image" src="https://github.com/user-attachments/assets/8fc202bf-fc2d-4a4d-92a9-14c4b06cf72b" />


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
<img width="1328" height="905" alt="image" src="https://github.com/user-attachments/assets/5f550cdb-8f72-49c1-b271-d0f8dcd24d7e" />



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
<img width="1319" height="899" alt="image" src="https://github.com/user-attachments/assets/e2f7f0c5-9607-49db-964f-c5b09a48e9dd" />


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
<img width="1314" height="909" alt="image" src="https://github.com/user-attachments/assets/ad91f299-76f9-4e0c-a862-bad7755c4759" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
<img width="1538" height="903" alt="image" src="https://github.com/user-attachments/assets/9900212d-b9d7-4bab-bedf-4728cf0ed8d9" />

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
<img width="1730" height="916" alt="image" src="https://github.com/user-attachments/assets/bf0f947d-d812-4462-b435-5dc4b5cdc6d4" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
<img width="1605" height="854" alt="image" src="https://github.com/user-attachments/assets/6f45b942-db6d-4bcc-a409-059c01a28b0c" />

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
<img width="746" height="603" alt="image" src="https://github.com/user-attachments/assets/53f50f01-1411-4578-943c-84310fffc25f" />







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
<img width="736" height="510" alt="image" src="https://github.com/user-attachments/assets/ea0504e1-a258-4698-888a-6667cabd2477" />


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
 <img width="747" height="415" alt="image" src="https://github.com/user-attachments/assets/193494b9-ac60-4f23-8ed5-ddab3af88dbb" />

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
<img width="680" height="142" alt="image" src="https://github.com/user-attachments/assets/d2a008e2-46af-454b-86ed-f60567eeea89" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

