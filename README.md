# Incident Response Playbook 
## Purpose and Scope
### Purpose
This incident response plan exists to ensure Nova Scotia Power is prepared to manage cyber incidents effectively and efficiently. Cybersecurity incidents are increasingly frequent and sophisticated, posing a serious risk to organizations worldwide. Nova Scotia Power is not immune to such threats and must be equipped to detect, prevent, and respond to incidents. By having a structured plan, a trained team, and conducting regular exercises, we will be better prepared to respond to inevitable incidents, minimizing potential damage and mitigating further risks to our organization. Resources must be deployed in an organized manner, utilizing exercised skills and clear communication strategies (Government of Canada, Innovation, Science and Economic Development Canada, Office of the Deputy Minister, Digital Transformation Service Sector & Digital Transformation Service Sector, 2021d).<br>
This document outlines the comprehensive plan for responding to cybersecurity incidents at Nova Scotia Power. It identifies the incident response structure, roles, responsibilities, common types of incidents, and the steps for preparing, identifying, containing, eradicating, recovering, and conducting lessons learned, all aimed at minimizing the impact of cybersecurity incidents.
The goal of this incident response plan is to ensure Nova Scotia Power is organized to respond to cybersecurity incidents both effectively and efficiently.
### Scope
This incident response plan applies to Nova Scotia Power’s networks, systems, data, and all stakeholders (including employees, contractors, and third-party vendors) who have access to them. Members of the Cybersecurity Incident Response Team (CSIRT) are expected to lead or participate in incident response activities. CSIRT members must familiarize themselves with this plan and be prepared to collaborate with the goal of minimizing the adverse effects on the organization.
This document establishes the incident handling and response capabilities of Nova Scotia Power and outlines the appropriate responses for common cybersecurity incidents. It does not provide a detailed list of every activity that should be performed but rather serves as a framework for combating cybersecurity incidents.
## Authority
Responsibility for the security of company and customer information resides with the President and CEO of Nova Scotia Power, Peter Gregg. In the event of a high or critical cybersecurity incident, this responsibility is delegated to the Chief Information Security Officer (CISO). However due to organization structure Shoaib Qabil Badshah the Grid Operations & Security
Manager will act as the Chief Information Security Officer. During such incidents, Shoaib Qabil Badshah, in collaboration with the Cybersecurity Incident Response Team (CSIRT), will oversee the execution of the incident response plan and ensure that all necessary actions are taken to safeguard the organization’s assets and information.

## Definitions
Review the definitions below and retain or revise as required. If necessary, expand the list to best reflect your organization's unique cyber security incident response plan.<br>
**Acceptable interruption window in business continuity planning** - is the amount of time in which basic functionality must be restored for critical systems. It is a major factor when planning a disaster recovery solution.<br>
**Confidentiality** - is a classification of data that typically refers to personally identifiable information. It may include such things as social insurance numbers, drivers licence numbers, etc.<br>
**Cyber security event** - is an observable occurrence in a system or network. Events include a user connecting to a file share, a server receiving a request for a web page, or a user sending email.<br>
**Cyber security incident**- is any incident that occurs by accident or deliberately that impacts communications or information processing systems. An incident may be any event or set of circumstances that threatens the confidentiality, integrity or availability of information, data or services within Nova Scotia Power. This includes unauthorized access to, use, disclosure, modification, or destruction of data or services used or provided by NS Power.<br>
**Denial of service (attack)**- also known as a dos attack, seeks to make a remote service unavailable to its intended users by flooding its host with superfluous requests, thereby overloading the system.<br>
**Exploit** -  in cyber security terms is a piece of software, a chunk of data, or a sequence of commands that takes advantage of a bug or vulnerability to cause unintended or unanticipated behavior to occur on computer software, hardware, or something electronic.<br>

