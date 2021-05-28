---
title: "Internet bottlenecks"
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
There is an accelerating growth of connection requests from mobile devices and IoT devices. What to expect if this continues?

## Connectivity

* Driven by a desire for our data, corporations will likely bundle connectivity into products whether people want it or not. Devices without IoT capabilities may even become more expensive because they will lack the data that can be harvested by manufacturers.
* A growing number of cross border attacks, economic protectionism, regulatory divergence and loss of government power to global online companies, will likely push governments towards breaking up the internet in cages.
* A large amount of the data will be stored in clouds, which will become the principle targets. The complex, hyperconnected networks of cloud providers looks to me like a potential single point of failure for hundreds of businesses, government entities, critical infrastructures, and all kinds of organisations, including healthcare.
* The pace of change seems to have exceeded the rate of human capability to absorb and adapt, while billions of devices add their demands on our rapidly dwindling connectivity, and lack of sufficient security becomes an ever bigger problem.
* Today’s web-based applications tend to push user-interaction work — accompanied by lots of data — to the client workstation. The code on the client then processes large amounts of data, which can cause multi-second pauses before the client display updates. Or, the host has a bottleneck.

## Internet-facing applications

Most applications are of the form of some front-end web server talking with an application server that is talking with a middleware server that queries one or more database servers. And all of those servers all might talk with DNS servers to look up IP addresses or map them back to server names. And the whole can be slow. Using packet capture tools to discover whether the network or application is to blame could take many, many hours of work.

* The applications or servers themselves may be slow.
* Applications are often developed in a fast network context with a small data set. In that context the application runs smoothly and fast. In production perhaps maybe not so. And as the database continues to grow, so does downtime.
    * A middleware server may be making too many requests to a database server (a single client request can cause many database requests or the transfer of a large volume of data.)
    * A database server may take several seconds to return data for a specific query.
* An application server or perhaps a client may make many small requests to execute a transaction.
* Automatic migration of a server image to a lightly loaded host can put it several milliseconds further away from the other servers or from its disk storage system. And it stacks.
* Slow network services can slow applications.
* Slow network.

