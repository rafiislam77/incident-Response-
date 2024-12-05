# Incident Response Playbook 
## Purpose and Scope
### Purpose
The purpose of this document is to create incident response playbook for a large organizaion. I have selected Nova Scotia power as the organization and created an incident response playbook. This main objective of this incident response playbook is to  ensure Nova Scotia Power is prepared to manage cyber incidents effectively and efficiently. Cybersecurity incidents are increasingly frequent and sophisticated, posing a serious risk to organizations worldwide. Nova Scotia Power is not immune to such threats and must be equipped to detect, prevent, and respond to incidents. By having a structured plan, a trained team, and conducting regular exercises, we will be better prepared to respond to inevitable incidents, minimizing potential damage and mitigating further risks to our organization. Resources must be deployed in an organized manner, utilizing exercised skills and clear communication strategies (Government of Canada, Innovation, Science and Economic Development Canada, Office of the Deputy Minister, Digital Transformation Service Sector & Digital Transformation Service Sector, 2021d).<br>
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

### Response Actions:
-	For Critical incidents, immediate executive involvement, legal consultation, and external communication are required, led by Peter Gregg, Judith Ferguson, and the Incident Handler, Shoaib Qabil Badshah. The full CSIRT will be activated, including all necessary engineers and communication personnel.
-	For High incidents, similar responses are initiated, though without the immediate need for broad public communication unless data loss or reputational damage is suspected.
-	Medium severity incidents may require focused efforts from specific departments or teams, coordinated by the Incident Handler, and may not necessitate full CSIRT activation.
-	Low severity incidents will often be handled locally, with the CSIRT being notified for documentation and further monitoring. <br>

## Incident Handling Process Overview (PICERL Model)
In the event of a cybersecurity incident, Nova Scotia Power's Cyber Security Incident Response Team (CSIRT) will adhere to the following PICERL process:
### Preparation
Preparation focuses on preparing the CSIRT to handle incidents by ensuring that all team members, tools, and processes are in place and operational.
Procedures:
-	Conduct regular security awareness training: Ensure all employees, especially CSIRT members, are trained in incident response procedures. Train personnel on incident types like ransomware, unauthorized access, and privacy breaches.
-	Develop and maintain documentation: Ensure that the CSIRT has access to current policies, incident response plans, contact lists, and system architecture diagrams.
-	Ensure monitoring tools are active:
-	Deploy intrusion detection systems (IDS), firewall logs, and SIEM systems.
-	Ensure backups of critical systems are regularly updated and stored securely.
-	Practice incident response drills: Conduct simulations to test the team’s readiness {NIST 7 Step Process (Cyber Security Immersive), n.d.}.

-	Command:
    -	sudo systemctl start fail2ban (Activate Fail2Ban service to monitor and block suspicious activity)
    -	iptables -L (Ensure firewall rules are set up correctly)
________________________________________
### 2. Identification
Identification focuses on detecting and confirming the presence of an incident.
Procedures:
-	Review alerts from monitoring tools: Gather data from logs, firewalls, IDS, antivirus software, and SIEM systems to identify anomalous behavior.
-	Analyze error messages and reports: Review system and network logs for suspicious activity such as unauthorized access attempts or service interruptions (DoS/DDoS).
-	Use automated threat intelligence tools to correlate alerts with known incidents.
-	Command:
    -	sudo tail /var/log/auth.log (Check recent authentication attempts)
    -	grep "error" /var/log/syslog (Search for errors in the system log)
    - sudo netstat -ntlp (Check network connections for suspicious activity) (Desai & Desai, 2024)
- Actions:
    -	If malware or phishing activity is detected, escalate to Incident Handler.
    -	Ensure key stakeholders such as Lia MacDonald (VP Customer Experience & Innovation) and Judith Ferguson (EVP Regulatory Legal & Business Planning) are informed.
________________________________________
### 3. Containment
Containment focuses on limiting the damage caused by the incident and preventing further damage.
Procedures:
-	Isolate affected systems: Disconnect compromised systems from the network to prevent the spread of malware or further unauthorized access.
-	Establish short-term containment:
	Implement temporary solutions such as firewall rules or shutting down affected services.
