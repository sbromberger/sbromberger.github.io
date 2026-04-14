---
title: Seth Bromberger
layout: default
---
## Projects & Research

<br/>

### Julia - A Fresh Approach To Numerical Computing
{: #julia}
[Julia](http://julialang.org) is a relatively new programming language focused on technical and scientific computing. I have been modeling AMI mesh networks using an <a href="https://github.com/sbromberger/LightGraphs.jl"> optimized graph representation</a> that I developed along with the necessary algorithms to perform simulations of various responses to network events.
[LightGraphs.jl](https://github.com/sbromberger/LightGraphs.jl) has been designed to scale to millions of vertices with hundreds of millions of edges on standard computing hardware, making accurate representation of modern AMI networks feasible.

I am the author of a [memory-efficient representation of IPv4 and IPv6 networks](https://github.com/JuliaWeb/IPNets.jl) which is also used for this modeling and simulation activity and am a member of the [JuliaWeb](https://github.com/JuliaWeb) and [JuliaGraphs](https://github.com/JuliaGraphs) organizations.

<br/>

### NetCanary™: Breaking the Kill Chain
{: #netcanary}
In 2008, I attended the [Idaho National Laboratory](https://www.inl.gov) Red / Blue Team cyber exercise. During a week of intense education and collaboration, I was part of a team defending a representative ICS network against mock attackers. As part of the defense strategy, I used some [open source tools](http://www.honeyd.org) in an ultimately-successful attempt to keep the bad guys at bay (see [“The SCADA HoneyNet Project”]("#honeynet") below for more details). The foundations of NetCanary™ were built during this exercise and were eventually turned into a workable product in late 2013 / early 2014.

NetCanary™ is designed to detect malicious activity as early in the [Cyber Kill Chain®](https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html) as possible, giving security teams the information they need to stop attacks during reconnaissance, before they happen. The system has been tested in production enterprise networks and in ICS environments, and has been designed to be safe, responsive, and easy to manage.

<br/>

### Industrial Control Systems / Advanced Metering Infrastructure / Smart Grid Security Research
{: #icsami}
I have spent the last several years researching the security implications of Industrial Control, AMI, and Smart Grid systems. While most AMI / Smart Grid technologies reference secure design principles, the implementation often deviates — sometimes significantly — from the reference models and standards. This leads to security and operational problems of varying severity. It is not enough that standards exist; they must be followed to the letter in order to ensure that the security and operational benefits that flow from such standardization accrue to the specific implementation.

In 2012, I was listed in [*Smart Grid Today* magazine](https://www.smartgridtoday.com) as one of its Smart Grid Pioneers.

I continue to study the use of [existing security technologies](/files/pki_whitepaper_1.4.pdf) within these new environments, and to [report](https://www.energy.gov/sites/prod/files/oeprod/DocumentsandMedia/DNS_Exfiltration_2011-01-01_v1.1.pdf) on [deficiencies](https://www.cisa.gov/news-events/ics-advisories/icsa-12-348-01), and provide mitigation suggestions, where appropriate.

<br/>

### Multi-Source Data Correlation and Analysis
{: #correlation}
The rise of “big data” — the accumulation and storage of large, non-normalized datasets — has prompted research into the best way to analyze the massive amounts of data now being compiled by organizations. Unlike traditional structured data analysis, analysis of disparate data sources that have been combined into large data stores requires a new approach to turn the data into useful information and then into knowledge. I have developed unique methods for performing multi-source correlation among large data sets in utility networks for the purposes of extracting actionable information regarding customer behavior and operational stability of AMI and Smart Grid components. These methods have been incorporated into the TopSight™ event correlation system (described below). My continuing research in this field focuses on properties of the associated “metadata” and the applicability of this derivative data to core event analysis functions via its use in unstructured machine learning processes.

<br/>

### TopSight™
{: #topsight}
In 2009, as Smart Meters were being deployed across the country, it became evident that the traditional methods of detecting anomalous behavior within data networks were inadequate to meet the specific technology limitations inherent in Smart Meter networks. Bandwidth, design, and processing constraints within these new networks required a different approach to event analysis, and a system that could provide rapid correlation from massive amounts of data — data obtained from multiple data stores and with varying degrees of reliability and availability — would be needed if any detection system were going to be successful.

From 2009–10, I proposed, obtained funding for, designed, and implemented a system called TopSight™ to provide a method for rapid analysis of Smart Meter system and network events. The system was implemented within six months of the start of the project and enjoyed rapid development of enhancements. A provisional patent was filed for the system in early 2011, and the non-provisional patent was submitted to the US Patent and Trademark Office later that year. I am the sole inventor listed on [filing number 13,339,509](/files/patent_20120232915.pdf), which describes a “System And Method For Monitoring a Utility Meter Network”.

<br/>

### The HoneyMeter™ Project
{: #honeymeter}
HoneyMeters are devices — similar to [honeypots](http://en.wikipedia.org/wiki/Honeypot_(computing)) — designed to detect and log unauthorized access within a Smart Meter / AMI environment. As one of the inputs to the TopSight™ system, the HoneyMeter™ was developed for deployment throughout a utility's AMI network and provided capture and alerting whenever unauthorized traffic was detected to the device. I designed and built a prototype, using both custom and off-the-shelf hardware and software components, and submitted it for field testing.

<br/>

### Quantitative Threat Management
{: #qtm}
The Quantitative Threat Management (QTM) project has its roots in the NSA's Infosec Assurance Capability Maturity Model (IA-CMM) effort. This capability maturity model evaluated an organization's security posture across nine process areas. Process area 4 dealt with the assessment of threats to an organization.

At [PG&amp;E](http://www.pge.com), I led my group in an effort to develop information security capabilities that could be evaluated against the IA-CMM. We used the reference materials to enhance existing capabilities and to develop new ones. When it came to threat analysis, there seemed to be no good quantitative models from which to choose — most of the models dealt with subjective criteria and were therefore not reliably repeatable. I developed the QTM in response to this gap.

There are a couple of articles describing the QTM methodology at a high level, and I am happy to provide a more detailed presentation upon request. Please [contact me](mailto:info@bromberger.com?subject="QTM") to schedule.

<br/>

### The SCADA HoneyNet Project
{: #honeynet}
Many people — including some experts in the field — perceive SCADA networks as fragile and easily subject to disruption. This perceived fragility is often used as an excuse to delay or deny implementation of hardware and software components that do not directly serve to manage control systems on these networks.

In 2008, I had an opportunity to attend the Advanced SCADA Security Training at [Idaho National Laboratory](https://www.inl.gov). Part of the highly recommended course involved penetration testing on a mock control systems network (while the equipment on the network was real, it was not controlling production processes). I took the opportunity in the weeks before the training to design and develop a defensive tool for use in the test. The result was the SCADA HoneyNet, which was a combination of open-source tools ([HoneyD](http://www.honeyd.org) and farpd on a standard [Ubuntu Linux](http://www.ubuntu.com) build) designed to mimic control systems for the purposes of deterring and delaying attacks on SCADA networks. I deployed the SCADA HoneyNet during the training exercise with great success: the system successfully detected and thwarted all attacks against the legitimate control systems, and did not interfere with the intended operation of the devices on the network. No production disruption of the control network occurred as a result of the deployment or operation of the SCADA HoneyNet.

A paper describing the setup and results is available [here](/files/honeypots%20and%20control%20systems.pdf).
