# Module 8: Network Scanning and Enumeration

<a id="module81"></a>
### 8.1 Network Scanning Techniques

#### Port Scanning

Port scanning is a pivotal phase in cybersecurity, enabling the identification of open ports on a target system. Understanding the network topology is crucial for developing effective defense strategies.

**Port Scanning Techniques:**

1. **TCP Connect Scan:**
   - **Description:** Establishes a full connection to each port.
   - **Example Nmap Command:**
     ```
     nmap -sT -p 1-1000 target_ip
     ```

2. **SYN Scan:**
   - **Description:** Sends SYN packets to identify open ports.
   - **Example Nmap Command:**
     ```
     nmap -sS -p 1-1000 target_ip
     ```

3. **UDP Scan:**
   - **Description:** Identifies open UDP ports.
   - **Example Nmap Command:**
     ```
     nmap -sU -p 1-1000 target_ip
     ```

#### Host Discovery

Host discovery is fundamental for focused scanning. It involves identifying active hosts on a network.

**Host Discovery Techniques:**

1. **Ping Sweep:**
   - **Description:** Sends ICMP Echo Requests to identify live hosts.
   - **Example Nmap Command:**
     ```
     nmap -sn 192.168.1.0/24
     ```

2. **ARP Scan:**
   - **Description:** Uses ARP requests to discover hosts in the local network.
   - **Example Nmap Command:**
     ```
     nmap -PR 192.168.1.0/24
     ```

#### Vulnerability Scanning

Vulnerability scanning is critical for identifying and assessing weaknesses in systems and applications.

**Vulnerability Scanning Process:**

1. **Discovery:**
   - Identify target systems and services.

2. **Enumeration:**
   - Gather information about target systems.

3. **Assessment:**
   - Identify vulnerabilities.

4. **Reporting:**
   - Provide detailed reports.

**Example OpenVAS Command for Vulnerability Scanning:**
- Launching a vulnerability scan against a target.
  ```
  omp -u admin -w admin --xml='<create_task><name>Target_Scan</name><comment>Vulnerability Scan</comment><config id="daba56c8-73ec-11df-a475-002264764cea"/></create_task>' --pretty-print
  ```

<a id="module82"></a>
### 8.2 Enumeration and Information Gathering

#### DNS Enumeration

DNS enumeration involves gathering information about domain names, subdomains, and associated records.

**DNS Enumeration Techniques:**

1. **Zone Transfer:**
   - Requests all DNS information from a DNS server.
   - **Example Dig Command:**
     ```
     dig axfr example.com @dns_server
     ```

2. **DNS Query:**
   - Interrogates DNS servers for specific information.
   - **Example Dig Command:**
     ```
     dig +short -t ANY example.com
     ```

#### SNMP Enumeration

SNMP enumeration gathers information from network devices using the Simple Network Management Protocol.

**SNMP Enumeration Steps:**

1. **SNMP Walk:**
   - Retrieve a list of all SNMP objects on a device.
   - **Example SNMPwalk Command:**
     ```
     snmpwalk -v2c -c public target_ip
     ```

2. **SNMP Get:**
   - Fetch specific information from SNMP-enabled devices.
   - **Example SNMPget Command:**
     ```
     snmpget -v2c -c public target_ip sysDescr.0
     ```

### [Go to Index](index.md) | [Previous Module: Security Information and Event Management (SIEM)](Module7.md) | [Next Module: Penetration Testing](Module9.md)

*Secure the Future. Learn Cybersecurity.*

### -Ritwik Dadarwal ;)