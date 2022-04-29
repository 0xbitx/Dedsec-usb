# Dedsec-usb

The dedsec-usb looks like any other USB flash drive, but when you insert the dedsec-usb, the computer perceives a keyboard, and it allows that "keyboard" to enter a host of preset keystrokes. Theoretically, this tool is for penetration testing. Security experts can use dedsec-usb to test the resiliency of their computers systems, But hackers can also use the dedsec-usb for keystroke injection attacks.

## Keystroke Injection Attacks

Computers have certain built-in safeguards against flash drives, and they don’t automatically run programs from these devices. In contrast, most computers intuitively trust keyboards. When they receive a keystroke from a keyboard, they assume that a trustworthy user is putting in those keystrokes and they follow the directions.

In light of that, if you put in a rubber ducky into a computer, the rubber ducky can tell the computer to take all kinds of actions including the following:

  -  Go to a certain website and download malware or ransomware.
  -   Pull up a website with code that puts a “backdoor” into your system, giving hackers the entrance they need to manipulate accounts or commit other types of fraud.
  -   Launch an app or a reverse-shell program, allowing the hacker to track the keystrokes you enter so they can steal usernames, passwords, and other critical details.
  -   Delete, add, or steal files.
  -   Change server settings to route your online banking customers to a malicious site that steals their information.

This list is just the tip of the iceberg. The potential of these devices is really only limited by the creativity and technical acumen of their users.


## requirements 
- arduino pro micro
- microsd module
```
Arduino ||| microSD module

VCC  --->   VCC

D15  --->   SCK

D14  --->   MISO

D16  --->   MOSI

GND  --->   GND

D4   --->   CS
```
- 
## code
- 0000 - reverse shell 
- 0001 - dump password
- 0011 - dump sam file
- 0111 - dns spoof
- 1111 - remote desktop
- 1000 - reverse shell using powershell
- 1100 - disable firewall
- 1110 - disable windows defender using powershell
- 1010 - rickroll
- 0101 - disable windows defender permanently
- 1100 - run metasploit payload
- 0011 - revershell using netcat
- 1001 - 
- 0110 - 
- 1011 - 
- 0111 -

