Description of the project

Acquisition of Solar Canada (SC) by Solar America (SA) to form North American Corporation. (NAC)
Goal: Increase sales across North America by consolidating operations
Merger involves merging IT operations using Software Defined Network (SDN) technology
Proposed design includes modular and standardized solutions for head offices, regional offices, and data centers
Emphasis on redundancy and scalability in design
SDN controller chosen for Dallas headquarters to streamline operations and preserve existing infrastructure
Private clouds deployed in Canada and the United States; public cloud in Dallas serves both countries
SD-WAN facilitates connectivity between regional offices and Dallas headquarters
Cisco switches replace standard routers for improved manageability and performance
SolarWinds used for network management, optimization, monitoring, and reporting
Integrated network architecture aims to unify SC and SA networks under NAC
Expected benefits: Cost savings, operational efficiency, expanded market presence across North America.


Design Criteria:

• Recommended a new Head Office network module in Dallas, copied from the original Toronto
Head Office design.
• Selected and designed a Software Defined Network system for the NAC network. design
should not change any existing applications, LAN/WAN functionality, Cloud utility or
management systems.  detail the plan and its expected benefits. Be
sure to indicate which SDN type you have chosen and if applicable, which brand/protocol you
will be using.
• Designed an effective Regional Office module for the Regional Offices in:
• Dallas (HO & collapsed Southern Region)
• San Francisco (Western Region)
• Chicago (Central Region)
• Boston (Eastern Region)
• Toronto (Northern Region) – Covers all of Canada because of the currency and taxes
difference.
• Created a new Private Cloud in Dallas DC to service a Sales access interface for the US
Agents. This private cloud is residing on internal infrastructure and separate from the Canadian
private cloud.
• Created a Public Cloud, also in Dallas DC for the Sales NAC services. The public cloud must
be accessible form both Canada and the US. Document storage will be specific to Canada and
the US. 
NOTE: Consider the compliance requirements for each country when determining
where the public cloud is located.
• Design new network SD-WAN links as follows:
• Regional Offices to Head Office
• Mirror the Dallas Data Center operations to the Markham SDN based back-up DC.
• Tunnel layer from each regional office to Markham so it becomes an active fail-over DC.
• Perform Data Hiding at the edge of Regional Failure Domains to isolate Northern Traffic.


Design

Regional Office

![image](https://github.com/mysteriousuh/SDWAN-Configurer/assets/30888240/9ca9f613-dd68-4b52-ab35-299d09570a62)

Markham DATA CENTRE

![image](https://github.com/mysteriousuh/SDWAN-Configurer/assets/30888240/780c1306-4eed-4529-a599-07310f7d9341)

TORONTO REGIONAL OFFICE
![image](https://github.com/mysteriousuh/SDWAN-Configurer/assets/30888240/5fcdfbd3-67c3-4625-8496-c822f18f3d91)



DALLAS HEAD OFFICE

![image](https://github.com/mysteriousuh/SDWAN-Configurer/assets/30888240/2f3cf7ff-3c97-4908-b943-6f946ec8122e)

NAC NETWORK

![image](https://github.com/mysteriousuh/SDWAN-Configurer/assets/30888240/ebf2a73d-f7fe-4c4e-a769-23bb6b3087d1)

