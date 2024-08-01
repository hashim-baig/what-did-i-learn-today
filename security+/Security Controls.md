The three key objectives (Confidentiality, Integrity, and Availability) are the CIA triad.
Cybersecurity professionals use the CIA triad to describe risks, attacks, and security controls.

### 1. Confidentiality
**Purpose:** Ensure that only authorized individuals can access sensitive information.  
**Controls:** Firewalls, access control lists, and encryption.  
**Threats:** Attackers may try to access and disclose sensitive information without permission.  
**Examples:**  
- **Encryption:** Scrambles data so it can only be read by someone with the decryption key.  
- **Access Controls:** Use passwords, biometrics, and other methods to restrict access to information.

### 2. Integrity
**Purpose:** Ensure information and systems are not changed without authorization.  
**Controls:** Hashing and integrity monitoring solutions.  
**Threats:** Attackers or accidents (like power spikes) can alter or corrupt information.  
**Examples:**  
- **Checksums and Hash Functions:** Verify data integrity by creating a unique digital fingerprint of data.  
- **Version Control Systems:** Track changes to documents and code to prevent unauthorized alterations.

### 3. Availability
**Purpose:** Ensure that information and systems are available for legitimate users when needed.  
**Controls:** Fault tolerance, clustering, and backups.  
**Threats:** Attackers may try to disrupt access, or events like fires can destroy data centers.  
**Examples:**  
- **Redundant Systems:** Use backup systems to ensure continuous availability even if one system fails.  
- **Load Balancers:** Distribute network traffic across multiple servers to prevent overload and downtime.

### Nonrepudiation (Additional Concept)
**Purpose:** Ensure that someone who performed an action cannot deny it later.  
**Example:** Digital signatures confirm that a message truly came from the sender.

### Evaluating Risks to the CIA Triad
Cybersecurity professionals must assess threats and vulnerabilities that could compromise the confidentiality, integrity, or availability of systems and data. This involves identifying potential risks and implementing appropriate controls to mitigate them.

### Security Controls
Security controls are measures put in place to protect information and systems. They are categorized based on their mechanism of action. Understanding these categories helps organizations design and implement effective security strategies.

#### 1. Technical Controls
**Definition:** Technical controls use technology to enforce security measures. They are often implemented in software, hardware, or firmware.  
**Examples:**  
- **Firewall Rules:** Firewalls block unauthorized access to networks by filtering incoming and outgoing traffic based on predefined security rules.  
  - **Example:** A company configures its firewall to block all traffic from known malicious IP addresses.  
- **Access Control Lists (ACLs):** ACLs restrict access to resources based on user permissions.  
  - **Example:** Only certain employees have permission to access sensitive files on the server.  
- **Intrusion Prevention Systems (IPS):** IPS monitor network traffic for suspicious activity and can automatically take action to prevent attacks.  
  - **Example:** An IPS detects and blocks a SQL injection attempt in real-time.  
- **Encryption:** Encryption converts data into a coded format that can only be read by someone with the correct decryption key.  
  - **Example:** Emails containing sensitive information are encrypted to ensure they can only be read by the intended recipients.

#### 2. Operational Controls
**Definition:** Operational controls involve the processes and procedures used to manage technology securely on a day-to-day basis.  
**Examples:**  
- **User Access Reviews:** Regularly reviewing user access rights to ensure that only authorized individuals have access to certain systems and data.  
  - **Example:** A company conducts quarterly reviews to revoke access for employees who no longer need it.  
- **Log Monitoring:** Continuously monitoring system and network logs for signs of unusual activity.  
  - **Example:** Security analysts review logs daily to detect potential breaches or unauthorized actions.  
- **Vulnerability Management:** Identifying, assessing, and mitigating vulnerabilities in systems and software.  
  - **Example:** Regularly scanning for and patching software vulnerabilities to prevent exploitation by attackers.

#### 3. Managerial Controls
**Definition:** Managerial controls are administrative mechanisms focused on managing risk and guiding the organization’s security strategy.  
**Examples:**  
- **Risk Assessments:** Evaluating potential risks to the organization’s information and systems.  
  - **Example:** Conducting an annual risk assessment to identify and prioritize security threats.  
