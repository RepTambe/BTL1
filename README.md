# BTL1
BTL1 Study! Gold Coin OTW! Started 02/09/24



# Security Fundementals

Learning Objectives:

-Understand the importance of generalized soft skills in the workplace, and how to develop the skills you are weaker in.

-Understand what professional burnout is, how it affects security professionals, and how to take steps to address it.

-Understand what imposter syndrome is, how it affects security professionals, and how to take steps to address it.


### Social Engineering
You're valuable. Not just because you're an awesome person, but because you know information about the company that outsiders don't. You know about the tools they use, internal IP addresses, team members, and lots more information that may seem pointless to you, but can be very valuable to attackers. If you publicly disclose that you work for an organization (Facebook status or employment section of your profile, LinkedIn post or employment history, etc) then you should prepare to receive social-engineering attacks at some point, where malicious actors try to get information out of you in harmless ways. Corporate policies can dictate what can and can't be shared online to reduce this threat, so make sure you read it if your organization has one. And please please PLEASE don't share photos of your work ID badge online! If you're traveling outside of the office, such as going to work or going home, out for lunch, or smoking outside, make sure your badge isn't visible (either in your pocket or if it's on a lanyard, inside your top). Malicious actors may attempt to view how ID badges look so they can design their own and use them to gain unauthorized access to the building.

### Communication Tips

K.I.S.S - "Keep It Simple Stupid" refers to using language that is appropriate for the audience, and that everything is clear and straightforward. If you're speaking to someone in a non-cyber department such as Human Resources, it's unlikely they'll understand what the suspicious connections coming from their work laptop are. It's often better to talk dumb to someone than use jargon and specialist vocabulary that they won't understand, which could give you a wrong answer and take up more time. This can apply to written communication such as emails and messages, and verbal communication.

If someone doesn't understand you, rephrase what you're saying. Don't blame them, and don't feel bad. Try to explain your message in a different way, giving them more information and time to understand what you're saying.