-	Long-term containment:
-	Apply patches or security updates to affected systems after confirming they are clean.
-	Command:
    -	sudo ifconfig eth0 down (Disable network interface to isolate a server)
    -	iptables -A INPUT -s [IP_ADDRESS] -j DROP (Block malicious IP address) (Desai & Desai, 2024)
-	Actions:
    -	Notify Rehan Khalid (Outage Coordinator Engineer) and Ron MacDougall (Sr. Engineer System Security) for containment actions.
    -	Ensure external stakeholders (e.g., legal, PR, and affected clients) are informed by Communications Expert.

### 4. Eradication
Eradication focuses on removing the threat from the network and ensuring that all traces of the incident have been fully addressed.
Procedures:
-	Remove malicious code or unauthorized access points: Use anti-malware tools or manual processes to eradicate threats.
-	Identify and close vulnerabilities: Implement software patches or reconfigure network settings to close the vulnerability that led to the incident (e.g., close open ports, fix weak passwords).
-	Command:
    -	sudo clamscan -r /home (Scan home directory for malware) (Desai & Desai, 2024)
    - sudo apt-get update && sudo apt-get upgrade (Update system to apply security patches) (Desai & Desai, 2024)
-	Actions:
    -	Ensure involvement of Mohit Agarwal (Engineer) and Pushpendra Singh (System Security Engineering Specialist) for technical eradication tasks.

### 5. Recovery
Recovery focuses on restoring affected systems to normal operation after the threat has been removed.
Procedures:
-	Restore from backups: Ensure that systems are restored from clean backups where necessary.
-	Test and validate systems: Ensure that systems are fully operational and secure by running tests to confirm no residual threats exist.
-	Monitor for anomalies: Continue to monitor systems closely for signs of reinfection or new attacks.
-	Command:
    -  sudo restore /backup/critical_data (Restore data from a verified backup) 
    -	 ping -c 5 [SERVER_IP] (Test connectivity to ensure restoration is complete) (Desai & Desai, 2024)
-	Actions:
    -	Coordinate with Hannah Lawrence (Outage Plan Coordinator) and Cali Beck (Business Analyst) to ensure full system recovery.

### 6. Lessons Learned
Lessons Learned focuses on reviewing the incident after it is resolved to identify ways to improve the organization’s defenses and incident response processes.
Procedures:
-	Post-incident review meeting: Hold a meeting with CSIRT members to evaluate how well the incident was handled, what went wrong, and what improvements can be made.
-	Document findings: Create a formal report summarizing the incident, the response, and the key takeaways. Include details such as whether malicious code or unauthorized access was detected, and how it was handled.
-	Implement changes: Use the lessons learned to update security policies, incident response plans, and CSIRT processes.
-	Actions:
    -	Ensure involvement of executives like Peter Gregg (President & CEO) to make final decisions on improving the incident response strategy.




## Incident-Specific Handling Processes
### Data Breach:
-	Steps:
    -	Isolate affected data systems.
    -	Notify affected stakeholders.
    -	Follow legal requirements for data breach notification under provincial/federal laws.
    -	Involve Judith Ferguson (Legal) and Communications Expert to handle media and regulatory responses.
### Ransomware:
-	Steps:
    -	Isolate the infected system immediately.
    -	Do not pay the ransom; attempt to recover using backups.
    -	Notify legal and PR teams for potential public disclosure.
    -	Coordinate with System Security Engineers like Eric Henderson to identify the point of entry.
     <br>
### Tampering of Payment Terminals:
-	Steps:
     -	Disconnect affected terminals from the network.
     -	Investigate for signs of physical tampering.
     -	Coordinate with financial institutions for fraud prevention.
### Widespread Service Interruption:
-	Steps:
    -	Engage Ron MacDougall and Shoaib Qabil Badshah to assess the extent of the outage.
    -	Prioritize restoring critical services and escalate communication efforts with affected clients.
### Loss of Equipment:
- Steps:
    -	Report the loss to legal and the insurance provider.
    -	Disable access credentials associated with the lost equipment.
    -	Notify the CSIRT team to begin tracking potential unauthorized access attempts.

