---
title: "Internet (in)security"
modified: 2021-04-22T21:44:00+00:00
categories:
  - Scenario-planning
tags:
  - Causes and effects
  - Elephants
  - Security
  - Internet
  - Trends
---
_"Gotta feel kind of bad for nation-state hackers who spend years implanting and cultivating some hardware exploit, only to discover the entire target database is already exposed to anyone with a web browser."_

[![Stack]({{ site.url }}{{ site.baseurl }}/assets/images/stack.png#center)](https://www.xkcd.com/2166/)

* Most [E2EE systems](https://github.com/tymyrddin/orchard/blob/main/threat-modelling/E2EE-threat-model/README.md) are secure against only the weakest passive adversaries, breakable not by cryptanalysis of underlying cryptographic algorithms but by flawed system designs and security assumptions. Unencrypted metadata and access patterns make these systems susceptible to inference attacks. And recently made laws seem to have been made to prepare the way for agencies to legitimately gather encrypted data via backdoors and ghost protocols.
* The [MitM server-to-server HTTPS communication](https://github.com/tymyrddin/orchard/blob/main/resources/vulnerabilities/endpoints/Server.md) attack for example, is not about a vulnerability, it is about a flawed concept. The abstraction of trusted Internet routing is wrong. DNSsec and IPsec routing were developed as stopgaps, but make packet flow harder to troubleshoot and add excessive administrative overhead.
* Hackers increasingly use [search engine poisoning](https://github.com/tymyrddin/orchard/blob/main/threat-modelling/SE-threat-model/attacks/Search-engine-poisoning.md) attacks because they are so easy to do, and several automated tool-kits are readily available to make it even easier.
* [Credential stuffing](https://github.com/tymyrddin/orchard/blob/main/trees/social-engineering/Credential-stuffing.md) is currently one of the most common techniques used to take-over user accounts. Credential spilling is when credentials gained from data breaches are sold to other adversaries. Credential stuffing is the large scale use of automated means to test stolen passwords against other unrelated websites. This is a possible and often successful attack because of the tendency for users to recycle their passwords for multiple accounts.
* Polymorphic malware created by machines are likely to develop (further). These learn to evade detection based on automated vulnerability detection and complex data analysis.
* [DDoS](https://github.com/tymyrddin/orchard/blob/main/trees/network-attacks/Distributed-Denial-of-Service-(DDoS).md) and [DrDoS](https://github.com/tymyrddin/orchard/blob/main/trees/network-attacks/Distributed-Deflection-Denial-of-Service-(DrDoS).md) attacks employ swarms of these vulnerable endpoints to attack public infrastructure through massively coordinated communication channels. Smarter control software exists but is costly, and certainly not available to consumer-grade endpoints. Think unpredictable spikes in infrastructure use and availability issues.
* Meanwhile, such [poorly-protected vulnerable endpoints](https://github.com/tymyrddin/orchard/tree/main/resources/vulnerabilities/endpoints) are ubiquitous and provide starting points for further structured attacks.
* And there is more to come. Mobile devices and connected sensors such as smart home devices, biochip transponders on farm animals and electric clams in coastal waters, you name it, the monitoring craze is everywhere, increasing the attack surface.

