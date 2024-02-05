# Module 13: Nmap

<a id="module131"></a>
### 13.1 Introduction to Nmap

Nmap, or Network Mapper, is a powerful open-source tool used for network exploration and security auditing. In this module, we'll delve into various aspects of Nmap, from basic scanning techniques to advanced service version detection and scripting capabilities.

#### Port Scanning Techniques

Nmap offers various port scanning techniques, allowing cybersecurity professionals to gather essential information about target systems.

1. **TCP Connect Scan:**
   - Establishes a full TCP connection to target ports.
   - Example Command:
     ```
     nmap -sT <target>
     ```

2. **UDP Scan:**
   - Explores open UDP ports on a target.
   - Example Command:
     ```
     nmap -sU <target>
     ```

3. **SYN Stealth Scan:**
   - Performs a SYN scan to determine open ports.
   - Example Command:
     ```
     nmap -sS <target>
     ```

4. **ACK Scan:**
   - Identifies filtered ports by sending ACK packets.
   - Example Command:
     ```
     nmap -sA <target>
     ```

#### Service Version Detection and Scripting

1. **Service Version Detection:**
   - Nmap can determine the version of services running on open ports.
   - Example Command:
     ```
     nmap -sV <target>
     ```

2. **Nmap Scripting Engine (NSE):**
   - Leverage NSE for advanced scripting and automation.
   - Example Command:
     ```
     nmap --script <script-name> <target>
     ```

3. **Custom Scripts:**
   - Develop custom NSE scripts to suit specific requirements.
   - Example Command:
     ```
     nmap --script custom-script.nse <target>
     ```

### [Go to Index](index.md) | [Previous Module: Armitage](Module12.md) | [Next Module: Incident Response and Forensics](Module14.md)

*Secure the Future. Learn Cybersecurity.*

### -Ritwik Dadarwal ;)
