# Enumeration

# Explore Google hacking and enumeration :

# AIM :

To use Google for gathering information and perform enumeration of targets.

## PROCEDURE :

### STEP 1 :

Install kali linux either in partition or virtual box or in live mode.

### STEP 2 :

Investigate on the various Google hacking keywords and enumeration tools as follows:

### STEP 3 :

Open terminal and try execute some kali linux commands.

## Pen Test Tools Categories :  

Following Categories of pen test tools are identified:

 Information Gathering.

### Google Hacking :

  Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking :

#### site : 

  This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain youtube.com

![img1](https://github.com/anto-richard/Enumeration/assets/93427534/07cb2e4b-9cfd-4aec-b58a-415700a74e48)

##### filetype : 

  This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain youtube.com

![img2](https://github.com/anto-richard/Enumeration/assets/93427534/ca044944-1f93-464a-95a3-c97dfb2fd9ce)

#### intext : 

  This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![img3](https://github.com/anto-richard/Enumeration/assets/93427534/9037a22c-984f-45bd-9da7-4596e3878ce2)

#### inurl : 

  This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
  
![img4](https://github.com/anto-richard/Enumeration/assets/93427534/728cb2b7-8748-4e58-9756-1cae82c82010)

#### intitle :

  This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![img5](https://github.com/anto-richard/Enumeration/assets/93427534/49058ea4-e519-4a2f-a6be-98e0cdf0176c)

#### link :

  This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![img6](https://github.com/anto-richard/Enumeration/assets/93427534/24de08e5-91bc-4322-9d4e-ea38584e7cb4)

#### cache : 

  This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![img7](https://github.com/anto-richard/Enumeration/assets/93427534/0f1d8157-048b-4b76-9606-701be427390a)

# DNS Enumeration :

## DNS Recon :

Provides the ability to perform:

Check all NS records for zone transfers

Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)

Perform common SRV Record Enumeration

Top level domain expansion

## OUTPUT :

![img8](https://github.com/anto-richard/Enumeration/assets/93427534/7bf60783-c4db-48ed-a50e-2d87a4a6b64a)

![img9](https://github.com/anto-richard/Enumeration/assets/93427534/c5cf1863-a8d9-40fa-b45f-f996fd3d7454)

## dnsenum :

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

![img10](https://github.com/anto-richard/Enumeration/assets/93427534/e16a9926-1b0b-457e-b5d4-e29a8342e9f9)

## smtp-user-enum :

  Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
  
![img11](https://github.com/anto-richard/Enumeration/assets/93427534/10b1435a-4964-4568-831a-28983616478d)

  In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![img12](https://github.com/anto-richard/Enumeration/assets/93427534/1bfedc22-915a-4b2b-a796-477516c8f855)

  Select any username in the first column of the above file and check the same
  
![img13](https://github.com/anto-richard/Enumeration/assets/93427534/5f86bc88-1ccc-4637-bc64-78e2dead1d33)

# Telnet for smtp enumeration :

Telnet allows to connect to remote host based on the port no. For smtp port no is 25

telnet <host address> 25 to connect

and issue appropriate commands.
  
## Output :

![img14](https://github.com/anto-richard/Enumeration/assets/93427534/e01fea7c-a06d-4caf-afec-6e59a4067143)

## nmap –script smtp-enum-users.nse <hostname> :

  The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT :

![img15](https://github.com/anto-richard/Enumeration/assets/93427534/74d2a93a-faf0-4dc1-ae98-63e704bd6e65)

## RESULT :

The Google hacking keywords and enumeration tools were identified and executed successfully.
