

### Active Directory Home Lab

#### Objective

The primary objective of this project is to create a simulated Active Directory (AD) environment for learning IT administration and cybersecurity concepts. By deploying Active Directory, configuring Splunk for log management, and conducting simulated attacks with Kali Linux, we aim to gain hands-on experience in network security, threat detection, and incident response.

#### Skills Utilized

- **Infrastructure Deployment and Configuration:** Setting up servers, computers, networking components, and virtualization environments.
- **Active Directory Administration:** Configuring domain controllers, user accounts, group policies, and organizational units.
- **Splunk Log Management:** Installation, configuration, and utilization of Splunk for centralized log collection, analysis, and visualization.
- **Cybersecurity Fundamentals:** Understanding attack techniques, detection methods, and defensive strategies.
- **Network Topology Design:** Creating logical network diagrams to plan and visualize lab environments.

#### Tools and Services Used

- **Virtualization Platform:** VirtualBox for creating virtual machines to simulate network infrastructure.
- **Microsoft Windows Server:** Deployment of Active Directory domain controllers and target machines.
- **Splunk:** Log management platform for collecting, indexing, and analyzing machine-generated data.
- **Kali Linux:** Offensive security distribution for conducting penetration testing and simulated attacks.
- **Draw.io:** Online diagramming tool for designing network topologies and architecture.

#### Lab Environment Details

- **Network Information:**
  - **Domain Name:** MyLab
  - **Network Subnet:** 192.168.10.0/24

- **Server IP Addresses:**
  - **Active Directory Server:** 192.168.10.7
  - **Splunk Server:** 192.168.10.10

- **Client IP Addresses:**
  - **Target Windows Machine:** DHCP-assigned (within the 192.168.10.0/24 range)
  - **Attacker Machine (Kali Linux):** 192.168.10.250

#### Process Overview

1. **Network Design and Lab Setup:**
   - Design a comprehensive network topology using Draw.io, detailing the layout of servers, computers, switches, routers, and internet connectivity.
   - Allocate IP address ranges, define subnets, and plan network segmentation to emulate real-world scenarios.

2. **Server Deployment and Configuration:**
   - Install and configure Microsoft Windows Server on virtual machines to act as domain controllers and Splunk servers.
   - Set up Active Directory services, including domain creation, DNS configuration, and DHCP services for dynamic IP assignment.
   - Configure Splunk Forwarders on Windows Server instances to forward event logs to the Splunk indexer.

3. **User and Group Management:**
   - Utilize Active Directory Users and Computers console to create user accounts, groups, and organizational units (OUs).
   - Organize users into departments such as IT and HR for role-based access control (RBAC) and administrative delegation.

4. **Integration with Splunk:**
   - Configure Splunk to receive, index, and search event logs from Active Directory domain controllers.
   - Create dashboards and alerts in Splunk to monitor user authentication events, group membership changes, and security-related activities.

5. **Brute Force Attack Simulation:**
   - Use Kali Linux as the attacking platform to simulate a brute force attack against a target Windows machine joined to the Active Directory domain.
   - Employ tools like Crowbar or Hydra with password dictionaries to systematically attempt login credentials.
   - Monitor event logs in Splunk to detect and analyze authentication failures and successful login events. (Event ID: 4625 - Failed Logon Attempt, Event ID: 4624 - Successful Logon)

6. **Telemetry Analysis and Incident Response:**
   - Analyze telemetry data collected in Splunk to identify patterns, anomalies, and indicators of compromise (IoCs).
   - Investigate security incidents, correlate events, and perform root cause analysis to understand the attack lifecycle.
   - Utilize open-source intelligence (OSINT) tools such as CyberChef and SpiderFoot to enrich event data and gather additional context about IP addresses, domains, and URLs observed in Splunk logs.

#### Conclusion

Through the implementation of this Active Directory home lab project, we have acquired valuable skills in IT administration, cybersecurity, and incident response. By building and managing a simulated network environment, conducting controlled attacks, and analyzing telemetry data, we have gained practical experience that can be applied to real-world scenarios. This project serves as a foundation for continuous learning and development in the field of cybersecurity and network defense.
