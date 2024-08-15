# Authenticating People

Authenticating people involves verifying that the individual attempting to access a system or resource is who they claim to be. This is typically done using various authentication methods:

1. **Something You Know**: This includes passwords, PINs, or answers to security questions.
2. **Something You Have**: This includes physical devices like smart cards, security tokens, or mobile phones used for two-factor authentication (2FA).
3. **Something You Are**: This includes biometric data such as fingerprints, facial recognition, or iris scans.

### Examples and Scenarios:

- **Username and Password**: The most common method. When a user tries to log into their email account, they enter their username and password. If the entered credentials match the stored ones, access is granted.  
  **Scenario**: A university's online portal requires students to log in with their student ID (username) and a password to access course materials and grades.

- **Two-Factor Authentication (2FA)**: Adds an extra layer of security by requiring a second form of verification. For example, after entering a password, a user receives a code on their mobile phone that they must enter to complete the login process.  
  **Scenario**: A bank uses 2FA for its online banking system. After entering the username and password, the user receives a one-time code on their registered mobile phone, which they must enter to access their account.

- **Biometric Authentication**: Uses physical characteristics to verify identity. For example, many modern smartphones use fingerprint sensors or facial recognition for unlocking the device.  
  **Scenario**: An office building uses facial recognition technology to allow employees to enter the premises. Each employee's facial data is stored in the system, and the camera at the entrance scans their face to authenticate them.

# Authenticating Systems

Authenticating systems involves verifying that a system or device attempting to connect to a network or access resources is trusted and has the appropriate credentials. This is essential for ensuring that only authorized devices can interact with sensitive data and services.

### Examples and Scenarios:

- **Digital Certificates**: Used in Public Key Infrastructure (PKI) to authenticate devices. Each device has a digital certificate issued by a trusted Certificate Authority (CA). When the device attempts to connect to a network, the certificate is verified.  
  **Scenario**: A corporate network requires all devices to present a digital certificate for network access. Employees’ laptops are issued certificates that are checked each time they connect to the company's Wi-Fi.

- **Secure Tokens**: Hardware or software tokens can be used to authenticate systems. These tokens generate time-based or event-based codes that are used to verify the device.  
  **Scenario**: A company issues USB security tokens to employees for VPN access. The token generates a one-time code that must be entered along with the username and password to establish a secure connection.

- **MAC Address Filtering**: Network access can be restricted based on the MAC address of a device. Only devices with pre-approved MAC addresses can connect.  
  **Scenario**: A university's Wi-Fi network allows only registered devices to connect. Students must register their device's MAC address with the IT department to gain network access.

# Authorization Models

Authorization models determine what resources a user or device can access and what actions they are permitted to perform. Common models include:

1. **Non-Discretionary Access Control (NDAC)**
   - **Description**: A policy-based mechanism where access control policies are centrally managed and enforced. Access permissions are determined by a central authority rather than the owner of the resource.
   - **Example**: A healthcare organization enforces access to patient records based on job functions. For example, doctors can access all patient records, nurses can access only the records of patients they are assigned to, and administrative staff can access only non-clinical records.
   - **Scenario**: In a hospital, the IT department centrally manages access policies to ensure compliance with regulations. Doctors, nurses, and administrative staff are given access based on their roles, regardless of their individual preferences.

2. **Discretionary Access Control (DAC)**
   - **Description**: Allows resource owners to control access based on their discretion. The owner determines who is allowed access to their resources.
   - **Example**: A file owner in a corporate network can grant or deny access to their files. For example, an employee can decide to share a document with specific colleagues by setting permissions on the file.
   - **Scenario**: An employee creates a project document and decides to share it with team members by granting read/write access to specific colleagues. The employee retains control over who can access and modify the document.

3. **Role-Based Access Control (RBAC)**
   - **Description**: Assigns permissions to roles rather than individuals. Users are assigned roles, and each role has specific permissions associated with it.
   - **Example**: In a software development company, roles like Developer, Tester, and Manager are defined. Developers have access to the source code repository, testers have access to the testing environment, and managers have access to project documentation and reports.
   - **Scenario**: A new developer joins the team and is assigned the Developer role. This role automatically grants the necessary permissions to access the source code repository and development tools, streamlining the onboarding process.

4. **Rule-Based Access Control (RuBAC)**
   - **Description**: Uses specific rules to determine access permissions. Rules are based on conditions like time of day, IP address, or user attributes.
   - **Example**: An organization implements a rule that allows access to the corporate network only during business hours and from specific IP addresses.
   - **Scenario**: An employee tries to access the corporate network from home after hours. The system denies access because the rule specifies that remote access is only allowed during business hours from the corporate office IP address.

5. **Mandatory Access Control (MAC)**
   - **Description**: A strict access control model where access permissions are determined by a central authority based on security labels. Users cannot change access policies.
   - **Example**: In a government agency, documents are classified as Top Secret, Secret, and Confidential. Access is granted based on the user's security clearance level.
   - **Scenario**: An employee with Secret clearance tries to access a Top Secret document. The system denies access because the document's classification level is higher than the employee's clearance.

6. **Attribute-Based Access Control (ABAC)**
   - **Description**: Grants access based on attributes of the user, resource, and environment. Attributes can include user roles, departments, project assignments, and more.
   - **Example**: A cloud service provider grants access to resources based on user attributes like department, job function, and project involvement.
   - **Scenario**: A marketing employee needs access to a specific customer data set. The system checks the employee's attributes, including department and project assignment, and grants access based on predefined policies.

7. **Group-Based Access Control**
   - **Description**: Grants access based on group memberships. Users are assigned to groups, and each group has specific permissions.
   - **Example**: In a university, students are assigned to groups based on their courses. Each course group has access to relevant course materials and resources.
   - **Scenario**: A student enrolls in a new course and is added to the corresponding group. The student automatically gains access to course materials, lecture notes, and other resources associated with the group.

8. **Linux-Based Access Control (Linux File Permissions)**
   - **Description**: Uses a combination of user, group, and other (world) permissions to control access to files and directories. Permissions include read (r), write (w), and execute (x).
   - **Example**: A file in Linux has permissions set to `rwxr-xr--`. This means the owner has read, write, and execute permissions; the group has read and execute permissions; and others have only read permissions.
   - **Scenario**: A user creates a script and sets permissions to `rwxr-x---`. The user can read, write, and execute the script; the group can read and execute the script; others cannot access the script at all.

# Summary
- **NDAC**: Centrally managed, policy-based control.
- **DAC**: Resource owners control access.
- **RBAC**: Access based on user roles.
- **RuBAC**: Access based on specific rules.
- **MAC**: Strict, centrally controlled access based on security labels.
- **ABAC**: Access based on user, resource, and environment attributes.
- **Group-Based**: Access based on group memberships.
- **Linux-Based**: User, group, and other permissions for files and directories.

Each model offers a different approach to managing access, catering to various organizational needs and security requirements.