**Indicators**- also known as "indicators of compromise" or iocs, are forensic clues or symptoms left behind by cybersecurity attacks or breaches in the company's network or systems. These clues are sometimes found in log entries, files, or databases.<br>
**Integrity** - refers to the maintenance or assurance of data accuracy, consistency, and its accessibility to authorized users for its entire life-cycle.<br>
**Maximum tolerable downtime** - in business continuity planning, this specifies the maximum period of time that a given business process can be inoperative before the organization's survival is at risk.<br>
**Response playbook** - introduces prescriptive cyber security measures and best practices that can be implemented to improve the organization's security profile. This playbook provides a set of standards to reference the organization, improves current systems and implement new ones.<br>
**Service availability**- describes the state of a system being available and responsive to prospective users. The term is sometimes used to reference a measure of reliability of a system or network resource based on how often it is available as a % of time. For example, 99.97% service availability means that a system is available 99.97% of the time.<br>
**SLA**- stands for service level agreement and is used to describe a guaranteed measure of service availability. If service availability drops below the prescribed sla, there are usually financial repercussions, like a money-back guarantee.<br>
**Stakeholder relationship map** - is a diagram that describes the relationship between individuals in an organization. With respect to cyber security, these diagrams are used to perform it risk assessments to better inform preventative and reactive measures.<br>
**Vulnerability**- is a piece of code or bug within a system that causes unintended or unanticipated behavior. A vulnerability implies that this behaviour can be taken advantage of for malicious reasons.<br>
**War room** -  is a dedicated meeting room where major incidents are handled together. It must have a door for privacy, must be available at all times, and must have good communications infrastructure (network, phone, etc.)<br>
**Zero-day** - is a type of vulnerability that is known to the software vendor but doesn't have a patch in place to fix the flaw. It has at least the potential to be exploited, if it has not already been exploited by cybercriminals.<br>

## How to recognize a cyber an incident
A cybersecurity incident may not be immediately apparent, but there could be indicators of a security breach, system compromise, unauthorized activity, or signs of misuse within Nova Scotia Power’s environment or that of our third-party service providers. It is crucial to remain vigilant for any signs that a security incident has occurred or may be in progress. Some key indicators applicable to Nova Scotia Power include: <br>
-	**Excessive or unusual login and system activity**, especially from inactive or unexpected user accounts (e.g., accounts that have not been in use for an extended period).
-	**Excessive or unusual remote access activity into the company's systems**, whether from employees, contractors, or third-party vendors.
-	**The appearance of unfamiliar or unauthorized wireless networks** (Wi-Fi) that are visible or accessible from within the company environment.
-	**Unusual activity related to malware, suspicious files**, or unauthorized executable files and programs found on Nova Scotia Power’s networks or systems, including customer-facing or web-facing systems.
-	**Hardware or software keyloggers** discovered on or connected to Nova Scotia Power’s devices or systems.
-	**Suspicious or abnormal behavior** on web-facing systems, such as unexpected activity on customer portals or billing systems.
-	**Unusual activity in control systems**, such as SCADA (Supervisory Control and Data Acquisition) systems, which manage critical infrastructure.
-	**Detection of tampered physical devices**, such as company laptops, payment terminals, or network equipment, showing signs of unauthorized physical access.
-	**Loss or theft of sensitive equipment or devices**, including computers, laptops, hard drives, USB sticks, or other media devices that contain proprietary company data, customer information, or other sensitive data (Government of Canada, Innovation, Science and Economic Development Canada, Office of the Deputy Minister, Digital Transformation Service Sector & Digital Transformation Service Sector, 2021d).



## Cybersecurity Incident Response Team (CSIRT) Structure
The Cybersecurity Incident Response Team (CSIRT) at Nova Scotia Power consists of key individuals responsible for managing and responding to cybersecurity incidents. The structure follows a common CSIRT model, which includes an executive, incident handler, communication spokesperson, and technical support roles across various departments.
CSIRT Structure:
-	Executive: Peter Gregg – President & Chief Executive Officer (NSP)
-	Incident Handler: Shoaib Qabil Badshah – Grid Operations & Security Manager
-	Communications: Lia MacDonald – Vice President Customer Experience & Innovation
-	Note-taker: Cali Beck – Analyst, Business
-	Network: Pushpendra Singh – System Security Engineering Specialist
-	Desktop: Eric Henderson – System Security Engineer
-	Server: Gilles Samson – Sr. Engineer
-	Legal: Judith Ferguson – Executive Vice President Regulatory Legal & Business Planning <br> <br>

