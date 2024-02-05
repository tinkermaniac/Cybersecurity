# Module 3: Operating System Security

<a id="module31"></a>
### 3.1 Windows Security

#### User Account Control (UAC)

User Account Control (UAC) is a crucial security feature in Windows, preventing unauthorized changes to the system.

*UAC Mechanisms:*
1. **File and Registry Virtualization:** Redirects write attempts to protected areas, ensuring compatibility with legacy applications.
2. **Elevation of Privilege:** Requests higher permission levels for specific tasks, requiring user consent.

*Configuration:*
Adjust UAC settings using the Control Panel or Group Policy. Lowering the UAC level enhances convenience but reduces security.

#### Windows Defender and Security Features

Windows Defender, Microsoft's built-in antivirus and antimalware solution, provides real-time protection.

*Key Features:*
1. **Virus and Threat Protection:** Scans and protects against malware, ransomware, and other threats.
2. **Firewall and Network Protection:** Monitors network activity and prevents unauthorized access.
3. **Device Security:** Ensures that device drivers and firmware are secure.

*Enhancing Security:*
- Enable automatic updates for Windows Defender definitions.
- Configure periodic full-system scans for comprehensive protection.

<a id="module32"></a>
### 3.2 Linux Security

#### User Management and Permissions

Linux security revolves around robust user management and permission systems.

*User Management:*
1. **User Accounts:** Create, modify, and delete user accounts using commands like `useradd`, `usermod`, and `userdel`.
2. **Password Policies:** Enforce strong password policies using `passwd` and `pam_pwquality`.

*Permissions:*
1. **File Ownership:** Use `chown` to change file ownership, ensuring proper access control.
2. **Access Control Lists (ACLs):** Extend traditional Linux permissions with ACLs for fine-grained control.

#### AppArmor and SELinux

AppArmor and Security-Enhanced Linux (SELinux) are Mandatory Access Control (MAC) frameworks providing additional layers of security.

*AppArmor:*
- Profiles applications, restricting their capabilities based on predefined policies.
- Example: Creating an AppArmor profile for the Apache web server.

*SELinux:*
- Assigns security labels to files, processes, and ports, enforcing policies.
- Example: Using `semanage` to manage SELinux policies.

<a id="module33"></a>
### 3.3 macOS Security

#### Gatekeeper and XProtect

Gatekeeper in macOS ensures only trusted applications are executed.

*Gatekeeper Components:*
1. **App Store:** Allows installation only from the Mac App Store.
2. **Identified Developers:** Permits apps from identified developers.
3. **Anywhere:** Allows apps from anywhere, but with reduced security.

*XProtect:*
- XProtect scans downloaded files for known malware signatures before opening.

#### FileVault and Security Recommendations

FileVault encrypts the entire macOS startup disk to protect data from unauthorized access.

*Enabling FileVault:*
1. Access System Preferences > Security & Privacy > FileVault.
2. Enable FileVault and follow the setup instructions.

*Security Best Practices:*
1. Regularly update macOS to patch security vulnerabilities.
2. Use strong, unique passwords for user accounts and FileVault.

### [Go to Index](index.md) | [Previous Module: Networking Fundamentals](Module2.md) | [Next Module: Cryptography](Module4.md)

*Secure the Future. Learn Cybersecurity.*

### -Ritwik Dadarwal ;)
