---
title: "Cracked: Surveillance architecture"
modified: 2019-11-02T15:40:00+00:00
categories:
  - Elephants
tags:
  - Causes and effects
  - Elephants
  - Information
  - Surveillance
---
_To put it bluntly, metadata is hidden data that can fuck you over. Fuck you over real hard and rough like, savvy? Often defined as “data about data,” metadata is information about a specific file that’s often included within the file itself but that’s often not readily visible or modifiable to the end-user when z is viewing the file in the standard application that z would typically use to view the file. In other words, metadata provides background information about a file. Chances are that every document you create, every digital photograph you take, every music file you download, and so on, all have little bits of metadata which can leak vital information about your identity._ ~ [The dangers of metadata, 2008](http://www.textfiles.com/uploads/diz-usp3.txt) 

[![Surveillance architecture, March 9, 2015, 11 minute read]({{ site.url }}{{ site.baseurl }}/assets/images/surveillance-architecture.png#center)](https://labs.rs/en/invisible-infrastructures-surveillance-achitecture/)

[![Data flow, March 7, 2015, 11 minute read]({{ site.url }}{{ site.baseurl }}/assets/images/data-flow.png#center)](https://labs.rs/en/invisible-infrastructures-data-flow/)

The Snowden leaks revealed a massive surveillance program including interception of email and other internet communications and phone call tapping. Upstream collection, Hemisphere and XKeyScore by way of wealthycluster2 gobble up our metadata, and with interconnected systems such as by ICReach that data can be shared and associated with other data. There are dozens of clever analyses you can perform with such linked databases. I'm sure that is what they're doing right now. If I can think of it, so did they.

And it is not just the US spying on its citizens and its “adversaries”. Every citizen on this planet is subject to dragnet surveillance. This includes data that does not, by itself, identify individuals, but sits in various databases until analysts do a search for a particular name. 

| Assets | Threat(s) | Mitigation(s) | 
| --- | :-- | :-- | 
|Communications |Nearly all states are copying and searching the communications (for example email addresses) and content of virtually every communication that comes into or goes out of the country, without a warrant. |Use encryption. Intelligence agencies target encrypted traffic, but any encryption is still better than sending traffic in the clear.|
|Encryption software |Be suspicious of commercial encryption software, especially from large vendors: The secret agreements between intelligence agencies and technology companies extends to those developing security and encryption software.[(For avoiding implicitly backdoored algorithms: Try to use public-domain encryption that has to be compatible with other implementations as much as possible: Do not use proprietary software; Avoid elliptic-curve systems.)|Assume that every commercial application has an intelligence-agency-friendly back door.|
|IP address|Packet headers identify the IP addresses of sender(s) and recipient(s) and the packet routes can rather easily be tracked. |Use tunnelling (VPN or SSH) or Tor and when doing so never ever post any personal data. Communications can be encrypted so that an observer cannot learn the content of these transmissions easily (it will cost), but this still reveals the fact that two parties are communicating|
|MAC address|MAC addresses can be and often are used by networking equipment to track users. This means proxy hopping on a network that has already authenticated your hardware is utterly useless. |Regularly change mac address|
|Video metadata| There are two sources in which video metadata is derived: operational gathered metadata - information about the content produced, such as the type of equipment, software, date, and location; and human-authored metadata |Do not add human-authored data and remove operational video and camera data|
|Telecommunications metadata|Information on the times, origins and destinations of phone calls, electronic messages, instant messages and other modes of telecommunication| |
|Digital photo metadata |Metadata may be written into a digital photo file that will identify who owns it, copyright and contact information, what brand or model of camera created the file, along with exposure information (shutter speed, f-stop, etc.) and descriptive information, such as keywords about the photo, making the file or image searchable on a computer and/or the Internet.|Do not add human-authored data and remove operational photo and image data|
|Document metadata |Metadata may be written into documents that will identify who owns it, copyright and contact information, and descriptive information, such as keywords, making the file searchable on a computer and/or the Internet.|Do not add human-authored data and remove operational document data|
|username(s)|A user often has a user account and is identified to a system by a username, login name, screen name, nickname, nick or handle |Regularly change user names; have a few pseudonyms (that you only use on separate (virtual) machines)|
|Digital identity|[[https://www.digitalidentityguide.com/what-is-a-digital-identity/|Digital identity]] based on dynamic entity relationships captured from behavioural history across multiple websites and mobile apps can verify and authenticate an identity with up to 95 percent accuracy|Use tunnelling (VPN or SSH) or Tor and when doing so never ever post any personal data.|