Chart below show the organization structure of Nova Scotia Power <br>
![image](https://github.com/user-attachments/assets/7249860c-c768-4ba8-9177-97d753095bd6)
<br>
Chart below show the Security Operation Center Team of Nova Scotia Power <br>
![image](https://github.com/user-attachments/assets/c63246dc-9c11-449f-b8cc-c9c8d31d5cf3)
<br>
CSIRT roles and responsibilities <br>
![image](https://github.com/user-attachments/assets/eeb6abab-9b21-407e-8f94-b99ee0030203)


Key External Contacts & Stakeholders
-	Legal Representative: Judith Ferguson – Executive Vice President Regulatory Legal & Business Planning
-	Third-Party Vendors: Contact information for critical service providers should be maintained and regularly updated.
-	Financial Institutions: Chris Smith – Executive Vice President Finance
-	IT Providers: External vendors or contracted IT teams involved in incident handling or investigation.
-	Key Clients: Ensure that key clients, especially those depending on Nova Scotia Power’s critical infrastructure, are notified if their services may be impacted.<br>

### CSIRT Responsibilities
The responsibilities described below are organized by role within Nova Scotia Power.
Executives
The executives, led by Peter Gregg, President & CEO, are responsible for:
-	Approving the overall cybersecurity incident response plan and ensuring it aligns with business objectives.
-	Allocating resources (financial, personnel, and technical) necessary to effectively respond to and mitigate incidents.
-	Serving as the final decision-making authority on incident response, especially in the case of high-impact or critical incidents.
-	Ensuring regulatory and legal compliance in relation to incident response, including reporting breaches to necessary authorities.
-	Reviewing and approving post-incident reports and recommendations to improve cybersecurity measures.
-	Communicating with the board of directors and key stakeholders regarding the impact and management of cybersecurity incidents.





Incident Handler
The Incident Handler, led by Shoaib Qabil Badshah, Grid Operations & Security Manager, is responsible for:
-	Coordinating and directing the CSIRT during an incident, ensuring a swift and organized response.
-	Identifying, assessing, and classifying the severity of incidents based on available data.
-	Initiating the incident response procedures, including containment, eradication, and recovery actions.
-	Ensuring that all relevant logs, reports, and evidence are collected and preserved for forensic analysis.
-	Leading post-incident analysis to identify vulnerabilities or gaps in the organization’s security posture.
-	Keeping the executive team informed of incident status and escalating issues when necessary.

Communications Expert
The Communications Expert, led by Lia MacDonald, Vice President Customer Experience & Innovation, is responsible for:
-	Developing and executing communication strategies during a cybersecurity incident to ensure transparency with employees, customers, and third parties.
-	Acting as the spokesperson for both internal and external communications related to the incident.
-	Managing media relations and coordinating public disclosures when necessary, ensuring accurate and timely information is provided.
-	Collaborating with legal and regulatory teams to ensure communications meet compliance standards.
-	Coordinating with customer support teams to provide consistent messaging and updates to affected customers.
-	Conducting post-incident communication reviews to improve future response efforts.

CSIRT Team
Members of the Cybersecurity Incident Response Team (CSIRT), including Pushpendra Singh, Eric Henderson, Gilles Samson, and other team members, are responsible for:
-	Assisting in the detection, analysis, containment, and eradication of threats during a cybersecurity incident.
-	Conducting technical investigations to determine the root cause of incidents and prevent recurrence.
-	Ensuring that systems (network, desktop, server, etc.) are secured and fully restored after an incident.
-	Maintaining up-to-date incident response tools, techniques, and procedures to improve team readiness.
-	Working closely with third-party vendors, contractors, and service providers to coordinate external assistance if needed.
-	Participating in regular incident response training and simulations to ensure preparedness.

All Staff Members
All staff members at Nova Scotia Power are responsible for:
-	Reporting any suspicious activities or potential cybersecurity incidents to the CSIRT immediately.
-	Adhering to cybersecurity policies and procedures, including using strong passwords, multi-factor authentication, and encryption.
-	Completing regular cybersecurity awareness training to recognize phishing attempts and other attack vectors.
-	Following the incident reporting guidelines and cooperating fully with the CSIRT during an investigation.
-	Protecting sensitive company and customer data in accordance with Nova Scotia Power’s information security policies.
-	Refraining from tampering with or attempting to resolve an incident independently, unless directed by the CSIRT.

### Contact Information OF CSIRT Team <br>
![image](https://github.com/user-attachments/assets/80b95afd-0656-4e08-a00c-dcc8775569ba) 
<br>
(Information Security Policy Templates | SANS Institute, n.d.)

## Severity Matrix 
The Incident Severity Matrix categorizes incidents into four levels of severity: Critical, High, Medium, and Low. Each category is associated with specific actions that must be taken by the CSIRT. <br>
![image](https://github.com/user-attachments/assets/38b0c760-4074-4e69-9509-5714fe867b68)
