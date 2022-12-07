## What is Email Analysis?

Email analysis is the process of extracting the **email header** information to expose the email file details.

-   **Social engineering:** Social engineering is the psychological manipulation of people into performing or divulging information by exploiting weaknesses in human nature. These "weaknesses" can be curiosity, jealousy, greed, kindness, and willingness to help someone.
-   **Phishing:** Phishing is a sub-section of social engineering delivered through email to trick someone into either revealing personal information and credentials or executing malicious code on their computer.


## Does Email Analysis Still Matter?

| **Questions to Ask / Required Checks**  | **Evaluation**   |
|---|---|
| Do the "From", "To", and "CC" fields contain valid addresses?  |  Having invalid addresses is a red flag. |
| Do the "From" and "To" fields are the same?  | Having **the same** sender and recipient is a red flag. |
| Do the "From" and "Return-Path" fields are the same?  | Having **differen**t values in these sections is a red flag.  |
|  Was the email sent from the correct server? |  Email should have come from the official mail servers of the sender. |
|  Does the "Message-ID" field exist, and is it valid? | Empty and malformed values are red flags.  |
| Do the hyperlinks redirect to suspicious/abnormal sites?  | Suspicious links and redirections are red flags.  |
|  Do the attachments consist of or contain malware? |  Suspicious attachments are a red flag. <br><br> File hashes marked as suspicious/malicious by sandboxes are a red flag. | 


Email Analysis tool:
**emlAnalyzer**: https://github.com/ninoseki/eml_analyzer

EML analyzer is an application to analyze the EML file which can:

-   Analyze headers.
-   Analyze bodies.
    -   Extract IOCs (URLs, domains, IP addresses, emails) in bodies.
-   Analyze attachments.
    -   Identify whether attachments contain suspicious OLE files.


Other useful investigation tools:

**VirusTotal**  
A service that provides a cloud-based detection toolset and sandbox environment.  

**InQuest**  
A service provides network and file analysis by using threat analytics.  

**IPinfo.io**  
A service that provides detailed information about an IP address by focusing on geolocation data and service provider.

**Talos Reputation**  
An IP reputation check service is provided by Cisco Talos.  

**Urlscan.io**  
A service that analyses websites by simulating regular user behaviour.  

**Browserling**  
A browser sandbox is used to test suspicious/malicious links.  

**Wannabrowser**  
A browser sandbox is used to test suspicious/malicious links.


## Further Try Hack Me Resources

You can find more information on phishing by completing the [**phishing module**](https://tryhackme.com/module/phishing).

