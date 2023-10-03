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

![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/013d2400-7b8f-4c14-bce4-6a56fdbe311a)


##### filetype : 

  This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain youtube.com

![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/0a177cac-edbf-435f-83fe-240eeaca5dcd)


#### intext : 

  This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/532a071e-cc7d-4787-bd1c-07b34e3bcb5f)


#### inurl : 

  This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
  ![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/bb8d397f-e921-4237-a75d-6cba86db1875)


#### intitle :

  This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/ccc0ca72-ee76-4555-b4fe-c7988ddcc7a3)

#### link :

  This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/b6fa4a07-62ae-4fa2-a715-d914578b49cc)

#### cache : 

  This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/177a9925-d658-46ce-99fb-a98c0fc91dbd)

# DNS Enumeration :

## DNS Recon :

Provides the ability to perform:

Check all NS records for zone transfers

Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)

Perform common SRV Record Enumeration

Top level domain expansion

## OUTPUT :
![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/5d35134b-b9a2-4d67-b83b-a554eaaba9ba)

![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/b93a7067-52d0-44e8-9929-4c0ff3930b1b)

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

![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/cf1ac56b-9914-48e4-957e-ce6a0638d55f)


## smtp-user-enum :

  Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
  
![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/0c3fe244-dc36-4683-ae80-b60182fa249d)


  In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/a1b77af9-5abd-41b1-9674-ad6a63f1dab8)


  Select any username in the first column of the above file and check the same
  
![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/a838b5a3-746c-4d52-bc3b-f6f70e1f35c9)


# Telnet for smtp enumeration :

Telnet allows to connect to remote host based on the port no. For smtp port no is 25

telnet <host address> 25 to connect

and issue appropriate commands.
  
## Output :

![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/1ee76fb8-8c63-4d59-8e50-cbf24e12ba1a)


## nmap –script smtp-enum-users.nse <hostname> :

  The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT :

![image](https://github.com/Kirupanandhan/Enumeration/assets/94386222/5814a98f-3e7c-47e5-8f66-cef06436cf2f)


## RESULT :

The Google hacking keywords and enumeration tools were identified and executed successfully.
