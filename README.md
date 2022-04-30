  <p align="center">
    <img alt="DEDSEC-USB" src="https://github.com/0xbitx/Dedsec-usb/blob/main/dedsec-usb.png" style="max-width:100%;max-height:100%;" />
  </p>

<p align="center"><strong>DEDSEC-USB</strong>
</p>


## DEDSEC-USB
The dedsec-usb looks like any other USB flash drive, but when you insert the dedsec-usb, the computer perceives a keyboard, and it allows that "keyboard" to enter a host of preset keystrokes. Theoretically, this tool is for penetration testing. Security experts can use dedsec-usb to test the resiliency of their computers systems, But hackers can also use the dedsec-usb for keystroke injection attacks.

## Keystroke Injection Attacks

Computers have certain built-in safeguards against flash drives, and they don’t automatically run programs from these devices. In contrast, most computers intuitively trust keyboards. When they receive a keystroke from a keyboard, they assume that a trustworthy user is putting in those keystrokes and they follow the directions.

In light of that, if you put in a dedsec-usb into a computer, the dedsec-usb can tell the computer to take all kinds of actions including the following:

  -   Go to a certain website and download malware or ransomware.
  -   Pull up a website with code that puts a “backdoor” into your system, giving hackers the entrance they need to manipulate accounts or commit other types of fraud.
  -   Launch an app or a reverse-shell program, allowing the hacker to track the keystrokes you enter so they can steal usernames, passwords, and other critical details.
  -   Delete, add, or steal files.
  -   Change server settings to route your online banking customers to a malicious site that steals their information.

This list is just the tip of the iceberg. The potential of these devices is really only limited by the creativity and technical acumen of their users.


## Requirements / Installation
- [Arduino pro micro](https://lazada.com)
- [MicroSD module](https://lazada.com)
- [Dip switch](https://lazada.com)

### Arduino to MicroSD module connection
```
Arduino   |   microSD module  |  Dip switch

VCC     --->    VCC              4 up pins (ON DP)     --->  GND in arduino
                                 4 down pins (1 2 3 4) --->  6 7 8 9 pin in arduino 
D15     --->    SCK

D14     --->    MISO

D16     --->    MOSI

GND     --->    GND

D4      --->    CS
```
<p align="center">
    <img alt="DEDSEC-USB-LAYOUT" src="https://github.com/0xbitx/Dedsec-usb/blob/main/dedsec-usb-layout.png" style="max-width:100%;max-height:100%;" />
  </p>

### flashing dedsec-usb.ino to arduino pro micro
 
 1. double click the dedsec-usb.ino file
 2. click on Tools > Board > Arduino Leonardo.
 3. Click on Tools again, choose Port and the port select Pro Micro.
 4. click the Upload button or press CTRL + U to flash the Pro Micro. You should see “Done uploading.” at the bottom if it’s successful.

 Format your microSD to FAT32 and move your script on the microSD without folder just a txt file script
  
## dip switch code and script function
- 1111 - sticky trick | press shift key 5 times
- 1110 - reverse shell
- 1101 - dump sam file
- 1100 - local dns spoof
- 1011 - enable remote desktop
- 1010 - reverse shell using powershell
- 1001 - disable firewall
- 1000 - disable windows defender using powershell
- 0111 - rickroll
- 0110 - disable windows defender permanently
- 0101 - run metasploit payload
- 0100 - revershell using netcat
- 0011 - run a virus 
- 0010 - add hidden user (user:dedsec password:dedsec1337)
- 0001 - 
- 0000 -

