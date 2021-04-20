---
title: "Powering the digital (2017)"
modified: 2017-12-19T13:54:00+00:00
categories:
  - Elephants
tags:
  - Causes and effects
  - Elephants
  - Blindspot
  - Consumerism
---

Environmental and climate change concerns have led to energy-efficient networking research. To gain some insights into whether this makes sense and what we can possibly do, I have used the method from [The Energy and Emergy of the Internet by Barath Raghavan and Justin Ma](https://www.icsi.berkeley.edu/pubs/networking/energyandemergy11.pdf). The Internet architecture makes assessing its components hard to do. The problem is compounded by new developments in the Internet architecture, mostly to do with functional off-loading, for example of mobile traffic to Wi-Fi, femtocell and Integrated Mobile Broadcast and video traffic via the development of CDN's.

Raghavan and Ma's tables have been adapted for the new developments and updated with (inferred) [data from Internet sites](#resources). Though crude, this suffices for gaining insight from asking more questions in a global context. For estimates regarding worldwide energy and electricity consumption, IEA reports were used and the significant data visualised.

- [How much energy and electricity is consumed worldwide in total?](#how-much-energy-and-electricity-is-consumed-worldwide-in-total)
- [How much energy is required to construct, and run and maintain the internet?](#how-much-energy-is-required-to-construct-and-run-and-maintain-the-internet)
  - [Constructing the internet](#constructing-the-internet)
  - [Running the internet](#running-the-internet)
  - [Maintaining the internet](#maintaining-the-internet)
  - [Energy required to maintain and run the Internet](#energy-required-to-maintain-and-run-the-internet)
- [Resources](#resources)
  - [Emergy](#emergy)
  - [Internet statistics](#internet-statistics)
  - [Cloud and data centers](#cloud-and-data-centers)
  - [Routers](#routers)
  - [Cables](#cables)
  - [Smart city](#smart-city)
  - [Energy](#energy)

## How much energy and electricity is consumed worldwide in total?

![Made with gnuplot]({{ site.url }}{{ site.baseurl }}/assets/images/wec.png)

|Year |Primary energy supply (TPES) (in Mtoe and TWh) |Final energy consumption (in TWh) |Electricity generation |Total amount of electricity consumed |Reports (retrieved from) |
| --- | :-- | :-- | :-- | :-- | --- |
|1973 |6.106 (Mtoe) 71.013 (TWh)|4.672 (Mtoe) 54.335 (TWh)|6.129 (TWh)|5.107 (TWh)| All IEA reports |
|1990 |102.569 (TWh)| -      |11.821 (TWh)| - | - |
|2000 |117.687 (TWh)| -      |15.395 (TWh)|12.116 (TWh)| - |
|2009 |12.150 (Mtoe) 141.304 (TWh)|8.353 (Mtoe) 97.145 (TWh)| 20.055 (TWh)|16.806 (TWh)|Stanford|
|2010 |12.717 (Mtoe) 147.899 (TWh)|8.677 (Mtoe) 100.914 (TWh)|21.431 (TWh)|17.861 (TWh)|IEA |
|2011 |13.113 (Mtoe) 152.504 (TWh)|8.918 (Mtoe) 103.716 (TWh)|22.126 (TWh)|18.358 (TWh)|IEA |
|2012 |13.371 (Mtoe) 155.505 (TWh)|8.979 (Mtoe) 104.426 (TWh)|22.668 (TWh)|18.608 (TWh)|webcitation |
|2013 |13.541 (Mtoe) 157.482 (TWh)|9.301 (Mtoe) 108.171 (TWh)|23.322 (TWh)|19.504 (TWh)|webcitation |
|2014 |13.369 (Mtoe) 155.481 (TWh)|9.425 (Mtoe) 109.613 (TWh)|23.816 (TWh)|19.840 (TWh)|webcitation |
|2015 |13.647 (Mtoe) 168.519 (TWh)|9.384 (Mtoe) 109.136 (TWh)|24.255 (TWh)|20.190 (TWh)|ucse.edu|
|2016 | - | -      | -     | - | cap|
|2017 | - | -      | -     | - | IEA|

* There is a delay in the reporting of two years. For example, for the data of 2010, look in the 2012 report.
* Mtoe = Million Tons of Oil Equivalent, a somewhat artificial energy unit - given that the energy content of grades of oil vary considerably depending on their source - that pretends that all the world’s energy comes from a standardized form of the dangerous fossil fuel petroleum, which, of course, is not true. 
* World total primary energy supply (TPES), or "primary energy" differs from the world final energy consumption because much of the energy that is acquired by humans is lost as other forms of energy during the process of its refinement into usable forms of energy and its transport from its initial place of supply to consumers.
* The Total amount of electricity consumed figure is smaller than the generated electricity due to grid losses, storage losses, and self-consumption from power plants.
* From the *not-quite-there-services-while-paid-for-with-our-tax-money* dept.: The IEA only makes reports of the current year available, OECD does have the previous files in its library but requires payment, so I have had to retrieve those from various other sources.
* The rise in final energy consumption worldwide, shows that energy conservation as an energy strategy is not working.
* The worldwide energy consumption averages say nothing of the distribution of energy. On some level energy is wealth, and wealth is ever more disproportionately distributed. Great Tesla car you got there!
* There are billions on this planet who live in energy poverty, and have to live with the consequences of the extractions made for and emissions made by the energy rich. Ah, and cannot afford a doctor either.
* Neodymium and aluminium are two examples of metals that require significant quantities of energy in its extraction:  Our false life industrial culture relies on the separation and refining of significant quantities of some sixty to seventy elements from their sources, be they rocks, gases, or liquids; all of these processes of separation of metals from ores and refining require energy. 

## How much energy is required to construct, and run and maintain the internet?

To answer this question, a non-exhaustive list of weighted components was used and because there is no single authoritative authority, the following are informed estimates and inferred guesstimates that will be updated and improved over time as new data emerges.

### Constructing the internet

|Device |Estimated amount |Unit emergy |Total potential emergy |Weight ||Estimated Internet emergy ||
| --- | :-- | :-- | :-- | :-- | --- |:-- | :-- | 
|                  |                 |            |             |Minimum |Maximum |Minumum |Maximum|
|Desktops          |  1.000.000.000|  7.5 GJ|  7500E+6 GJ|  0.5  |  0.95  |  3750E+6 GJ|  7125E+6 GJ|
|Laptops           |  1.000.000.000|  4.5 GJ|  4500E+6 GJ|  0.75  |  1.0  |  3375E+6 GJ|  4500E+6 GJ|
|Smartphones and mobile phones |  4.000.000.000|  1 GJ|  4000E+6 GJ|  0.25  |  0.9  |  1000E+6 GJ|  3600E+6 GJ|
|Cloud servers  |  150,000,000|  5 GJ|  7500E+6 GJ|  0.8  |  1.0  |  6000E+6 GJ|  7500E+6 GJ|
|Servers |  50.000.000|  5 GJ|  2500E+6 GJ|  0.5  |  0.95  |  1250E+6 GJ|  2375E+6 GJ|
|Core and edge routers|  2,000,000|  50 GJ|  100E+6 GJ|  0.9  |  1.0  |  90E+6 GJ|  100E+6 GJ|
|WiFi/LAN routers |  200,000,000|  1 GJ|  200E+6 GJ|  0.75  |  1.0  |  150E+6 GJ|  200E+6 GJ|
|Cell towers |  6,000,000|  100 GJ|  600E+6 GJ|  0.1  |  0.5  |  6E+6 GJ|  300E+6 GJ|
|Telecom switches  |  100,000|  1000 GJ|  100E+6 GJ|  0  |  0.25  |  0|  25E+6 GJ|
|Fiber optics      |  3,000,000,000 km|  10 GJ|  3.000E+6 GJ|  0.5  |  0.9  |  1500E+6 GJ|  2700E+6 GJ|
|Copper            |  6,000,000,000 km|  10 GJ|  6.000E+6 GJ|  0.1  |  0.5  |  600E+6 GJ|  3000E+6 GJ| 
|                  |                  |       |             |    **Totals**||  17721E+6 GJ|  31425E+6 GJ|

Notes:
* Weight is a factor for determining how much a device participates in the internet
* In 2017, more than half of the world’s population used a smartphone; Almost two-thirds had a mobile phone; More than half of the world’s web traffic came from mobile phones.
* Cloud servers embodied in high powered rack-mounted devices in big server farms from corporations such as AWS, Oracle, Microsoft, Google, Range International Information Group, Switch SuperNAP, DuPont Fabros Technology, etc.
* Servers here are not user facing and not in the cloud.
* WiFi/LAN routers includes cable modems, hubs, small switches, WiFi access points.
* Cell towers does not include femtocell.
* Telecom switches includes satellites and has been extrapolated to global use.

### Running the internet

|Device |Estimated amount |Unit electricity |Duty cycle |Total electricity |Weight ||Estimated Internet electricity|| 
| --- | :-- | :-- | :-- | :-- | :-- |:-- | :-- | :-- |
|                  |       ||          |      |    |Minimum |Maximum |Minumum |Maximum|
|Desktops          |  1.000.000.000|  150 W|  0.5  |  75 GW|  0.5  |  0.95  |  38 GW|  71 GW|
|Laptops           |  1.000.000.000|  40 W|  0.5  |  20 GW|  0.75  |  1.0  |  15 GW|  20 GW|
|Smartphones and mobile phones |  4.000.000.000|  1 W|  0.5  |  2 GW|  0.25  |  0.9  |  1 GW|  2 GW|
|Cloud servers |  150.000.000|  450 W|  1  |  67.5 GW|  0.8  |  1.0  |  54 GW|  68 GW|
|Servers |  50.000.000|  375 W|  1  |  18.75 GW|  0.5  |  0.95  |  9 GW|  18 GW|
|Core and edge routers|  2.000.000|  5000 W|  1  |  10 GW|  0.9  |  1.0  |  9 GW|  10 GW|
|WiFi/LAN routers |  200.000.000|  20 W|  1  |  4 GW|  0.75  |  1.0  |  3 GW|  4 GW|
|Cell towers |  6.000.000|  3000 W|  1  |  18 GW|  0.1  |  0.5  |  2 GW|  9 GW|
|Telecom switches  |  100,000|  75 GW|  1  |  7.5 GW|  0  |  0.25  |  0|  2 GW|
|Fiber optics      |  3.000.000.000 km|  0|  0  |  0|  0.5  |  0.9  |  0|  0|
|Copper            |  6.000.000.000 km|  0|  0  |  0|  0.1  |  0.5  |  0|  0| 
|                  |                  |       |        |   |   |    **Totals**|  131 GW|  204 GW|

### Maintaining the internet

To answer the question “How much energy is required to maintain the internet?”, data from constructing the internet is used with replacement timespan estimates. 

|Device 	|Estimated Internet emergy||  Replacement timespan  ||  Embodied power ||
| --- | :-- | :-- | :-- | :-- | :-- |:-- |  
|      |Minumum 	|Maximum|  Years  |  Seconds  |Minimum  |Maximum  |
|Desktops |  3750E+6 GJ|  7125E+6 GJ|  4  |  1.26E+08  |  30 GW|  57 GW|
|Laptops |  3375E+6 GJ|  4500E+6 GJ|  3  |  9.47E+07  |  36 GW|  48 GW|
|Smartphones and mobile phones |  1000E+6 GJ|  3600E+6 GJ|  2  |  6.31E+07  |  16 GW|  57 GW|
|Cloud servers |  6000E+6 GJ|  7500E+6 GJ|  3  |  9.47E+07  |  63 GW|  79 GW|
|Servers |  1250E+6 GJ|  2375E+6 GJ|  3  |  9.47E+07  |  13 GW|  25 GW|
|Core and edge routers |  90E+6 GJ|  100E+6 GJ|  3  |  9.47E+07  |  1 GW|  1 GW|
|WiFi/LAN routers |  150E+6 GJ|  200E+6 GJ|  3  |  9.47E+07  |  2 GW|   2 GW|
|Cell towers |  6E+6 GJ|  300E+6 GJ|  10  |  3.16E+08  |  ~ 0 GW|  1 GW|
|Telecom switches |  0|  25E+6 GJ|  10  |  3.16E+08  |  0|  ~ 0 GW|
|Fiber optics |  1500E+6 GJ|  2700E+6 GJ|  10  |  3.16E+08  |  5 GW|  8 GW|
|Copper |  600E+6 GJ|  3000E+6 GJ|  30  |  9.47E+08  |  1 GW|   10 GW|
|  |  |  |  |  Totals|  167 GW|  288 GW|

Notes:

* Embodied power: The power P in watts (W) is equal to the energy E in joules (J), divided by the time period t in (seconds)

### Energy required to maintain and run the Internet

The minimum total power that was required to run (wall socket power) and maintain (embody) the internet in 2017 was guesstimated to be somewhere between ~131 GW + ~167 GW = ~298 GW and ~204 GW + ~288 GW = ~492 GW.

## Resources

### Emergy

* [On the materials basis of modern society, T. E. Graedel, E. M. Harper, N. T. Nassar, and Barbara K. Reck, 2013](https://www.pnas.org/content/112/20/6295)
* [The Energy and Emergy of the Internet (pdf), Barath Raghavan and Justin Ma, 2011](https://www.icsi.berkeley.edu/pubs/networking/energyandemergy11.pdf)
* [Networking in the Long Emergency, Barath Raghavan and Justin Ma, 2011](https://www.icsi.berkeley.edu/pubs/networking/networkinglongemergency11.pdf)
* [Supporting information for – Energy intensity of computer manufacturing: hybrid assessment combining process and economic input-output methods, AACM, 2004](https://pubs.acs.org/doi/suppl/10.1021/es035152j/suppl_file/es035152jsi20040820_075507.pdf)

### Internet statistics

*  [Internet live stats](http://www.internetlivestats.com/)
*  [Internet world stats](https://www.internetworldstats.com/stats.htm)
*  [Cisco Annual Internet Report (2018-2023)](https://www.cisco.com/c/en/us/solutions/collateral/executive-perspectives/annual-internet-report/white-paper-c11-741490.html)

### Cloud and data centers

* [How dirty is your data? A Look at the Energy Choices That Power Cloud Computing (pdf), Greenpeace, 2014](https://wayback.archive-it.org/9650/20200406044849/http://p3-raw.greenpeace.org/international/Global/international/publications/climate/2011/Cool%20IT/dirty-data-report-greenpeace.pdf)
* [Estimating total power consumption by servers in the US and the world (pdf), Jonathan G. Koomey, AMD, 2007](https://www.researchgate.net/publication/228365136_Estimating_Total_Power_Consumption_by_Servers_in_the_US_and_the_World)

### Routers

* [The Energy Intensity of the Internet: Edge and Core Networks, D. Schien, V.C. Coroama, L.M. Hilty, and C. Preist, 2014](http://publicationslist.org/data/lorenz.hilty/ref-230/2014_Schien_Coroama_Hilty_Preist_Energy_Intensity_Internet_Edge_Core.pdf)
* [Measuring the Degree Distribution of Routers in the Core Internet, Matthieu Latapy, Elie Rotenberg, Christophe Crespelle, Fabien Tarissan, 2014](https://hal.archives-ouvertes.fr/hal-01208359/document)

### Cables

* [Submarine Cable Map](https://www.submarinecablemap.com/)
* [This map shows the explosive growth of underwater cables that power the global internet, Christopher Groskopf, October, 2016](https://qz.com/657898/this-map-shows-the-explosive-growth-of-underwater-cables-the-power-the-global-internet/)
* [The internet has been quietly rewired, and video is the reason why, Joon Ian Wong, October 2016](https://qz.com/742474/how-streaming-video-changed-the-shape-of-the-internet/)
* [FOA](https://www.thefoa.org/)

### Smart city

* [5G small cell forum](https://www.smallcellforum.org/)

### Energy

* [Current World Energy Demand, Ethical World Energy Demand, Depleted Uranium and the Centuries to Come (pdf), Nadir, 2014](https://bravenewclimate.files.wordpress.com/2014/12/nnadir_worldenergy.pdf)
