## Remote Access Services

**SSH** stands for **Secure Shell**. It was initially used in Unix-like systems for remote login. It provides the user with a command-line interface (CLI) that can be used to execute commands.

**RDP** stands for **Remote Desktop Protocol**; it is also known as Remote Desktop Connection (RDC) or simply Remote Desktop (RD). It provides a graphical user interface (GUI) to access an MS Windows system. When using Remote Desktop, the user can see their desktop and use the keyboard and mouse as if sitting at the computer.

**VNC** stands for **Virtual Network Computing**. It provides access to a graphical interface which allows the user to view the desktop and (optionally) control the mouse and keyboard. VNC is available for any system with a graphical interface, including MS Windows, Linux, and even macOS, Android and Raspberry Pi.


## Authentication

Authentication refers to the process where a system validates your identity.

The user needs to prove their identity. This process is usually achieved by one, or more, of the following:

1.  **Something you know** refers, in general, to something you can memorize, such as a password or a PIN (Personal Identification Number).
2.  **Something you have** refers to something you own, hardware or software, such as a security token, a mobile phone, or a key file. The security token is a physical device that displays a number that changes periodically.
3.  **Something you are** refers to biometric authentication, such as when using a fingerprint reader or a retina scan.


## Attacking Passwords

The following are some of the ways used in attacks against passwords:

1.  **Shoulder Surfing:** Looking over the victim’s shoulder might reveal the pattern they use to unlock their phone or the PIN code to use the ATM. This attack requires the least technical knowledge.
2.  **Password Guessing:** Without proper cyber security awareness, some users might be inclined to use personal details, such as birth date or daughter’s name, as these are easiest to remember. Guessing the password of such users requires some knowledge of the target’s personal details; their birth year might end up as their ATM PIN code.
3.  **Dictionary Attack:** This approach expands on password guessing and attempts to include all valid words in a dictionary or a word list.
4.  **Brute Force Attack:** This attack is the most exhaustive and time-consuming, where an attacker can try all possible character combinations.


## Hacking an Authentication Service

Ex.

we open a terminal and use Nmap to scan the target machine of IP address `10.10.201.171`.

**`nmap -sS 10.10.201.171`**

We want an automated way to try the common passwords or the entries from a word list; here comes [THC Hydra](https://github.com/vanhauser-thc/thc-hydra). 

Hydra supports many protocols, including SSH, VNC, FTP, POP3, IMAP, SMTP, and all methods related to HTTP. 

**`hydra -l username -P wordlist.txt server service`**




## Further Try Hack Me Resources
	
You can learn more about THC Hydra by joining the [Hydra](https://tryhackme.com/room/hydra) room. The general command-line syntax is the following:

If you liked the topics presented in this task, check out these rooms next: 
- [Protocols and Servers 2](https://tryhackme.com/room/protocolsandservers2)
- [Hydra](https://tryhackme.com/room/hydra),
- [Password Attacks](https://tryhackme.com/room/passwordattacks)
- [John the Ripper](https://tryhackme.com/room/johntheripper0).