- **Security Planning Exercises:** Developing and documenting security strategies and plans.  
  - **Example:** Creating a comprehensive incident response plan outlining steps to take in case of a data breach.  
- **Change Management:** Ensuring that changes to systems and processes are managed in a controlled and secure manner.  
  - **Example:** Reviewing and approving all changes to the IT infrastructure to prevent unintended security risks.

#### 4. Physical Controls
**Definition:** Physical controls are security measures that protect the physical environment and hardware from unauthorized access and potential damage.  
**Examples:**  
- **Fences:** Barriers that restrict physical access to a facility.  
  - **Example:** A company installs a high fence around its data center to prevent unauthorized entry.  
- **Perimeter Lighting:** Lighting around a facility to deter and detect unauthorized access attempts.  
  - **Example:** Bright lights around the exterior of the building to discourage intruders and improve visibility for security cameras.  
- **Locks:** Mechanical or electronic devices used to secure doors, cabinets, and other physical assets.  
  - **Example:** Biometric locks on server room doors to ensure only authorized personnel can enter.  
- **Fire Suppression Systems:** Systems designed to detect and extinguish fires to protect equipment and data.  
  - **Example:** Installing a gas-based fire suppression system in the data center to minimize damage to electronic equipment.  
- **Burglar Alarms:** Systems that detect and alert on unauthorized entry.  
  - **Example:** A security alarm system that notifies security personnel of any forced entry into the building.

Organizations must choose security controls that align with their specific control objectives and regulatory requirements. This involves assessing the importance of confidentiality, integrity, and availability for their information and systems.

### Example Scenario
- **Handling Sensitive Information:** An organization handling sensitive customer information might prioritize confidentiality. They would invest heavily in encryption (technical control), access control policies (operational control), and regular security audits (managerial control). Conversely, if their website’s availability is less critical, they might not allocate as many resources to protecting it against denial-of-service (DoS) attacks.

Often, achieving a security objective requires a combination of different types of controls.

### Example Scenario
- **Preventing Unauthorized Access to a Data Center:**  
  - **Physical Control:** Implement biometric locks to ensure that only authorized personnel can enter the data center.  
  - **Operational Control:** Conduct regular reviews of the access list to ensure that only current employees have access.  
  - **Managerial Control:** Perform routine risk assessments to identify potential threats and vulnerabilities related to data center access.

By combining these controls, organizations can create a comprehensive security posture that addresses multiple aspects of security risks.

### Security Control Types
Security control types are categorized based on their desired effect on mitigating security risks.

#### 1. Preventive Controls
**Definition:** Preventive controls aim to stop security issues before they occur by blocking potential threats.  
**Effects:**  
- **Proactive Defense:** Preventive controls create barriers to stop attacks before they can cause harm.  
- **Reduced Incidents:** By preventing incidents, these controls reduce the number of security breaches and associated damage.  
**Examples:**  
- **Firewalls:** Block unauthorized access to a network by filtering incoming and outgoing traffic based on predefined security rules.  
  - **Effect:** Prevents unauthorized network access, thereby protecting internal systems from external threats.  
- **Encryption:** Protects data by converting it into a secure format that can only be accessed by authorized individuals with the decryption key.  
  - **Effect:** Ensures that even if data is intercepted, it cannot be read by unauthorized parties.  
**Use Case:**  
- **Network Security:** A company uses firewalls to prevent unauthorized access to its internal network, blocking potentially harmful traffic from entering the system.

#### 2. Deterrent Controls
**Definition:** Deterrent controls are designed to discourage attackers from attempting to breach security policies by creating the perception of risk.  
**Effects:**  
- **Discouragement:** Potential attackers are less likely to attempt a breach if they perceive high risk or difficulty.  
- **Enhanced Security Posture:** Visible deterrent measures contribute to an overall stronger security posture.  
**Examples:**  
- **Vicious Guard Dogs:** Physical security measures that can deter unauthorized entry.  
  - **Effect:** Potential intruders are discouraged by the presence of guard dogs, reducing the likelihood of attempted break-ins.  