## Approvals
### Responsible Party
Responsibility for the security of Nova Scotia Power's company and customer information resides with the following responsible party: <br>
The responsible party, Judith Ferguson, has reviewed the incident response plan and delegates the responsibility for mitigating harm to the organization to the Incident Handler or their delegate. <br>
![image](https://github.com/user-attachments/assets/b21a0c11-1141-417c-a072-77a77ea4f1f3)



During times when a high or critical cybersecurity incident is underway, this responsibility is entrusted to the Incident Handler. <br>

## Incident Handler
The incident handler has reviewed the security incident response plan and acknowledges that, when a high or critical cybersecurity incident is underway, responsibility for managing the incident is entrusted to them or their delegate. <br>
The incident handler or their delegate is expected to manage the incident to mitigate further exposure to the organization. The incident will be handled according to the PICERL process: Identification, Containment, Eradication, Recovery, and Lessons Learned.<br>

![image](https://github.com/user-attachments/assets/8e151a51-06cc-4282-9a4a-c94cd33547ff)



### Escalation Scenario
In the event that a high or critical cybersecurity incident occurs and the Incident Handler is unavailable, the following escalation process will be enacted:
- 1.	Initial Assessment by CSIRT:
The CSIRT, led by Eric Henderson (System Security Engineer), will conduct an initial assessment of the incident severity to determine if it meets the criteria for escalation.
- 2.	Delegation to Deputy Incident Handler:
If the Incident Handler is unavailable, authority will be escalated to the Deputy Incident Handler, Shoaib Qabil Badshah (Engineer System Security). The Deputy will take full responsibility for leading the response.
- 3.	Escalation to Senior Management:
If the situation worsens or becomes more critical, Peter Gregg (President & CEO) and Lia MacDonald (VP Customer Experience & Innovation) will be notified for senior-level oversight and decision-making.
- 4.	External Notification:
Depending on the incident, external stakeholders, including legal counsel, regulatory bodies, and affected clients, will be informed by the Communications Expert and Legal Team, led by Judith Ferguson.
- 5.	Approval for Additional Resources:
If required, the Incident Handler or Deputy Incident Handler will request additional technical or financial resources from senior management to contain and mitigate the incident.
- 6.	Post-Incident Review:
After containment, Hannah Lawrence (Outage Plan Coordinator) and Cali Beck (Business Analyst) will lead a post-incident review session with senior management to ensure that lessons learned are incorporated into the updated incident response plan.
<br>


## References

- Government of Canada, Innovation, Science and Economic Development Canada, Office of the Deputy Minister, Digital Transformation Service Sector & Digital Transformation Service Sector. (2021d, December 8). Develop an Incident Response Plan: Fillable template and example. https://ised-isde.canada.ca/site/cybersecure-canada/en/certification-tools/develop-incident-response-plan-fillable-template-and-example
- Gregg, P., Smith, C., Ferguson, J., MacDonald, L., Pickles, D., NSP, Energy Delivery (Transmission) Function Employees, Wholesale Merchant Function Employees, & Power Production (Generation) Function Employees. (2024). SOC-006 Organizational chart (pp. 1–20). https://www.nspower.ca/docs/default-source/monthly-reports/oatt-soc-006---organizational-chart.pdf?sfvrsn=fe306a56_43
- NIST 7 step Process (Cyber Security Immersive). (n.d.). https://web.compass.lighthouselabs.ca/p/14/3101252b-f113-44d0-98b4-79d14da77185
- NIST 7 step Process (Cyber Security Immersive). (n.d.). https://web.compass.lighthouselabs.ca/p/14/3101252b-f113-44d0-98b4-79d14da77185
- Information Security Policy Templates | SANS Institute. (n.d.). https://www.sans.org/information-security-policy/?category=incident-handling
- Desai, N., & Desai, N. (2024, February 5). Top Advanced Linux Commands: Way To become an administrator - cloudyuga.guru. cloudyuga.guru -. https://cloudyuga.guru/blogs/top-advanced-linux-commands-way-to-become-an-administrator/
