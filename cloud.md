4.2 Cloud Services
Truelec currently operates all core systems (HR, CRM, File Storage, and Accounting) on on-premises Dell PowerEdge tower servers located at its Melbourne headquarters.
As part of its digital transformation, the company is evaluating migration to cloud-based virtual machines (VMs) to improve scalability, uptime, and disaster recovery readiness.
This task compares two leading cloud providers – Amazon Web Services (AWS) and Microsoft Azure – using each vendor’s official pricing calculator to estimate the cost of hosting equivalent virtual machines for the next five years.

Cloud Server Specifications
The selected configuration matches a mid-tier Dell PowerEdge T40 used at HQ for application hosting and file sharing.
Component	Specification
vCPU	4 virtual CPUs
RAM	16 GB
Storage	512 GB SSD
Operating System	Windows Server 2022 Datacenter
Region	Australia East (Sydney)
Availability	99.9% SLA uptime
Backup	Daily snapshot, 7-day retention
All parameters (CPU, RAM, OS, region) are kept identical across providers to ensure fair cost comparison.

Cloud Cost Comparison
Provider	Region	vCPU	RAM	Storage	OS	Monthly Cost (AUD)	5-Year Cost (AUD)
Amazon AWS (EC2 – t3.xlarge)	ap-southeast-2 (Sydney)	4	16 GB	512 GB SSD	Windows Server 2022	$185	$11,100
Microsoft Azure (D4as v5)	Australia East (Sydney)	4	16 GB	512 GB SSD	Windows Server 2022	$175	$10,500
On-Prem Dell PowerEdge T40	HQ (Physical Server)	4 Cores	16 GB	512 GB SSD	Windows Server 2022	One-time cost: $2,500 + 10% annual maintenance (~$250)	$3,750 (5 years)

Cost Analysis
•	On-Prem Server (Dell T40): Lowest total cost (~$3.75K) but requires physical maintenance, electricity, cooling, and lacks redundancy.
•	Azure: Slightly cheaper than AWS overall (~$10.5K vs. $11.1K), with integrated compliance features and easier AD/Office365 integration for Truelec’s Windows environment.
•	AWS: More globally scalable, with flexible instance types and automated backup services, but slightly higher cost in Sydney region.

5-Year Cost Summary
Option	Total 5-Year Cost (AUD)	Relative Cost
On-Prem	$3,750	🔻 Lowest
Azure	$10,500	💲💲
AWS	$11,100	💲💲💲

 Although on-prem is cheaper short-term, it lacks disaster recovery, auto-scaling, and global uptime guarantees that cloud solutions provide.

Recommendation
After evaluating cost, compatibility, and reliability:
Microsoft Azure is recommended for Truelec’s migration.
Reasons:
•	Seamless integration with Microsoft 365 and Active Directory.
•	Slightly lower pricing than AWS in the Sydney region.
•	Built-in compliance tools supporting ISO 27001 and Australian Privacy Principles.
•	Simple portal-based backup and monitoring for SMEs.
Azure balances cost and reliability for a Windows-based SME like Truelec.

Pros and Cons of Cloud Adoption
Aspect	Advantages	Disadvantages
Scalability	Quickly scale up/down resources during project peaks.	May overpay if resources are left idle.
Maintenance	No physical maintenance or power requirements.	Relies entirely on vendor infrastructure.
Disaster Recovery	Built-in redundancy and offsite backups.	Recovery depends on internet availability.
Cost	Predictable monthly billing (OpEx).	Higher total cost than on-prem after 5 years.
Accessibility	Staff can access CRM/HR remotely via VPN or web.	Security risk if remote access is misconfigured.
Compliance	Azure & AWS meet ISO 27001, SOC2, and APP standards.	Data stored in Sydney — potential sovereignty concerns.

Summary
•	Both AWS and Azure provide robust options for Truelec’s workload.
•	Azure is recommended due to:
o	Best cost-to-performance ratio.
o	Native Windows ecosystem integration.
o	Local Sydney data centre (low latency).
•	Migration can start with hybrid approach — keeping critical servers on-prem while gradually moving CRM and HR to cloud.