- **Barbed Wire Fences:** Physical barriers that prevent unauthorized access to a facility.  
  - **Effect:** Visible barriers discourage intruders from attempting to climb or breach the fence.  
- **Security Cameras:** Visible surveillance cameras deter criminal activities by increasing the likelihood of being caught.  
**Use Case:**  
- **Facility Security:** A data center installs barbed wire fences and security cameras around its perimeter to deter unauthorized physical access.

#### 3. Detective Controls
**Definition:** Detective controls identify and detect security events that have already occurred, allowing for a timely response.  
**Effects:**  
- **Incident Detection:** These controls alert security personnel to suspicious activities or breaches, enabling prompt investigation and response.  
- **Forensic Analysis:** Helps in understanding how an incident occurred, which aids in preventing future occurrences.  
**Examples:**  
- **Intrusion Detection Systems (IDS):** Monitor network or system activities for signs of malicious behavior and generate alerts.  
  - **Effect:** Detects unauthorized access attempts and provides alerts for immediate action.  
- **Security Information and Event Management (SIEM):** Collects and analyzes log data from various sources to identify suspicious patterns.  
  - **Effect:** Provides comprehensive monitoring and correlation of security events, enabling detection of complex threats.  
- **Audit Logs:** Record system and user activities, providing a trail for forensic analysis.  
**Use Case:**  
- **Network Monitoring:** An organization uses an IDS to monitor its network for signs of malicious activity and alerts the security team when suspicious behavior is detected.

#### 4. Corrective Controls
**Definition:** Corrective controls remediate security issues that have already occurred, restoring systems and data to a secure state.  
**Effects:**  
- **Damage Mitigation:** Corrective controls minimize the impact of security incidents by quickly addressing and resolving issues.  
- **System Recovery:** Ensures that systems and data can be restored to their original state or a secure state after an incident.  
**Examples:**  
- **Restoring Backups:** Recovering data from backups after a ransomware attack or data loss incident.  
  - **Effect:** Restores lost or corrupted data, minimizing the impact of the incident.  
- **Patch Management:** Applying software updates to fix vulnerabilities that were exploited during an attack.  
  - **Effect:** Removes security vulnerabilities, preventing further exploitation.  
**Use Case:**  
- **Ransomware Recovery:** After a ransomware attack, an organization restores its encrypted data from backups and patches the exploited vulnerability to prevent future attacks.

#### 5. Compensating Controls
**Definition:** Compensating controls are alternative measures designed to mitigate risk when primary controls cannot be implemented.  
**Effects:**  
- **Risk Reduction:** Provides a way to manage risk when standard controls are not feasible, ensuring continued security.  
- **Flexibility:** Allows organizations to adapt to specific circumstances while maintaining a secure environment.  
**Examples:**  
- **Manual Review of Access Logs:** When automated logging systems are unavailable or too costly, manual review can serve as a compensating control.  
  - **Effect:** Ensures that access activities are still monitored and reviewed for suspicious behavior.  
- **Increased Monitoring:** Enhanced surveillance or monitoring activities when primary controls are insufficient.  
  - **Effect:** Provides additional oversight to detect and respond to potential threats.  
**Use Case:**  
- **Manual Log Review:** In a small organization without automated SIEM capabilities, security personnel manually review system logs daily to detect potential security incidents.

#### 6. Directive Controls
**Definition:** Directive controls inform employees and others on how to achieve security objectives, providing guidance and instructions.  
**Effects:**  
- **Policy Enforcement:** Ensures that everyone in the organization follows the same security practices and procedures.  
- **Behavioral Guidance:** Directs the actions of employees to align with security goals and reduce human-related risks.  
**Examples:**  
- **Security Policies:** Formal documents that outline an organization's security practices, procedures, and responsibilities.  
  - **Effect:** Provides a framework for implementing and enforcing security measures across the organization.  
- **Standard Operating Procedures (SOPs):** Detailed instructions on how to perform specific tasks securely.  
  - **Effect:** Ensures consistency and compliance with security requirements in daily operations.  
**Use Case:**  
- **Security Policy Implementation:** An organization implements a security policy that mandates regular password changes and provides training to employees on how to create strong passwords.