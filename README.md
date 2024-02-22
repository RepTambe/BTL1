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

### Defang
![image](https://github.com/RepTambe/BTL1/assets/56054621/17ddfcd9-097c-42b6-9a38-222fa72001c5)


![image](https://github.com/RepTambe/BTL1/assets/56054621/bf142db6-dc5e-4093-90e2-48a20e1df9bc)


## Example Phishing Report

Email Description and Artefacts Collected
Sending Address: emailsecalert1@gmail.com

Subject Line: Your Email Will be Locked! Act NOW!

Recipients:
john.smith@dicksonunited.co.uk
alice.cooper@dicksonunited.co.uk
jacon.long@dicksonunited.co.uk
fred.johnson@dicksonunited.co.uk
pickle.rick@dicksonunited.co.uk

Sending Server IP: 209.85.222.173

Reverse DNS: mail-qk1-f173.google.com (Gmail)

Reply-To: emailsecalert1@gmail.com

Date and Time: 3:21 PM Monday 1st June 2020

Full URL (sanitized): hxxps://outlook-security.emailsecalerts[.]net/index/2020/OWA.php?

Root Domain: hxxps://emailsecalerts[.]net

Looking at the reported email in the Outlook email client, this message is impersonating an Outlook security alert using branding such as Outlook logos. The email is informing recipients that their mailboxes will be closed unless they confirm their identity, where they are directed to click on a button, likely leading to a credential harvester based on the context of the email.

 

Artifact Analysis
Checking the email gateway shows that there have been no outgoing emails to the sending address, therefore no recipients have replied to the sender.

A reverse DNS search on the sending server IP shows that this email has definitely originated from Gmail, and not Microsoft.

URL2PNG analysis shows that the full URL is an Outlook credential harvester, asking users to enter their email and password.

A VirusTotal search for the domain shows that it has been flagged for malicious and phishing activity, therefore it is known to be malicious within the security community.

Checking the SIEM and EDR no employees have made a network connection to the malicious domain, so no recipients have clicked on the link in the email at this time.

The domain is also attempting to typo squat or appear as a legitimate domain related to email security alerts, trying to make the attack more believable to targets.

 

Suggested Defensive Measures
As the sender is using a Gmail address, the most appropriate action would be to block this specific mailbox to prevent any more incoming malicious emails from this sender.

Requesting an email gateway block for the sending address “emailsecalert1@gmail.com“.

The domain has been recognized as malicious, and there is no business justification for any employees needing to access this site. As it has a malicious reputation on VirusTotal, and analysis has shown that it is hosting a credential harvester, the entire domain can be blocked on the web proxy, preventing employees from connecting to the site. This will also make future phishing attacks using this same domain ineffective.

Requesting a web proxy block for the domain “hxxps://emailsecalerts[.]net“.


# Threat Intelligence

Objectives:
Understand why threat intelligence is used to aid security operations and risk management, by providing enrichment and context to investigations, threats, and vulnerabilities.
Understand and explain what threat actors and advanced persistent threats are, including cybercriminal groups and state-sponsored hackers.
Understand the differences and applications of operational intelligence, tactical intelligence, and strategic intelligence.
Be able to conduct threat exposure checks using indicators of compromise to search the network and assets for any signs of intrusion using known indicators.
Be able to conduct research into threat actors using OSINT sources to gather intelligence such as; alternative names, tools, and malware used, targeted organizations, motives, and indicators of compromise.

![image](https://github.com/RepTambe/BTL1/assets/56054621/69b87f1f-3e2c-4880-93ab-22d50246312a)

![image](https://github.com/RepTambe/BTL1/assets/56054621/750a7dfb-10e3-46ad-bc50-a3d6758be1f3)

COMINT – Communications intelligence related to communications between people and groups of people (messages and voice) and is often synonymous with SIGINT, even though it is considered a discipline of SIGINT.
ELINT – Electronic intelligence is collected from systems not used directly for communications, such as guidance communication for missile systems and radars.

Strategic Threat Intelligence
This type of intelligence provides high-level, typically non-technical information that can be understood by anyone. It is used when presenting to executives and other decision-makers within an organization to aid with decisions such as budget spending and policy review or creation. Below are some examples of strategic intelligence pieces:

A presentation that covers global events and links them with cyber activity (such as the Coronavirus pandemic resulting in an increase of tailored phishing attacks claiming to be from health authorities such as the World Health Organization).
A report on patterns of cyber attacks that the organization is facing over a period of time (such as recognizing that the organization is receiving a more distributed denial of service (DDoS) attacks on Monday, and suggesting plans to mitigate this).
Keeping the internal security team informed about activity related to threat actors that target organizations operating in the same industries (such as the threat intelligence team in a bank monitoring for attacks against other banks, and updating their internal team so they are aware and can prepare for attacks).
Strategic intelligence specialists can be very geographically-focused, understanding the political situation and motives of a country. They will then provide closer tracking of threat actors which have been linked to regions or countries that may pose a threat to the organization based on the industries it operates in. Any geopolitical tension between the country or countries the organization operates in and foreign nations. They will also focus on activity happening within the industry in which the business operates. So strategic analysts at a bank or financial institution would keep track of any cyber attacks that occur within the financial industry.

 

Operational Threat Intelligence
Operational intelligence is all about studying threat actors that might target the organization, in order to gain information about who they are, their motivations, and tactics, techniques, and procedures (TTPs) used to conduct campaigns or prolonged cyber operations. This can help to build more effective defenses by actively monitoring techniques that are used by adversaries, and understanding the actor(s) at a deeper level. This work, which is typically technical, is not easily automated and requires human analysts to track and research malicious groups.

 

Tactical Threat Intelligence
Tactical intelligence is technical in nature and is of immediate value to an organization. It is typically shared in the form of indicators of compromise (IOCs), which are known malicious artifacts such as URLs, domains, email addresses, file hashes, IP addresses, and more. These can either be used by human analysts to check for exposure or can be ingested by security tools via APIs or threat feeds. Below are some examples of tactical intelligence pieces:

A list of email addresses (IOCs) that are being used to send phishing emails containing the Emotet malware is given to an analyst, and they manually check the email gateway security tool to identify any incoming emails from these addresses.
A threat feed that can be subscribed to, which includes a constantly updated list of malicious IPs, is primarily intended to feed into network intrusion prevention systems, so they can autonomously block bad IPs.
A public report from a threat intelligence company that includes a number of IOCs gathered by monitoring exploitation activity targeting a new zero-day vulnerability.

https://www.tenable.com/blog/predictive-prioritization-is-now-available-in-tenable-io
### Precursors: 
Port Scanning, Operating System and Application Fingerprinting
One of the most effective ways to obtain information about a network is through scanning. Using tools such as Nmap, Netcat, or Nessus, both a researcher and an attacker can learn about the services and vulnerabilities that exist on a system. A lot of information can be gained from performing host discovery, port scanning, and vulnerability scanning activities, such as which ports or services are running and responding on a system, what operating system is installed on the system, and what applications and versions of applications are present.

When considering the precursors that this activity would generate, we would mainly be looking to monitor network connections and event logs from internet-facing systems.

Logs from firewalls or web application firewalls (WAFs) that have rules written to alert and log when one source IP is attempting to connect on X number of ports over a short period of time.
Logs from systems that are being scanned.
 

Social Engineering and Reconnaissance
Another way to obtain the greatest amount of information about an organization is, without a doubt, social engineering. This is because, with social skills and deception, both an attacker and a researcher can learn about any type of information and vulnerabilities of an organization. Techniques such as “dumpster diving” (searching for items in the rubbish such as USB sticks, printed documents, notebooks, etc) or “eavesdropping” (Listening to conversations between employees) are very useful for identifying pieces of information that can be brought together to potentially discover vulnerabilities that can be exploited by an attacker.

When considering the precursors that this activity would generate, we would mainly be looking to listen to employee reports of unusual or suspicious activity or CCTV footage from both inside and outside the office.

Non-employees looking through the organization’s bins that are conducting ‘dumpster diving’.
Non-employees hanging around outside the office or lobby areas.
Employees being engaged with outside or near the office by unknown individuals.
Calls from unknown, withheld or spoofed phone numbers.
Documents or office equipment going missing.
 

OSINT Sources and Bulletin Boards
And finally, we have the review of social media, blogs, forums, and bulletin boards, security articles and reports, and other OSINT data both on the clear web and dark web.

When considering the precursors that this activity would generate, we would mainly be looking to monitor OSINT sources using free tools such as TweetDeck and paid intelligence resources such as Recorded Future.

An email or online message from a threat group threatening or stating they will attack the organization.
Publicly disclosed vulnerabilities (CVEs) that affect systems or programs that are used by the organization.
Chatter on underground forums about a zero-day or new malware that is being exploited or utilized in the wild.
Reports stating an increase in vulnerability exploitation activity supplied by government organizations or intelligence vendors.

STIX and TAXII


https://medium.com/mitre-attack/getting-started-with-attack-cti-4eb205be4b2f
https://www.pscp.tv/w/1yoKMVDjbrkGQ

### Attribution

Machine Attribution
Attributing malicious cyber activity to a machine or multiple machines would mean identifying the machine(s) used in an attack. This would usually require examining things like the IP address, log files that document what is happening in the network, who has logged in to the machine. So, we could find out that Azleon’s machine was used in an attack but find a trail leading to Jupiter’s machine which was the originating point of attack. There could be multiple machines in a trail. The IP address may be in another country or require further investigation. Should the IP lead back to Azleon then law enforcement could seize that machine for investigation.

 

Human Attribution
Attributing the malicious activity to a human is finding the identity of the person(s) responsible for the activity, those pushing the keys as it were. Technical forensics which looks at data left behind may not be able to help much further, credentials may point to one person but that may not have been the person physically executing the attack. Credentials get stolen or machines compromised. Technical means may not be enough to identify the person involved as data collected would need to be compared to a database to match an identity, therefore it is only as good as the database. If you can identify the person responsible it is vital to know why it was carried out and if other parties were involved.

 

Ultimately Responsible Attribution
Attributing this malicious activity to the ultimately responsible party answers the question of who is to blame? Was the actor working alone and fully responsible or working on behalf of an organization or nation-state? The “why” is often a more important factor here as people can be coerced into committing these acts, or may be in a position that they feel they can’t refuse. Law enforcement could decide to prosecute an individual or a nation could decide to engage in diplomatic discussion with the offending nation, they might then attribute this to an organization and prosecute or even retaliate.

As you can see the process of assigning attribution can be difficult and complicated, even more so when it is easy to use proxies in other countries. Then requiring deeper and longer investigations will need more cooperation with other agencies.

Key Indicators to attribution
Tradecraft – Frequently used behaviors such as an attacker’s techniques, tools, and procedures used to conduct cyber-attacks.
Infrastructure – The physical machines or networks used in the attack; are often compromised by other means before an attack.
Malware – Malware can be specific to a threat actor; it can be reused or it can be modified quickly if a compromise is suspected to avoid attribution.
Intent – The intent behind the attack, the motivation, or reasoning.
External sources – External reports from organizations like cyber security companies, media even students.
 

Cyber Attribution Techniques
Investigators use many different tools and programs to reveal information about attacks. As an example, let's consider a US-based company that was attacked with malware. This was written in a non-native language, the Cyrillic alphabet. This information can be used by security professionals to help identify the actors behind it. If the malware itself is written with references to Cyrillic, Russian actors could be involved.

Some threat actors, based on their intentions and motived, may WANT to be recognised for their attacks, Example of this could include intentionally fingerprinting malicious files, setting specific filenames during attacks, initiating connections from IP addresses or domains previously linked to the actor, and using custom malware not utilized by any other groups.

 

Issues with Attribution
A major difficulty in analyzing data from attacks is to determine what can be reliable. Metadata such as source IP addresses, email data, domain names, user names, and registration data can all be helpful. Still, it may be faked, through proxies and by using other compromised targets to carry out the attack. The TOR browser can enhance anonymity for malicious actors and automatically encrypts traffic.

Threat actors may choose to share infrastructure to make attribution to a single group harder or use commodity malware or living-off-the-land techniques to prevent identification via the use of unique tools or techniques. Copy-cat attacks can occur where one malicious actor will use the same tools and techniques as another actor in an attempt to trick researchers and threat intelligence analysts into believing the attack was conducted by the other group.

Remember our example of the US company getting hit with malware that include Russian phrases? This could have been engineering by threat actors in another country to try and mislead analysts and researchers!

![image](https://github.com/RepTambe/BTL1/assets/56054621/c16c35ad-f50d-4af9-85ee-d17e29f668d2)

#### IOC monitoring-
is an important part of security operations and can help alert security analysts to malicious activity by monitoring for the presence of any precursors or indicators of compromise across the environment. Watchlists are typically created in either the SIEM or EDR platform (or both).

This allows Threat Exposure Checks (TECs) to be conducted continuously without a need for a human threat intelligence analyst to perform the searches themselves, freeing them up to work on more important tasks.

### public exposure checks-
what we mean is the process a threat intelligence analyst takes to determine what information is publicly available online about their organization, and if this can be exploited in any way to cause damage. This can range from employees posting pictures of them in the office on social media to employee credentials in data breach dumps for sale on the dark web. This work is important and works to protect the organization more than you think.

Image Metadata
Why do we care if people take selfies in the office? – We’re not robots, and let’s face it, we don’t work 100% of the time we’re at work. As long as we’re not disruptive or unproductive it’s usually fine. But taking photos at work can cause some serious issues. You’d be surprised at what information can be contained in a single photo. If you took a photo at work, depending on the device and settings, attackers could potentially discover the make and model of the device you took the photo on, the devices name (we typically name our devices after ourselves, such as “Josh’s iPhone”), the date and time the photo was taken, and in some cases even direct GPS coordinates. If this photo gets posted to social media, an attacker could immediately find the exact location of that office – super not good if it’s a secure or covert site.

 

Leaked Information
Following on from the example above of taking photos or videos in an office, there’s still more damage that can be done. Maybe the selfie looked really good and you’re getting tons of likes on Instagram, but what about the computer screens in the background that are extremely clear, and show the operating system and programs your organization uses. What about the whiteboard on the far wall with confidential business diagrams and information all over it. And the sticky note on someone’s screen with their login details. Even tiny details can help attackers in the long run. An innocent photo could end up being a goldmine of information for attackers, so be careful what you post, and refer to the organization’s social media policy!

 

Early Warnings Signs of Insider Threats
John posts on Twitter that he hates his job. Okay, maybe he’s just had a bad day. John continues to tweet how he’s had enough, he doesn’t get any respect from his peers, and he’s “going to do something about it”. This Tweet could mean a lot of different things – maybe John is going to work extra hard, or just maybe he’s going to become an insider threat, and intentionally cause damage to company assets. The security team can monitor the situation, and work to monitor this individual closer using forensic-grade tools such as DTEX. Whether the employee uses technical skills and access to damage IT equipment, steals confidential documents and gives them to competitors, or works with malicious actors to give them a foothold in the network, monitoring early signs like this could turn out to be nothing, or it could save the organization a lot of money by stopping an attack before it happens.

 

Brand Abuse and Impersonation
Social media account hijacking requires access to legitimate login credentials. Impersonations do not, and therefore are much more dangerous. Impersonations can occur when a threat actor pretends to be an individual or organization, often seeking to either tarnish a reputation, cause general chaos and confusion, or conduct a phishing campaign. With almost no effort, in the digital world, nefarious actors can create digital footprints (websites, social media, e-commerce, apps, etc.) that look like your brand and execute a monetization strategy to target your customers. The immediate impact of brand infringement on your business is lost revenue and eroded customer trust.

Data breaches happen all the time, and unfortunately, sometimes employees get caught up in it. While it is not the job of the security team to alert employees if their personal email addresses have been included in data breaches, it is important when company email addresses are included, especially if passwords were leaked. Password reuse is common, and it won’t go away – it’s just too convenient, but it’s very insecure. If James G was going on a work trip and stayed with The Blue and White Hotel when he books it he’ll probably use his work email, as it’s a work trip, and he can get the expenses refunded by the company. If the hotel gets hacked, and email addresses and passwords are leaked, it’s only a matter of time before someone tries to use James’ credentials elsewhere.

 

Acquiring Data Breach Lists
Sometimes these lists can be shared on the clear web, and threat intelligence analysts can acquire them for analysis, looking for any company-owned email addresses. Other times it can be a lot harder to get access, such as if the list is only being sold to trusted customers on the dark web. Threat intelligence companies around the world work hard to infiltrate dark web marketplaces, and will sometimes purchase data breach lists on behalf of all their clients, allowing them access to only the data related to their organization, reducing further exposure of credentials or private details.

![image](https://github.com/RepTambe/BTL1/assets/56054621/56abea27-9665-4456-852d-6e0f241fff92)


## What Does MISP do?
 

Facilitate the storage of technical and non-technical information about seen malware and attacks
Automatically create relationships between malware and their attributes
Store data in a structured format (allowing automated use of the database to feed detection systems or forensic tools)
Generate rules for Network Intrusion Detection System (NIDS) that can be imported on IDS systems (e.g. IP addresses, domain names, hashes of malicious files, pattern in memory)
Share malware and threat attributes with other parties and trust-groups
Improve malware detection and reversing to promote information exchange among organizations (e.g. avoiding duplicate works)
Create a platform of trust – trusted information from trusted partners
Store locally all information from other instances (ensuring confidentiality on queries)
 

 

 

How Does MISP Work?
 

Malware Information Sharing Platform is accessible from different interfaces like a web interface (for analysts or incident handlers) or via a ReST API (for systems pushing and pulling IOCs). The inherent goal of MISP is to be a robust platform that ensures a smooth operation from revealing, maturing, and exploiting the threat information.

There are 4 options regarding distributing events and their respective attributes:

Your organization only (private)
This community only
Connected communities
All communities (public)
There is also a set of sharing groups accessible to various members per sector (such as the Financial sector).

MISP, Malware Information Sharing Platform and Threat Sharing, core functionalities are:

An efficient IOC and indicators database allows to the storage of technical and non-technical information about malware samples, incidents, attackers, and intelligence.
Automatic correlation finding relationships between attributes and indicators from malware, attack campaigns, or analysis. The correlation engine includes a correlation between attributes and more advanced correlations like Fuzzy hashing correlation (e.g. ssdeep) or CIDR block matching. Correlation can also be enabled or event disabled per attribute.
Built-in sharing functionality to ease data sharing using different models of distributions. MISP can automatically synchronize events and attributes among different MISP instances. Advanced filtering functionalities can be used to meet each organization’s sharing policy including a flexible sharing group capacity and attribute level distribution mechanisms.
An intuitive user interface for end-users to create, update and collaborate on events and attributes/indicators. A graphical interface to navigate seamlessly between events and their correlations. An event graph functionality to create and view relationships between objects and attributes. Advanced filtering functionalities and warning lists to help the analysts to contribute events and attributes and limit the risk of false positives.
Export: generating IDS, OpenIOC, plain text, CSV, MISP XML or JSON output to integrate with other systems (network IDS, host IDS, custom tools), Cache format (used for forensic tools), STIX (XML and JSON) 1 and 2, NIDS export (Suricata, Snort and Bro/Zeek) or RPZ zone. Many other formats can be easily added via the misp-modules.
Import: bulk-import, batch-import, import from OpenIOC, GFI sandbox, ThreatConnect CSV, MISP standard format or STIX 1.1/2.0. Many other formats easily added via the misp-modules.
STIX support: import and export data in the STIX version 1 and version 2 format.


### ISAC 
An example of an ISAC is the Aviation ISAC or a-isac. This is a collective of organizations that operate within the aviation industry and come together to share threat intelligence to help each of the member partners to better defend themselves. You can view their website for more information, and an insight into a real ISAC here

![image](https://github.com/RepTambe/BTL1/assets/56054621/a38c9a6a-e28f-4b6b-9e94-f282e8fefed2)

### Example Walkthrough
 
The strategic threat intelligence analyst at Organisation A receives an email from an analyst at Organisation B, who is in their industry-specific information-sharing partnership (ISAC). Organisation B’s analyst informs the strategic analyst that they have just been hit by an APT who specifically targets the industry they operate in, and during incident response, they collected IOCs including IP addresses that were used to scan and exploit systems at Org B. The strategic analyst then passes these IOCs to a tactical threat analyst who performs threat exposure checks within the SIEM platform to see if the same IPs have scanned Org A recently based on perimeter firewall logs.

The strategic analyst also provides the wider security operations team with a situational awareness email, informing everyone that a similar organization has been hit by an APT and that they may target Org A in the near future.

 
#### TLP

The Traffic Light Protocol was originally created in the early 2000s by the UK Government’s National Infrastructure Security Coordination Centre to promote the greater sharing of sensitive information. While not originally designed specifically for cybersecurity, our industry has widely adopted this approach for sharing sensitive information relating to cyber-attacks and internal documentation.

The purpose of TLP is to allow the author of the original information to state how they want their information to be circulated, such as sharing only with specific individuals, within an organization, within trusted communities, or in the public domain. It is extremely important that if you ever receive a document that uses the TLP system you do not breach the intended level of distribution, as the entire protocol relies on trust.

TLP Clear
Information that is classed as TLP CLEAR can be publicly shared, but copyright rules still apply. Reports or updates that use this TLP are distributed freely for the good of everyone.

 

Example:

The US Cybersecurity and Infrastructure Security Agency (CISA) shares a number of TLP:WHITE analysis reports on malware, and freely shared the related indicators of compromise. Other organizations offer the ability for anyone to subscribe to an email listing that will send out security updates and reports which can be freely shared. We suggest students take a look at a couple of the CISA analysis reports, they’re awesome! – Cybersecurity Alerts & Advisories | CISA

 

 

TLP Green

Information that is classed as TLP GREEN may be shared within communities, such as information sharing and analysis centers (ISACs), which are groups of organizations operating in the same industry or industries. This information should not be shared outside of the intended communities, such as posting it publicly on the internet.

 

Example:

‘Organisation A’ operates in the aviation industry and forms an ISAC with four other companies who all operate in aviation too. One day Org A is subject to a cyber attack from APT33, an Iranian-based threat actor that has been known to target this sector. During the incident response process, Org A collects a number of indicators of compromise (IoCs) such as the email address that sent a spear-phishing email, hashes of malicious files, IP addresses used for command-and-control communication, and so on. Org A has the choice to disclose the IOCs ISAC member organizations to help other companies defend themselves from the same threat actor, but this means these companies (which may be competitors in the business space) will know Org A has been the victim of a successful cyber attack (which could damage the reputation, projected sales, stock price, etc if it is leaked to the public).

 

 

TLP Amber

Information that is classed as TLP AMBER may only be shared internally within an organization on a need-to-know basis to limit who has access to the information.

 

Example:

Penetration test reports, red team engagement reports, and vulnerability scan results are likely to be TLP AMBER as they contain information about serious security flaws that can be exploited to achieve certain actions. Only specific individuals within the organization would need to see these documents, and if they were publicly disclosed there is the chance that malicious actors will find these sensitive reports and could use them to launch effective cyberattacks against the organization because they now have detailed information about the systems, network layout, and vulnerabilities present within that company.

 

 

TLP Amber Strict

This classification restricts sharing to the organization only. TLP:AMBER+STRICT may be used when information requires support to be effectively acted upon however still carries risk to privacy, reputation, or operations if shared outside of the organization.

 

Example:

An Advanced Persistent Threat (APT) group has just launched a new kind of malware. A cybersecurity firm has discovered this malware during an investigation for a client. The malware has a unique signature that has not been detected by any other antivirus or endpoint detection systems yet. The team would continue to investigate and analyse any findings and write up a report, This report would typically include its technical indicators, behaviors, and potential mitigation steps.

In this instance - this report would be classified as TLP AMBER:STRICT as a firm's public report like this could potentially tip off the APT group. This classification would mean tighter restrictions over how the report is distributed, especially within the organization.

 

 

TLP Red

Information that is classed as TLP RED is extremely sensitive and could have severe consequences if it falls into the wrong hands. If an online or in-person meeting is classed as TLP RED then the information should not be shared with anyone that isn’t present in the meeting. Regarding electronic communication such as emails, if an email is TLP RED then only the listed recipients should be exposed to the material, and it should not be shared under any circumstances without the author’s permission.

 

Example:

During a threat hunt, the blue team has discovered what they believe to be an advanced adversary within the network that has Domain Administrator privileges (the highest possible access and permissions). A meeting occurs between the hunting team, the security incident response team (SIRT), and other personnel. Due to the nature of this attack, the organization doesn’t want any information getting out that could alert the adversary that they have been discovered, so only the persons in the meeting are permitted to discuss what has happened.

#### PAP
PAP is a framework designed to classify actions based on the potential exposure of sensitive data to malicious entities. Just as with TLP, the PAP structure also relies upon a tiered system, each distinctly represented by a color code.

PAP Clear
Actions are relatively unrestricted at this level. There are no severe constraints and information can be handled as desired provided they align with legal and licensing frameworks. The primary goal is to ensure a seamless yet compliant handling of the data.

 

 

PAP Green

PAP at this level permits controlled, non intrusive actions with malicious sources.,

This would be likened to something like an organization blocking incoming threats at their firewall, especially if they can trace it back to a particular IP. Similarly, blocking outbound malicious traffic targeting specific web addresses via proxy servers is a standard protocol.

 

 

PAP Amber

Activities at this level are confined to passive data handling, ensuring actions remain undetected by malicious sources.

 

Example:
PAP:AMBER in this instance would be if organizations leverage open-source platforms or online knowledge repositories to further clarify and understand the provided data from an investigation or a breach.

In situations where infrastructure might already be compromised, this data proves pivotal to pinpoint possible IOCs.

Note, that direct or indirect communication with the threat actor is forbidden at this level.

 

 

PAP Red

PAP:RED at this level is centered exclusively around detection and investigation of the threat actor. Just like TLP:RED access is based on a "need-to-know" principle. The infrastructure at hand is typically protected from the public domain but also segregated from the organization's overall system to seclude the information and maintain integrity. In this instance, direct engagements with external services and devices are a strict off limits.

It is expected that permitted actions will be invisible to potential adversaries. A classic example would be searching non-production environments based on previously logged data.

 

Example:
Threat hunting and Incident Response teams are to be mentioned here as they typically have insight and capabilities to monitor infrastructures to confirm the absence or detect the appearance of a threat while maintaining the integrity of the isolated network their are monitoring.

# Digital Forensics

![image](https://github.com/RepTambe/BTL1/assets/56054621/36590cc6-6b27-4a23-b4ea-dfec905860df)
A crucial activity that accompanies the first four steps is contemporaneous notetaking. This is the documentation of what you have done immediately after you have completed it and should provide sufficient detail for another person to reproduce what you have done from the notes alone. The chain of custody, which we cover later in this domain, should also be followed at every stage of the investigation to ensure that evidence integrity is not compromised.

Free Course, Digital Forensics by OpenLearn
// https://www.open.edu/openlearn/science-maths-technology/digital-forensics/content-section-0?active-tab=description-tab


 #### Binary
 It is a simple and elegant design.
Binary’s 0 and 1 method is quick to detect an electrical signal off or on state.
The positive and negative poles of magnetic media are quickly translated into binary.
Binary is the most efficient way to control logic circuits.

#### Base64
Base64 is a reversible encoding algorithm that allows for the transformation of data from the original form to strings such as the one above. We use eight-bit bytes,
VGhpcyBzZW50ZW5jZSBkb2Vzbid0IHJlYWxseSBtZWFuIGEgbG90LiBTb3JyeS4=

#### Hexadecimal
![image](https://github.com/RepTambe/BTL1/assets/56054621/1ccb4010-3b06-4838-8356-4781431191d1)

#### Octal
![image](https://github.com/RepTambe/BTL1/assets/56054621/3381464c-893c-481b-8116-62250836b0d0)

Let’s explain this with an example. Start with a binary number:

10011111
Group the binary number into threes from the right. Add a zero to the left if there are only 2 digits left:

(0)10-011-111
Convert each three-digit group into an octal number by counting from left to right:

2-3-7
Combine the numerals to form the octal number:

237
Using an octal number instead of a binary number saves digits. In the above example we went from 8 digits down to 3, yet the final value still means the same thing as the original. In the early days of computing, octal was often used to shorten 12-bit, 24-bit or 36-bit words. Hexadecimal is now more commonly used in programming, making number representations even shorter than octal.

You’re probably wondering where octal is actually used. Arguably the most common use is in Linux or UNIX file and directory permissions. Using the chmod command, administrators can assign read, write and execute privileges to users and groups.

#### ASCII
ASCII (American Standard Code for Information Interchange) is the most common format for text files in computers and on the Internet. In an ASCII file, each alphabetic, numeric, or special character is represented with a 8-bit binary number (a string of eight 0s or 1s).
![image](https://github.com/RepTambe/BTL1/assets/56054621/1f5171f9-8e8e-46f4-a532-5a840fb4a9ba)


## Data Representation

![image](https://github.com/RepTambe/BTL1/assets/56054621/828e4f54-86be-4225-b147-a8dbdaaf534f)

A hard disk drive platter (or disk) is the circular disk on which magnetic data is stored in a hard disk drive. The rigid nature of the platters in a hard drive is what gives them their name (as opposed to the flexible materials which are used to make floppy disks). Hard drives typically have several platters which are mounted on the same spindle. A platter can store information on both sides, requiring two heads per platter.

A cluster, in the context of a hard disk, is a group of sectors (described above) within a disk and is the grouping by which disk files are organized. A cluster is larger than a sector, and most files fill many clusters of disk space. The hard drive is able to find all the clusters on a disk because each cluster possesses its own unique ID value.
 
Slack space is the leftover storage that exists on a computer’s hard disk drive when a computer file does not need all the space it has been allocated by the operating system. The examination of slack space is an important aspect of computer forensics as we can find the remaining data from previous files allocated in the same cluster. For example, if a user deleted files that filled an entire hard drive cluster, and then saved new files that only filled half of the cluster, the latter half would not necessarily be empty. It may include leftover information from the deleted files that we can retrieve, and may potentially include evidence.

### SSD

#### Garbage
 

Garbage collection is a process used by solid-state drives to optimize space and improve efficiency. The goal of garbage collection is to keep as many empty blocks as possible so that when the SSD needs to write data, it can do so without waiting for a block to be erased. The SSD’s controller looks for any pages that are no longer being used, such as deleted data and modified data. It then moves used pages to new blocks, leaving behind the data that is no longer needed. The controller then erases the block so that it’s ready for use. This is a background process, handled by the SSD controller and the operating system.

Why is garbage collection important in regard to digital forensics? If we have crucial evidence on a system, there’s always the risk that garbage collection will identify the blocks either legitimately or illegitimately as unwanted, and the controller will erase the blocks in order to free up space. If a computer is using solid-state drives, it needs to be powered off immediately to prevent this from happening, either with a hard shut-down (holding the power button until the system turns off), or by pulling the plug so the power supply unit (PSU) receives no electricity. Shutting down the system via the operating system could execute a malicious script that works to destroy data contained on any attached drives, and could ruin an investigation (but we need to remember volatile evidence, which we’ll cover later!).

#### Trim
 

When files are sent to locations such as the Recycle Bin, they are not immediately deleted. Moving them to this location tells the operating system that it is ok to overwrite these files, as they are no longer wanted by the user. If a deleted file is 174192 bytes, and a new file is only 121 bytes, then there will still be 174071 bytes of the deleted file available, so we can recover this and attempt to fix the file so we can see what it was, even with some missing data. However, TRIM operates similarly to Garbage Collection, and instead of telling the SDD to make the size of the deleted file unallocated (available for overwriting), TRIM on an SSD will simply select the data and clear it, removing any chance of forensic investigations recovering the file, or parts of the file.

To counter this, we should take the same actions when dealing with Garbage Collection, as they work together. Power the system off with a hard shut-down or pull the plug (again, we need to remember volatile evidence, which we’ll cover later!).

#### Wear Levelling
 

Wear leveling is a technique that some SSDs utilize to increase the lifetime of the memory using a very simple approach: evenly distribute writing on all blocks of an SSD so they wear evenly. Using this method, all physical cells in the SSD receive the same number of writes, to avoid writing too often on the same blocks, causing damage over time.

Wear leveling is performed by the micro-controller or the firmware of the SSD device. The process of wear leveling is conducted by algorithms, of which there are two basic varieties.

Dynamic wear leveling – When dynamic wear leveling is used blocks that undergo rewriting are repositioned to new blocks. The algorithm selects an empty block on which to write the data. The number of writes to each block is kept track of by the controller. A downside to dynamic leveling is that data blocks that are not frequently updated are not moved which can lead to uneven block wear.
Static wear leveling – The same techniques are employed by static wear-leveling with one important difference. Blocks of static data are moved when their block erase count falls below a certain threshold. This leads to more effective leveling which results in slightly slower write performance countered with enhanced longevity of the device.\

### File Systems


![image](https://github.com/RepTambe/BTL1/assets/56054621/9f5773f4-d045-44a6-805d-046947bf0741)


EXT3 / EXT4
 

Linux Architecture
Before we take a look at EXT3 and EXT4, we’re going to quickly cover the architecture of Linux file systems. These filesystems are divided into three parts:

User Space – The applications are located in the user space, which sends system calls to the system call interface. System call is nothing but a request that is sent to the kernel of the operating system, for a service.
Kernel Space – Kernel is the core of the operating system that answers the system calls from the user space by providing the requested resources, managing the I/O (input/output) devices, memory devices, file management etc.
Disk Space – The device driver in the kernel space sends the I/O request to the hard disk of the system which contains critical file data.
 
Third Extended Filesystem (Ext3)
Third extended filesystem (Ext3), is a journaled file system that is commonly used by the Linux kernel. It is the default file system for many popular Linux distributions. The changes made in the journal, which is a circular log present in the file system, is monitored by ext3 which is called journaling. Journaling filesystem is an additional feature in ext3, which was not in ext2. In a non-journaled filesystem, data recovery and detecting the errors involved more time, as we may have to go through the entire data structure of the directory. But, in a journaled filesystem, we have a journal that keeps track of the changes we do in the file system. So, to detect the errors or recover data, after a crash, it just requires reading the journal instead of processing the whole data structure.

 

Fourth Extended Filesystem (Ext4)
The stable version of ext4 was introduced in 2008 by Linux. The maximum volume size of data supported by ext4 is 1exbibyte and file size is up to 16 tebibytes. The maximum length of the filename is 56 bytes. The fragmentation in terms of physical blocks where data is stored, is replaced by extents. This modification, which was not available in ext2 and ext3, increased the performance of the file system. Extent is a data storage area that reduces file fragmentation and file scattering.


## Digital Evidence

E-mails - These can contain written communication between two or more individuals, and may also contain files as attachments.
Digital Photographs - The photos themselves can be evidence, additionally extra information may be present as photo metadata, which can include the location and device used to take the photograph.
Logs - System logs can contain a wide range of information, depending on the device that has created the log, and the level of logging enabled. Examples can include Windows Event logs that can show login times to show when a user account was accessed.
Files - User files such as notes, code, images, installed software, and more can all provide context about the activity of a user.
Messages - Similar to emails, messages (text, iMessage, Facebook Messenger, WhatsApp, etc) can provide information about a conversation between two or more individuals.
Browser History - This can help us to understand what websites and resources have been accessed from a device, and at what time.
Backups - If files have been deleted, they may be present in backups, allowing us to investigate them even if they have been overwritten on the original storage medium.
Video/audio files - These files, similarly to digital photographs, could be evidence themselves, but could also have metadata to help provide additional information.

Proper handling and securing of evidence are critical. Mistakes in how evidence is acquired can lead to that evidence being tainted and, subsequently, not forensically sound. In addition, if an incident involves potential legal issues, critical evidence can be excluded from being admitted in a criminal or civil proceeding. There are several key tenets for evidence handling that need to be followed, as listed here:

 

– Altering the original evidence: Actions taken by digital forensics examiners should not alter the original evidence. For example, forensic analysts should not access a running system if they do not have to. It should be noted that some of the tasks that will be explored have the potential to alter some of the evidence. By incorporating proper documentation and having a justifiable reason, digital forensics examiners can reduce the chance that evidence will be deemed tainted.

 

– Using write-blockers: Although most forensic software tools have built-in software write blockers, you also need an assortment of physical write blockers to cover as many situations or devices as possible. A write blocker is used to keep an operating system from making any changes to the original or suspect media to keep from erasing or damaging potential evidence. Software write blockers work at the operating system level and are specific to the operating system. In other words, a software write blocker works on only the operating system in which it is installed. A physical write blocker works at the hardware level and can work with any operating system because, at the physical level, the write blocker is intercepting (or, in many cases, blocking) electrical signals to the storage device and has no concern about which operating system is in place.

 

– Document:  One central theme you will often hear in law enforcement is the phrase: “If you didn’t write it down, it didn’t happen.” This is especially true when discussing digital forensics. Every action that is taken should be documented in one way or another. This includes detailed notes and diagrams. Another way to document is through photographs. Proper documentation allows examiners to reconstruct the chain of events if ever the integrity of evidence is called into question.


 ![image](https://github.com/RepTambe/BTL1/assets/56054621/4af76194-96a8-440c-9095-19c440e7389d)


###  Metadata and FileCarving

We can also retrieve metadata in a Linux system by using the same method as above, right-clicking on a file and viewing the properties, or using two commands, ls -lisap <file> and stat <file>, as shown below. In this case, we’re provided with information such as the read/write permissions we have, the file name and size, and the times for when the file was last accessed and modified.
A great command-line tool we can use in Kali Linux is exiftool, which works to retrieve metadata from files

### Why is Memory Forensics Important?
Memory forensics can provide unique insights into runtime system activity, including open network connections and recently executed commands or processes. In many cases, critical data pertaining to attacks or threats will exist solely in system memory – examples include network connections, account credentials, chat messages, encryption keys, running processes, injected code fragments, and internet history which is non-cacheable. Any program – malicious or otherwise – must be loaded in memory in order to execute, making memory forensics critical for identifying otherwise obfuscated attacks.

As attack methods become increasingly sophisticated, memory forensics tools and skills are in high demand for security professionals today. Security solutions such as antivirus programs and endpoint detection and response (EDR) agents may be unable to detect malware written directly into a computer’s physical memory or RAM. Security teams should look to memory forensics tools and specialists to protect invaluable business intelligence and data from stealthy attacks such as fileless, in-memory malware or RAM scrapers.

What is Pagefile.sys?
The Pagefile.sys is used within Windows operating systems to store data from the RAM when it becomes full. The Pagefile.sys is a contiguous file, so it can be read more quickly, that is located on the root of the hard drive and, normally, the more infrequently used memory pages are stored to it. Whilst RAM is used by the system to store active data as, due to the speed of its operation of it, the system functions more quickly than if that data were stored and read from the hard drive. However, through normal use, RAM is filled by the system and then Windows is able to identify which data to move from it to the Pagefile.sys where it can remain until required again.

It can also be used as a backup of data in the event of a system crash. By default, the Windows operating system configures the size of the Pagefile.sys, however, it can also be altered by the user. Normally the Pagefile.sys can be a significant proportion of data present on the hard drive, however, removing it can greatly reduce the operating speed of the computer.

 
Deleting Pagefile.sys
The Pagefile.sys is hidden from the normal Windows user by default as, like many other files on the hard drive, it is a system file that Windows identifies as important in the normal operation of the system. If the file is deleted fully then the system will not function correctly and is likely to become unstable, however, the system can be configured to store the pagefile.sys onto another secondary hard drive.

The Swap file in Linux
Similar to Windows, Linux uses swap space to store RAM when it is full or when the data is not in current use. Within Linux however, traditionally it is a swap partition rather than a swap file and is therefore separate from the other files as it is contained on its own partition. However, it is possible to create a swap file within Linux and to manage the size of that file if required, whereas it is not as easy and sometimes impossible to adjust the size of a swap partition. This can be done via the command sudo fallocate -l [file size] /swapfile once the swap file has been temporarily disabled.

 

Swap space Related Commands in Linux
In order to check the amount of swap space available to the system, the free -h command can be used which will provide the breakdown of total, used and free swap space on the system. The swapon –show command can then be used to identify whether the swap space is a file or a partition. It is also possible to adjust how often the swap space is used within Linux, the default being 60, however, it can be increased from between 0 (for servers) to 100 (for desktop) which makes the system use the swap space more frequently.

What is a Hibernation File?
Starting with Windows 2000, Microsoft introduced the hibernation feature that allows the operating system to store the current state of operation when you turn off the computer, or the system goes into sleep mode. During hibernation everything from memory is copied to the disk in a file called hiberfil.sys, when the computer is restored, the system moves to the saved state. Hibernation files are a good source of information for digital forensic practitioners, as they store data in RAM file without having to run special tools.

### Digital Evidence Collection


Electro-Static Evidence Bags with Tamper-proof Stickers
![image](https://github.com/RepTambe/BTL1/assets/56054621/ad405123-906d-439a-af59-9b5d0e43c0a0)


![image](https://github.com/RepTambe/BTL1/assets/56054621/a925e59c-132f-4600-8b60-701efdd70e88)


![image](https://github.com/RepTambe/BTL1/assets/56054621/de4bd031-6914-41c2-9107-8c91429a2a3b)


## Windows Investigation

Question 1 - Analyze the .LNK files in the Shortcuts folder using Windows File Analyzer - What is the full file name of the PlagueRat file?

Open Windows File Analyzer by right-clicking it and selecting ‘Run as Administrator’ (C:\\Users\\BTLOTest\\Desktop\\Windows Investigation One\\WFA.exe), then choose File > Analyze Shortcuts... and choose C:\\Users\\BTLOTest\\Desktop\\Windows Investigation One\\Shortcuts folder.

Next, look a the row (marked in red) and look at the file name (marked in yellow).

We can see that ‘Plaguerat' is found in the Filename column. Looking along the row we find lots of useful information.

Question 4 - Analyze the Prefetch files using PECmd.exe - What is the full file name of the PlagueRat file in CMD.EXE-89305D47.pf?

Open a command prompt and move to the location of PECmd.exe using cd "C:\Users\BTLOTest\Desktop\Windows Investigation One\PECmd\" , then run the following command:

PECmd.exe -f "C:\Users\BTLOTest\Desktop\Windows Investigation One\Prefetch\CMD.EXE-89305D47.pf"


Question 6 - Analyze the Prefetch files using PECmd.exe - Open all .pf files by pointing PECmd at the /prefetch/ directory using the -d flag. Add the following to your command -k "plaguerat.ps1" to highlight rows that mention this string in red - What two applications were used to open PlagueRat.ps1?

Open a command prompt and move to the location of PECmd.exe, then run the following command:

PECmd.exe -k “plaguerat.ps1” -d "C:\Users\BTLOTest\Desktop\Windows Investigation One\Prefetch\"

Because we've used the -k flag to highlight string matches (PECmd.exe will also match certain strings by default, so not every red-highlighted line will be relevant to us) we can look for red lines to see if they contain ‘plaguerat.ps1’ or not. Going from the bottom of the output upwards we can find our first match:


## Windows Artifacts
Artifact Description

Identifying what user accounts have logged into a system, and at what time, can be useful for both digital forensic investigations and incident response. Doing so can help us attribute activity to a user account by showcasing they were the account signed in before these events occurred. For this artifact, we're looking specifically at:

### Event ID 4624 (Successful Logon)
### ID 4672 (Special Logon)

Special Logon events are when a user with administrative privileges logs into the system.
### ID 4625 (Failed Logon)

Failed Logon events are very useful for us, especially when dealing with incident response. This is because these logs contain error codes, which help us to understand exactly why the logon attempt failed. The different error codes are:
![image](https://github.com/RepTambe/BTL1/assets/56054621/4c647289-56c4-482b-81cb-33523e594a17)

### ID 4634 (Logoff)

One of the most important properties for us to note is the Logon Type, where there are 8 possible values:

2 – Interactive (interactively logged on, meaning a physical logon to the device)
3 – Network (accessed system via network)
4 – Batch (started as an automated batch job)
5 – Service (a Windows service started by service controller)
6 – Proxy (proxy logon; not used in Windows NT or Windows 2000)
7 – Unlock (unlock workstation - think Interactive logon, but unlocking to resume a previous session)
8 – NetworkCleartext (network logon with cleartext credentials)
9 – NewCredentials (used by RunAs when the /netonly option is used)


Question 1) What is the FileName value of the largest deleted file detected?

First, we'll type CMD into the Windows menu and right-click it to run as Administrator. We'll then cd into the Recycle Bin directory.

 


 

Next we'll run RBCmd using the following command:

C:\Users\BTLOTest\Desktop\Recycle-Bin-Analysis\Tools\RBCmd.exe -d . --csv C:\Users\BTLOTest\Desktop\

This will run RBCmd.exe in the Recycle Bin directory, and generate a CSV inside an output folder on our Desktop called “Output”.
 

Next we'll open the CSVQuickViewer application from the folder on the Desktop.


If we receive the Search for app in the Store? popup, we can just click Yes to launch the program anyway.

Click Open File in the top-left corner and select the CSV within the Output folder. We can now start to triage the results!