Body language matters. Obviously, this only applies to face-to-face or video communication, but it's an important factor. It will keep your audience engaged, and help to get across your message. Pay attention to the audience's body language, as it can help to identify whether they understand or if they're confused. Formal etiquette also applies in the workplace, and you should be actively showing you're engaged in communication by nodding, focusing on, and keeping eye contact with the speaker (plus it's just polite!).

Keep it professional. While the workplace can be a really social place, you always need to remain professional, after all, you're at work. There may also be company policies that you must abide by during working hours. Do not make racist, sexist, or otherwise derogatory remarks, and think about what you say to ensure it isn't inappropriate. Actions like this will be reported to the organization's Human Resources department, and it is likely they will take disciplinary action against any individuals involved.

### Problem Solving:

Analyzing: Using disciplined thought processes to evaluate each possible solution. Besides listing their costs and benefits, you might apply deductive reasoning, game theory, and the rules of logic (including fallacies) to them.
 
Deciding: The ability to decide on a solution and move forward with it. After an appropriate amount of time, an analysis of possible solutions, and feedback from team members, a designated decider must choose and implement a solution.
 
Managing Emotions: Applying emotional intelligence to improve your own and team members’ ability to think clearly. This requires you to recognize emotions in yourself and others, manage feelings, and channel emotions into useful work.
 

Don't be afraid to think outside of the box, and come up with creative solutions to address problems. At the same time, if you are completely stuck don't be afraid to ask for help, and don't spend too long focused on one problem if you're really unsure how to approach it.

## Security Controls

Physical Security Controls (Deterrents, access controls, monitoring controls) 
Network Security Controls (Firewalls, NIPS, NIDS, SIEM, NAC) 
Endpoint Security Controls (HIPS, HIDS, EDR, Anti-Virus, SIEM) 
Email Security Controls (Spam filters, DLP, email scanning) 

Learning Objectives: 
Understand the basics of physical, network, host, and email security technologies.
Explain what the different security controls do to reduce risk and protect the organization.
Build a foundation of security controls that will be developed throughout the course.

#### ######  Physical Security controls#############

By using Access Controls, we can make it hard for unauthorized individuals to gain access to protected areas. An example of this would be turnstiles at the main entrance that require an RFID badge to unlock and pass through. Using this control, only employees that have a badge with the correct digital keys will be able to pass through.

Monitoring Controls such as CCTV are useful for live monitoring and keeping a record of any malicious behavior so that it can be used in the event of prosecution. CCTV can also be classed as a deterrent, because if people know they’re being recorded, they may be less likely to commit a crime or malicious act.

Deterrents are designed to deter people; an example would be warning signs telling people that if they go any further, they will be trespassing. This may be enough to prevent some people from continuing.


#### Email Security

DLP - ecurity control that works to prevent sensitive business or personal information from leaving the organization in an unauthorized manner. This data can be categorized as files, banking information, account credentials, or PII; for the purpose of this module, we are focusing on the application of DLP technologies to email communication (we’ll cover the other applications of DLP later in the course). Depending on the DLP solution in use, it can monitor outgoing emails at different levels, such as:
email body content
email headers
email attachments of various types

#### Network Security

NIDS- 
Inline - The system running the NIDS software is sitting directly in the path of network traffic, meaning all traffic will pass through the NIDS. In this case, the system will actually by definition become a Network Intrusion Prevention system, as it is able to perform defensive measures such as blocking or resetting connections.

Network Tap - The NIDS will be connected to the network by tapping into a physical connection, such as a cable.

Passive - The NIDS is connected to a SPAN port on a network device. This physical port allows all traffic passing through the device to be mirrored to the SPAN port, so the NIDS will get a copy of all network activity.

Firewall-

Firewalls are used to separate parts of a network to create private zones by restricting the traffic that can come in or go out. The most obvious example is having a physical firewall between the internet and your network, only allowing common protocols in such as HTTP, HTTPS, and DNS. This prevents random hosts from connecting to your systems, which could allow them to be exploited and compromised. There are different types of firewalls, which we will cover later in the course, with the three main being;

Standard firewalls run on dedicated hardware and sit at key points of the network.
Local firewalls in software form run on endpoints (such as Windows firewall).
Web application firewalls in software form sit on internet-facing web servers that host websites or web applications.

Log Monitoring- 
Network devices can generate logs, and these logs can be sent to a SIEM platform. By having logs come from systems across the environment, the SIEM is able to provide a dashboard that analysts can utilize to monitor activity and respond to alerts that are generated when suspicious or malicious traffic is detected. Network devices can provide very valuable information, let's take a look at a couple of examples:

Web Proxy Logs - This device processes web-based requests to the internet, and will contain a list of sites visited by employees. This can be combined with a blacklist to generate SIEM alerts when an employee tries to visit a malicious website or explicit website.

Perimeter Firewalls - If a malicious actor starts port scanning the organization, the perimeter firewalls will pick this activity up first as they get smashed with requests from the scanning IP(s). By sending this to a SIEM an alert can be generated when a port or vulnerability scanning is being conducted, or when distributed denial-of-service attacks (DDoS) start.

### Network Tools

Command Line:
ip or ipconfig- shows current network config of the current device.
ip a - shows the Ip address of the device
ip r list - displays current routing table
ip link set defv [Device Name] up/down - sets the network interface eiter up or down

traceroute [url] - Runs the basic traceroute to see the path it takes to get to a specified address
traceroute [url] -p [port number] - Allows the trace to be run with a specific port

dig [domain name] - Queries the DNS server for the A record for the specified domain
dig [domain name] MX - Queries the DNS server for mail (MX) records for the specified domain
dig [domain name] ANY +nocomments +noauthority +noadditional +nostats - Queries the DNS server for all DNS records for the specified domain and removes the extra information provided by dig

netstat -a - Displays all of the current connections and listening ports on the system
netstat -a -b - Displays all of the current connections and listening ports on the system, as well as their corresponding executable
netstat -s -p tcp -f - Displays the statistics for all connections using TCP and then displays them in an FQDN format

![image](https://github.com/RepTambe/BTL1/assets/56054621/acef4da0-075f-4872-81be-3e495e2bd9ae)

### Risk
![image](https://github.com/RepTambe/BTL1/assets/56054621/23618832-43d2-46bf-bca6-9251e5079085)


# Phising Analysis
Learning Objectives: 
Explain the structure of an email, and how emails are composed, transported, and viewed, in terms of infrastructure, protocols, and clients.

Explain what phishing is, and the impact it can have on both individuals and organizations in regard to confidentiality, integrity, availability, financial, reputation, and other factors.

Understand what phishing is and the impact it can have on businesses and individuals.

![image](https://github.com/RepTambe/BTL1/assets/56054621/d459fa69-1a3b-4761-9ad1-b24a6a610a0a)

### Email Protocol

Simple Mail Transfer Protocol (SMTP)
Simple Mail Transfer Protocol works on TCP port 25 by default, is a communication protocol for electronic mail transmission. Once an email is created it is sent to the organization's SMTP server, which transports the email to the next server, before it eventually reaches the SMTP server of the recipient organization.

However, the world is moving away from port 25 and the new standard is becoming TCP port 587. This port, coupled with TLS encryption, will ensure that email is submitted securely and follows the guidelines set out by the IETF.

 

Post Office Protocol 3 (POP3)
Post Office Protocol (POP) is an application-layer Internet standard protocol used by e-mail clients to retrieve e-mail from a mail server, with version 3 (POP3) being the most widely-used version on the internet. POP works by contacting your email server and downloading all emails from it. Once they are downloaded onto your system, they are deleted from the email server. This means that after the email is downloaded, it can only be accessed using the computer that downloaded the emails, and trying to access your emails from a different device will not work.

 

Internet Mail Access Protocol (IMAP)
IMAP allows you to access your email wherever you are, from any device. When you read an email message using IMAP you're reading it from the email server. As a result, you can check your email from different devices, such as a laptop, desktop, and mobile phone. IMAP still allows for emails to be downloaded, but you must manually click to save the email locally. This method for accessing emails is a lot more common than using POP, as it allows for better accessibility.

In the below diagram, we will be following a scenario where John Smith working at BlackArch Solutions is emailing a friend, Aimee Faren at DicksonUnited. We will cover which protocols are used to deliver emails, and make them accessible by clients.

![image](https://github.com/RepTambe/BTL1/assets/56054621/1f94d88c-438e-4c42-bd64-c297d1b32e66)

Webmail:
While we can access emails via an email client such as the Outlook application or Mozilla's Thunderbird program, a more convenient method is to use webmail. These are web-based email accounts, such as those offered by Hotmail/Outlook, Gmail, and Yahoo Mail. Internet service providers often provide free webmail accounts as part of their internet service package. Webmail allows users to access their emails as long as they have access to an Internet connection and a web browser. As with any web application, webmail's main advantage over the use of a desktop email client is the ability to send and receive email from anywhere via a web browser, such as your laptop, desktop, phone, or tablet. The main disadvantage is that email cannot be accessed without an internet connection, which can be done with an email client, where emails are downloaded and stored locally.

## Tactics

Spam Recon Emails
These emails do not use any tactics, and are simply looking to see if an email error code is sent back to the attacker, such as "undeliverable". This allows the attacker to determine whether the mailbox is in use (no error email sent back means the mailbox is in use, and the email was delivered).

Below is an example of an "undeliverable" message that is displayed when sending emails from Outlook. In this case, we have attempted to send a blank message to a Gmail mailbox that isn't in use.

Social Engineering Recon Emails
These emails will use social engineering techniques, such as posing as a person that the recipient may know or have regular communications with in order to get a response. Other tactics may include creating a sense of urgency, such as "I am about to meet with some important stakeholders, have you read the meeting notes yet?". 

Tracking Pixels Explained
Before we get into tracking pixels within emails, let's define what a tracking pixel is. This is an HTML code snippet that is loaded when a user visits a website or opens an email, very useful for tracking user behavior and preference—if you are an advertiser or hacker.

Data harvesting through a tracking pixel is highly contentious, for many reasons like it being utilized in phishing campaigns, allowing hackers to gather information on their targets.

Tracking Pixel Recon Emails
These emails will typically follow the format of either a spam recon email, or a social engineering email, but are combined with an invisible tracking pixel, which allows the attacker to see if the email has been viewed by an email client. Whilst the other email types can determine if a mailbox is being used, using a tracking pixel can help the attacker understand how active the mailbox is. Monitoring the time it takes between sending the email and having it opened, can help the attacker avoid sending emails to unmonitored mailboxes which would have no impact but increase the risk of detection.

![image](https://github.com/RepTambe/BTL1/assets/56054621/e371233c-a965-4b45-af83-61036814a772)

### Credentail Harvesting
These emails typically feature a lure email that is styled to look like it is from a legitimate company, Impersonating some of the most popular online services and retailers such as Outlook, Amazon, and DHL. The email will tell the recipient to click a button or URL, where they will typically be presented with a real-looking login portal - however, any credentials entered are either stored on the site in an inaccessible directory, or emailed to a dummy account, typically utilizing free online mail services such as Gmail, Hotmail, and Outlook, where the attacker can log in and collect them.

![image](https://github.com/RepTambe/BTL1/assets/56054621/6f9354d1-693c-4d05-8981-07820ccfc712)


### Malicious Files

Can't send an exe, it will be scanned. But Mircosoft office documents are used daily. 

Microsoft Office Macros
MS Office documents such as Word and Excel offer the ability to include macros. These are a series of commands and instructions that can be run automatically once enabled. Macro malware was fairly common several years ago because macros ran automatically when a document was opened. However, in recent versions of Microsoft Office, macros are disabled by default. This means malware authors need to convince users to enable macros so their malware can execute. They do this by showing fake warnings when a malicious document is opened.

****![image](https://github.com/RepTambe/BTL1/assets/56054621/6520770a-80fa-4804-89db-f301ee6df4e6)

Hosted Malware - Hyperlinks. 

![image](https://github.com/RepTambe/BTL1/assets/56054621/09089949-2a3d-4b1c-98e2-08cb887c24db)

![image](https://github.com/RepTambe/BTL1/assets/56054621/17d25cc3-c2c2-4ae8-95a6-4257b7acabc3)


### Homographs
A homograph phishing attack is virtually impossible for users to spot. This attack exploits the fact that many different characters look exactly alike. These characters are called homographs, and the problem is with how the characters are encoded using Unicode.

Wikipedia summarizes that “Unicode incorporates numerous writing systems, and, for a number of reasons, similar-looking characters such as Greek Ο, Latin O, and Cyrillic О were not assigned the same code. So, the Latin “o” and the Cyrillic “o” have a different Unicode and are therefore different letters.” It also means domains with those two different Os are two different domains. Domains using non-Latin letters are referred to as internationalized domain names (IDN) and are used quite frequently in homograph attacks.
![image](https://github.com/RepTambe/BTL1/assets/56054621/53b56201-aacd-46a2-96f3-e907fed24350)

Lure Documents-
Inserting hyperlinks into a malicious email is common, and can potentially be detected easily by email security tools that retrieve URLs and sandbox them to see if the destination is malicious or has a bad community reputation. A way to prevent this is by including the hyperlink in a document, such as a PDF or Microsoft Word file. This means that the attachment itself isn’t inherently malicious, but the hyperlink inside can be. In the below example, this file is a lure document to direct users to “view an invoice online”. The destination URL could simply take the user to a malicious domain that downloads malware to the system.


We can use a URL visualization tool URL2PNG to search for our short Bitly address. When we attempt to view the link, we can see that it is actually showing us the error page on the Security Blue Team site!

### Legit Services

![image](https://github.com/RepTambe/BTL1/assets/56054621/71e91690-95b3-4db6-be2b-b7320ea85ae3)


## Investigating a Phishing Email
#### Email Artifacts:

Sending Email Address
This is where the email has come from or appeared to come from. During the Tactics and Techniques section, we covered spoofing, and how malicious actors can alter what the sending address looks like to make it appear legitimate. Regardless of whether this has obviously been spoofed, we need to record the email address that has apparently sent the email. We can use this as a search term in email gateway security products to identify any other emails that have come from, or been sent to that address.

 

Subject Line
The subject line is a very useful artifact for both searching for other associated emails by using it as a search term in our email gateway security product, or for blocking incoming emails that are in the same attack and using the same subject line.

 

Recipient Email Addresses
We need to identify which mailboxes have received this same phishing email, so we can inform them not to interact with it. Usually, the malicious actor will enter the recipients into the Blind Carbon Copy (BCC) field, so that recipients can’t see who else the email was sent to. To identify recipients we would typically check our email gateway, and search for emails coming from the sending address and including the subject line we have observed, which will give us a list of any other mailboxes that received the same email.

 

Sending Server IP & Reverse DNS
We need to know the address of the server that has sent the email, as this will help us to identify if the sending address has been spoofed. Once we have collected the IP we can perform a reverse DNS search on it using online tools such as Reverse IP Lookup by MXToolbox, which will provide us with a hostname that should give us some more information about the server.

 

Reply-To Address
This is the email address that will receive any replies to the original email. In some cases, this value will be different than the sending address, as if an attacker has successfully spoofed “support@amazon.com” any replies would go to that address, which the attacker won’t have access to. Instead, they can insert an email address of an attacker-controlled account, so now replies will go to “flamingo91591@outlook.com”.

 

Date & Time
It’s good practice to record the date and time an email was sent. Searching for a period of time on either side of the observed time could allow for other emails to be identified that are a part of the same attack or campaign. This can also be used as a metric to see at what times the organization receives the most malicious emails.

#### File Artifacts: 

Attachment Name
The attachment name is a useful artifact when it comes to defensive measures, as depending on the uniqueness of the name, it can possibly be blocked using an organization’s Endpoint Detection and Response (EDR) platform, using the filename as an indicator of compromise. This should always include the file name and file extension.

 

SHA256 Hash Value
A hash, the unique string generated from a file, needs to be recorded as it represents the file in its entirety, and can be used for reputation checks using online tools such as VirusTotal and Talos File Reputation. MD5 and SHA1 hashes should no longer be used, as they have known hash collisions, so SHA256 is the current security standard for file hashing.

#### Web Artifacts:
 

Full URLs
It’s important that when investigating a phishing email that contains a URL that it is copied properly, and not written out by hand, as this can lead to mistakes that will impact the investigation during the analysis stage. The URL should be copied either from the email client by right-clicking the hyperlink and selecting “Copy Link Destination”, or by copying it from a text editor.

 

Root Domain
Whilst this artifact isn’t necessary if you have the full URL, sometimes the root domain can be an important artifact, as it can help show if the site has been created for malicious activity, or if it is a legitimate site that has been compromised.

### Text Editor Extraction
Whilst we can get the majority of the email artifacts we need from a client, there is additional information that we need to collect such as the Sending Server IP (which server has sent the email), and the Reply-To address (where any replies to the email will be sent – this may not always be the initial sender). These can easily be obtained by downloading the email in either .eml or .msg file format and opening the file with a text editor.

When the email opens in the text editor it’ll produce a long document that looks extremely long and complicated – but do not worry, we’re only looking for some specific parts, and we can easily get to them using the Find feature (CTRL+F).

![image](https://github.com/RepTambe/BTL1/assets/56054621/441d51eb-e612-44c0-887a-18dc7868cf4e)




The first thing we want to collect is the sending server IP, also referred to as the **X-Sender-IP**. Press CTRL + F (or your OS equivalent) and search for “IP”. The first string that you find should be the X-Sender-IP (if not, keep clicking “Find” or “Find Prev” until you find it).

 ![image](https://github.com/RepTambe/BTL1/assets/56054621/d8fb3390-2862-4674-9397-7dd63e5c0d6a)


Now that we have the IP, we need to convert the address into a hostname. We can do this by performing a reverse DNS lookup. We recommend you use the free online service by Domain Tools – https://whois.domaintools.com/. If we input the sending server IP we just received (https://whois.domaintools.com/209.85.167.42) we can retrieve information about the server.


 ![image](https://github.com/RepTambe/BTL1/assets/56054621/87de5be7-b2db-4d51-b49f-91244a748f1e)


In the above screenshot, we can see that the host is mail-If1-f42.google.com – a Gmail sending server. Sometimes the sending address domain and sending IP might not match up. If the sender is bob@gmail.com but the IP address belongs to Outlook, we know that the sending address has been spoofed. We’ll cover this in a future lesson.

Next, we need to retrieve the Reply-To address. In the below screenshot, using a different example email, we have used the search function within Sublime Text 2 to look for the string “reply”. We have now identified the address that would receive any replies to this email.

![image](https://github.com/RepTambe/BTL1/assets/56054621/48d6d6c8-9ac4-49ef-b188-424b2e261d71)

#### Conclusion
 

You should now be able to extract the following artifacts from a suspicious email:

Sending Address
Subject Line
Recipient(s)
Date and Time
Sending Server IP
Reverse DNS of Sending Server IP
Reply-To (if present)
 
### Web Email Extraction
Text Editor Extraction
 

In a text editor, we can use the CTRL+F keyboard shortcut to enable the “Find” feature. There are three quick ways to find the URL(s) we want:

Search for “http” as this will identify any http or https addresses being mentioned within the email.
Search for anchor HTML tags <a> which are used to perform hyperlinking.
Search for the text from the email body that is a hyperlink, in this example, we could search for “you can cancel it”.
We’re going to use the last method.

![image](https://github.com/RepTambe/BTL1/assets/56054621/ee6701e0-e23b-4d1b-ab1c-510518e7ece8)


And there we have it, we can see the URL within the <a> HTML tags, and can copy it without fear of accidentally clicking on the link and being taken to a potentially malicious site.


## FIle Artifacts

#### Hashes via PowerShell

We can also retrieve MD5 and SHA1 hashes using the get-filehash command with the -Algorithm switch.
![image](https://github.com/RepTambe/BTL1/assets/56054621/850dbd1e-7eb8-4d43-b08c-b3fbd39d196b)

#### Hashes via Linux CLI

File hashes can be easily retrieved using the Linux command-line. The three commands we would use are;

sha256sum <file>
sha1sum <file>
md5sum <file>

![image](https://github.com/RepTambe/BTL1/assets/56054621/1d647379-a6b9-4274-b781-097d498a5be3)



#### External Emails:

In the below screenshot, we have named our rule “Received from scope Outside the organization”. The rule is applied if:

The sender is outside the organization (securityblue.team domain)
AND the recipient is inside the organization
If these two conditions are met (which will always occur when an external email is delivered to a @securityblue.team mailbox) the following action will be taken:

Prepend the subject of the message with “[EXTERNAL]”

### Email Security Technology
SPF - 
A Sender Policy Framework (SPF) record is a type of DNS (TXT) record that can help prevent an email address from being forged.  This record is established to identify the hostnames or IP addresses that are allowed to send emails for your custom domain.  When having an SPF record specified on your domain, helps prevent a malicious actor from spoofing your domain. The SPF TXT record contains three parts: the declaration of the record type, the IP addresses and external domains that can send on your domain’s behalf, and an enforcement rule.

The basic syntax of the record is:

v=spf1 <IP> <enforcement rule>

For example, securityblue.team has the following SPF record:

v=spf1 a: include:mailgun.org protection.outlook.com -all

We can see that the record declares that it’s an SPF record, that it allows mail to be sent from mailgun.org and protection.outlook.com, and the -all specifies that the email will show a hard fail if the domain is spoofed by an unauthorized sender.


DKIM Records - 
 
Domain Keys Identified Mail (DKIM) is a method of email authentication that cryptographically verifies if an email has been sent by its trusted servers and hasn’t been tampered with during transmission.  The way that DKIM works is that when the mail server sends an email, an encrypted hash of the email contents is generated using a private key and then it adds this hash to the email header as a DKIM signature.  The receiving server will be able to verify whether the email contents have not been tampered with by looking up the corresponding public key in the domain's DNS records.  Once the receiving mail server decrypts the email with the public key, it calculates a new hash and verifies whether the original and the newly generated hash match to ensure email message integrity.

The basic syntax of the record is:

V=DKIM1 <key type> <public key>

DMARC Records
 

Domain-based Message Authentication, Reporting & Conformance (DMARC) is an email authentication, policy, and reporting protocol.  DMARC is built largely off of concepts taken from SPF and DKIM, but it adds several improvements to those protocols.  This type of record allows the domain owner to specify what should happen if emails fail both SPF and DKIM checks.  There are three basic options that the mail server can take: none, quarantine, and reject.

The basic syntax of the record is:

v=DMARC1 <action> <report address>

For example, securityblue.team could have the following DMARC record:

v=DMARC1; p=quarantine; rua=mailto:contact@securityblue.team

We can see that the record declares that it’s a DMARC record, that it sets emails to go to the quarantine/spam folder when failing both checks, and that aggregate reports are sent to contact@securityblue.team of emails that have failed DMARC.

### Spam Filters - 

Gateway Spam Filters – Ones that sit behind an on-premises firewall of a network.  These can often be utilized by larger enterprise organizations and an example of a Gateway filter is the Barracuda email security gateway.
Hosted Spam Filters – These are ones that are hosted within the cloud.  These work very similar to gateway spam filters but are able to update more quickly than some of the on-premises filters and an example of a hosted filter is SpamTitan.
Desktop Spam Filters – These filters are user-installed and are typically used in SOHO scenarios.  One major drawback of these kinds of filters is that they can sometimes be categorized as “Freeware” and you may not fully know what the application is installing on your system.

#### Content Filters
A content filter is the classic depiction of a spam filter and uses information in the email header and body to try to determine whether the email is legitimate or spam.  When looking at the header, the filter could cross-reference the header with published blacklists or known spamming networks and automatically classify it as spam.  When this filter scans the body of the message it could, for example, look for adult-oriented content and determine that as spam, based on preferences set on the account.

 

#### Rule-Based Filters
A rule-based filter allows for emails to be filtered based on predetermined criteria.  A good example of this is Mail Flow rules in Microsoft Exchange where you could say:

If the subject or body contains “FREE OFFER” and the Sender is located Outside of the Organization, raise the likelihood of the message being spam

![image](https://github.com/RepTambe/BTL1/assets/56054621/1751cdbc-7bea-4764-bf5c-bdc469e92677)

#### Bayesian Filters
Bayesian filters have become one of the most intelligent types of spam filters that can be used.  This is because it can often utilize concepts such as machine learning, to learn the users’ spam preferences.  For example, when the user marks an email as spam, it can analyze the characteristics of that message and use that information to block similar messages from going to the inbox.  One slight downside to this kind of filter, however, is that it can often require a large amount of spam to efficiently utilize the machine learning capabilities.

 

While there are many other kinds of filters, the three listed above are some of the most widely used.  One important thing to note about spam filters is that they need to be configured correctly to work properly.  If the individual maintaining a Bayesian filter flags legitimate email, then the system will start classifying legitimate email as spam.  It is important to maintain proper configurations and provide user training on what should and shouldn’t be considered spam.


### Attachment Filtering 

It isn’t a good idea to block attachments outright – employees will have difficulty sending legitimate documents internally and externally. The most appropriate way to approach this situation is to consider what file types are often used for malicious purposes, which file types the organization deals with on a regular basis, and whether blocking them would have any negative impact on the business. The most obvious file types that are used for malicious activity are:

 

.exe (Executable)
.vbs (Visual Basic Script)
.js (JavaScript)
.iso (Optical Disk Image)
.bat (Windows Batch File)
.ps/.ps1 (PowerShell Scripts)
.htm/.html (Web Pages / Hypertext Markup Language)
 

Typically businesses will use and send the following file formats via email, which can also be used for malicious purposes:

 

.zip (Archive)
.doc/.docx/.docm (Document file, often for Microsoft Word)
.pdf (Portable Document Format)
.xls/.xlsx/.xlsm (Spreadsheet file, often for Microsoft Excel)
 

Email gateways and email security tools will often allow for different actions to be taken once a certain attachment has been identified, such as scanning it for malicious indicators, blocking the email from being delivered, quarantining the email, stripping the attachment, alerting the email gateway administrator, sending an email to specific recipients about the activity (such as the security team), or generating logs which can be ingested by a SIEM platform and used to generate an alert for security analysts to investigate.


## Reporting Phishing

Email Header:

Sending Email Address (Ex: J0hnSm1th@gmail.com)
Reply-to Address (Ex: F4keacc0unt2421@gmail.com)
Date Sent (Ex: 20th October 2019, 9:34 AM)
Sending Server IP (Ex: 40.92.10.10)
Reverse DNS of Sending Server IP (Ex: mail-oln040092010100.outbound.protection.outlook.com)
Recipient(s) (Ex: jason.s@domain.com, kirsty.p@domain.com, brian.b@domain.com)
Subject Line (Ex: Payroll Update – URGENT!)
 

Email with URLs:

Any relevant URLs (Sanitised) (Ex: hxxps://Healthcare-United[.]com/wp/index/2020/PAYPAL/lure.php?)
 

Emails with Attachments:

File Name(s) + Extension (Ex: PayrollDecember_UK.exe)
MD5 Hash(es)
You should aim to write approximately 1-2 sentences describing what the email looks like, and what it’s trying to get the recipient to do. We cover two examples below that’ll give you some guidance on how this information, as well as the artifacts, should be presented in a clear and concise manner.
.eml or .msg format

![image](https://github.com/RepTambe/BTL1/assets/56054621/c8df5b25-7167-4826-9e7b-aea9b5cccf8c)

![image](https://github.com/RepTambe/BTL1/assets/56054621/5ceab5ee-b8a5-48ea-b690-6a4a5072db18)
