# Zero Trust

Zero Trust is a security concept based on the principle of "never trust, always verify." It assumes that threats could exist both inside and outside the network and, therefore, no entity (user, device, or system) should be trusted by default. Instead, every access request must be authenticated, authorized, and continuously validated before granting access to resources.

## Key Principles of Zero Trust

1. **Verify Explicitly**:
   - Always authenticate and authorize based on all available data points, including user identity, location, device health, service or workload, data classification, and anomalies.

2. **Use Least Privilege Access**:
   - Limit user and application access to only what is necessary, applying just-in-time and just-enough-access (JIT/JEA), risk-based adaptive policies, and data protection to help secure both data and productivity.

3. **Assume Breach**:
   - Minimize the impact of breaches and prevent lateral movement by segmenting access. Verify end-to-end encryption, use analytics to detect threats, and improve defenses.

## Planes of Operation

1. **Data Plane**:
   - The Data Plane is responsible for the actual transmission of data between endpoints. It handles the forwarding of traffic, data encryption, and decryption, as well as managing the communication between users, applications, and services.

2. **Control Plane**:
   - The Control Plane is responsible for the management and orchestration of network resources. It includes functions such as routing decisions, network topology management, and policy enforcement. The Control Plane determines how data should be handled, but it does not directly handle the data itself.

## Key Concepts in Zero Trust Architecture

1. **Controlling Trust**:
   - Trust should not be implicit based on location (e.g., inside a corporate firewall). Instead, trust must be continually assessed and validated. This involves verifying user identities, ensuring device compliance, and monitoring behavior for anomalies.
   
   - **Example**: An employee working remotely needs access to a sensitive financial application. The employee must use MFA to verify their identity, and their device must pass a compliance check (e.g., updated antivirus, no malware). The request is continuously monitored for anomalies.

2. **Adaptive Identity**:
   - Adaptive Identity involves dynamically adjusting access controls based on the context of a request. Factors such as user behavior, device health, location, and risk levels are considered to adaptively grant or deny access.
   
   - **Example**: A user normally logs in from New York but suddenly tries to access the system from another country. The system prompts the user for additional verification steps due to the unusual location.

3. **Threat Reduction Scope**:
   - This involves minimizing the potential impact of a security breach by reducing the scope of what an attacker can access. This can be achieved through network segmentation, limiting access permissions, and continuously monitoring for suspicious activities.
   
   - **Example**: An attacker gains access to a compromised account. Network segmentation limits the attacker’s movement, and policies restrict access to only the necessary resources for that account, minimizing potential damage.

4. **Policy-Driven Access Control**:
   - Access control is based on policies that define who can access what resources under which conditions. These policies are centrally managed and enforced consistently across the organization.
   
   - **Example**: A developer needs temporary access to production data. A policy grants just-in-time access for a specific task and duration, and all activities are logged and monitored.

5. **Security Zones**:
   - Security Zones are logical or physical segments within a network, each with its own security policies and controls. By segmenting the network into zones, the spread of potential threats can be limited.
   
   - **Example**: Protecting sensitive customer data. Create a separate security zone for databases containing customer information, with stricter access controls and monitoring.

## Components of Policy Enforcement and Decision

1. **Policy Enforcement Point (PEP)**:
   - PEPs are the points where access decisions are enforced. They can be firewalls, gateways, or any network device that can control the flow of data based on the policies set by the Policy Decision Point. PEPs ensure that only authorized traffic is allowed.

2. **Policy Decision Point (PDP)**:
   - PDPs are responsible for making decisions about whether a particular access request should be granted or denied. The PDP evaluates the request against policies defined in the Policy Engine and is often divided into two components:
   
   - **Policy Engine**:
     - The Policy Engine is responsible for the logic that determines whether an access request should be allowed. It uses predefined rules and policies to evaluate the request based on factors like user identity, device health, and current context.
   
   - **Policy Administrator**:
     - The Policy Administrator manages the configuration and deployment of policies across the network. It ensures that the policies defined by the Policy Engine are correctly enforced by the PEPs.

## The 5 W's in Zero Trust Policy

1. **Who**:
   - Identifies the user or system requesting access. This involves verifying the identity through credentials, multi-factor authentication, and role-based access controls.

2. **What**:
   - Defines the resource or data the user is trying to access. This includes files, databases, applications, and services.

3. **When**:
   - Specifies the time or conditions under which access is requested. This could include time of day, day of the week, or specific events.

4. **Where**:
   - Refers to the location from which the access request originates. This could be an IP address, geographical location, or specific network segment.

5. **Why**:
   - Explains the reason or purpose for the access request. This could involve understanding the user’s role, the task they are trying to perform, or the business context of the request.

Zero Trust architecture fundamentally changes the approach to network security by assuming no implicit trust, continuously verifying access requests, and enforcing strict, policy-driven controls. By implementing these concepts and components, organizations can better protect their resources and minimize the risk of breaches.