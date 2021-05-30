---
title: "Creating spaces"
modified: 2021-04-23T00:02:00+00:00
categories:
  - Scenario-planning
tags:
  - Causes and effects
  - Elephants
  - Scenario logics
  - Trends
---
 _“This is space. It's sometimes called the final frontier (Except that of course you can't have a final frontier, because there'd be nothing for it to be a frontier to, but as frontiers go, it's pretty penultimate . . .)”_ ~ Terry Pratchett, Moving Pictures 

![Problem spaces]({{ site.url }}{{ site.baseurl }}/assets/images/distinctions.png#center)

Rather tricky these distinctions, as they are not mutually exclusive depending on context and level of abstraction. For example, a heterarchical system can contain hierarchies and each level in a hierarchical system can be composed of potentially heterarchical groups. For the sake of the sense of the distinctions made here, DNS can be seen as a decentralised, hierarchical system and Facebook's OpenGraph as a centralised, heterarchical system.

* Components can be pigeon-holed as co-located vs distributed (physically or logically).
* Components can be designed to be under the control of a single entity vs multiple entities (logical or abstract able to coordinate nodes in the system).
* Components can be considered heterarchical (unranked or having the potential to be ranked a number of different ways) vs hierarchical (ranked).

Hierarchical structures tend to resemble pyramids, with the highest levels of power and authority at the very top and are known causes of loss of resilience and unequal socialisation. What problems can distributed solutions solve? And which not? In which contexts and for what do distributed solutions make sense? 

## Internet frontier

The internet is heterarchical in its overall design, and hierarchical in its details. Communication is distributed, but content is not. The internet suffers from canonical/authority issues due to economic and structural incentives that have made/evolved it that way.

* When connecting to an Internet Service Provider (ISP), the device connecting becomes part of that ISP network. The ISP may then connect to a larger network and become part of their network. Large ISPs run dedicated backbones connecting various regions and there are several high-level networks connecting to each other through Network Access Points (NAPs). Dozens of large Internet providers interconnect at NAPs in various cities, and trillions of bytes of data flow between the individual networks at these points. A collection of huge corporate networks that agree to intercommunicate with each other at the NAPs. With more and more devices connecting and no net neutrality, leading to [connectivity bottlenecks]({{ site.url }}{{ site.baseurl }}/scenario-planning/internet-bottlenecks).
* The internet requires agency in multiple forms (DNS, serving content from centralised servers on some port, ISO/OSI stack, hierarchical internetworking model, etc.)
    * The DNS hierarchy consists of root level, top level domains, second level domains, sub-domains, and hosts, in that order.
* ["Consumer" computers are grazed for information]({{ site.url }}{{ site.baseurl }}/scenario-planning/panopticon) about its users by the “predators” in the hierarchy.
* The internet does not have built-in mechanisms to promote redundancy for durability, availability, or performance purposes. One daemon serves one copy. Everything else (CDNs, forward/reverse proxies, failover) is some kind of optimisation tacked on afterwards.
* Users have to depend on hosts providing [secure access]({{ site.url }}{{ site.baseurl }}/scenario-planning/internet-insecurity-trends), which for providers has often been an afterthought if thought of at all, in an environment that can not be secured from attacks on the routing level like [BGP hijacking](https://github.com/tymyrddin/orchard/blob/main/trees/network-attacks/Hijack-BGP.md) because trust is a flawed concept.


