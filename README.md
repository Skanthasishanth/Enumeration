# Enumeration
Enumeration Techniques

# Explore Google Hacking and Enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows

### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:yahoo.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
## Output:

![exp3_1](https://github.com/Skanthasishanth/Enumeration/assets/118298456/2d52a20e-eb9b-49d9-813e-a0ce852b9ccb)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## Output:

![exp3_2](https://github.com/Skanthasishanth/Enumeration/assets/118298456/85d51c97-0e0a-45f7-9b03-4963bf188149)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.


## Output:


![exp3_3](https://github.com/Skanthasishanth/Enumeration/assets/118298456/337ca349-ee18-41b3-9168-dfe5a79a70bb)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.


## Output:

![exp3_4](https://github.com/Skanthasishanth/Enumeration/assets/118298456/91462aa4-19bb-4736-b0df-07563f2c02c7)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.


## Output:

![exp3_5](https://github.com/Skanthasishanth/Enumeration/assets/118298456/3b1ee44c-8e4e-45c3-ac8b-e4dfba947bf2)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:amazon.in" would search for pages that link to the example.com domain.


## Output:

![linkethical](https://github.com/Skanthasishanth/Enumeration/assets/118298456/beb5dfda-e31b-4e5f-bb0f-d13d6b4201f8)


cache: This operator allows you to view the cached version of a page. For example, "cache:amazon.in" would show the cached version of the example.com website.


## Output:

![cacheethical](https://github.com/Skanthasishanth/Enumeration/assets/118298456/95273661-2996-46b9-8671-c668cbb9e9ed)

 
DNS Enumeration

DNS Recon
Provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## Output:

![exp3op1](https://github.com/Skanthasishanth/Enumeration/assets/118298456/2418849a-fee2-4ac1-968d-9a4d9c913e94)



![exp3op2](https://github.com/Skanthasishanth/Enumeration/assets/118298456/8bf6ef4a-f61e-48cb-bea2-5674d0118597)



dnsenum

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


![exp3op3](https://github.com/Skanthasishanth/Enumeration/assets/118298456/ef0c17ba-d7e8-4292-8c3a-7921771af4be)


smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

## Output:

![exp3op4](https://github.com/Skanthasishanth/Enumeration/assets/118298456/2b83fc0f-8200-4928-845c-19a9ec1af43f)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![exp3op5](https://github.com/Skanthasishanth/Enumeration/assets/118298456/66329b0e-154a-4920-8075-7db651353606)


Select any username in the first column of the above file and check the same

![exp3op6](https://github.com/Skanthasishanth/Enumeration/assets/118298456/04d84284-64c4-40f3-b5ba-ee0790426082)




Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
  
## Output:

![exp3_14](https://github.com/Skanthasishanth/Enumeration/assets/118298456/4dd3d0ae-0470-45d4-94c7-e7fe4a8e0621)

  
## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## Output:

![exp3_15](https://github.com/Skanthasishanth/Enumeration/assets/118298456/689f3a1f-e64f-4fad-a5af-d47e9e675943)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
