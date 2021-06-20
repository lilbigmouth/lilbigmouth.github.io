---
layout: post
---

In the past two months, I had been occasionally seeing slow speeds or even errors when browsing the internet. I have since changed my computer's DNS provider to use
Google's service, which appears to be more reliable. This post describes why you might like to change your DNS provider and how to do so on a Windows 10 system.

## What DNS is

In brief, "The Domain Name System (DNS) is the phonebook of the Internet" (What Is DNS? \| How DNS Works \| Cloudflare UK, n.d.).

Websites are hosted at different Internet Protocol (IP) addresses, such as 10.10.10.5 or more recently with IP version 6: 2001:0db8:85a3:0000:0000:8a2e:0370:7334. 
Of course, humans are extremely unlikely to be able to remember addresses like these so instead we input something such as **lilbigmouth.github.io** into our internet browser.
The DNS translates our human-readable input to the IP address, to allow us to browse to the website we would like to visit.

## Why to change the DNS provider

Typically, a DNS is provided by your Internet Service Provider (ISP). This is the case for me as well. Over the past month or two, I had been occasionally experiencing slow speeds when
selecting "go" or pressing enter after entering the domain name into a browser. More noticably, sometimes this would return a ERR_NAME_NOT_RESOLVED error. This meant
we couldn't browse to the website we wanted, which was quite frustrating.

Google, being the internet giants they are, are typically more reliable for this service. Since I have made the switch, I have experienced no such problems.

## How to change the DNS provider to Google

**Disclaimer**: This will only change the provider that your device uses. These instructions are for a Windows 10 operating system so they may be inaccurate if you
are not using Windows 10. You will need administrator privileges to make this change.

1. Select the network icon, found in the system tray of the taskbar.
2. Select **Network and Internet settings**.
3. Select **Change adapter options**.
4. Right-click on the icon, likely to be named Ethernet. It should have a coloured icon.
5. Select Properties from the context menu. Windows will check for an administrator account at this point.
6. Select Internet Protocol Version 4 (TCP/IPv4).
7. Select Properties.
8. Select "Use the following DNS Server addresses:".
9. To the right of "Preferred DNS Server", enter **8.8.8.8** .
10. To the right of "Alternate DNS Server", enter **8.8.4.4** .
11. Select OK.

You may now close all of the open dialogs. You have now changed your settings to use Google's DNS Server!
To test this is working, open a new tab or window in your internet browser and enter **https://www.google.com** into your address bar. If set correctly, this will take you to the Google website.


## References

What Is DNS? \| How DNS Works \| Cloudflare UK. (n.d.). Cloudflare. Available at: [https://www.cloudflare.com/en-gb/learning/dns/what-is-dns/](https://www.cloudflare.com/en-gb/learning/dns/what-is-dns/).

## Bibliography

Google Developers. (2019). Get Started  \|  Public DNS  \|  Google Developers. Available at: [https://developers.google.com/speed/public-dns/docs/using](https://developers.google.com/speed/public-dns/docs/using).
‌