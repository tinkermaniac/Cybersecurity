# Module 5: Web Application Security

<a id="module51"></a>
### 5.1 Common Web Application Vulnerabilities

#### SQL Injection

SQL Injection is a prevalent attack vector where malicious SQL queries are injected into input fields.

*Example Attack:*
1. User inputs: `'; DROP TABLE users; --`
2. Malicious SQL Query: `SELECT * FROM users WHERE username = ''; DROP TABLE users; --`

*Prevention:*
- Parameterized Queries: Use parameterized statements to sanitize user inputs.

#### Cross-Site Scripting (XSS)

XSS involves injecting malicious scripts into web pages viewed by other users.

*Types of XSS:*
1. **Stored XSS:** Malicious script permanently stored on the target server.
2. **Reflected XSS:** Script is embedded in a URL and executed when the URL is opened.

*Mitigation:*
- Input Validation: Validate and sanitize user inputs.
- Content Security Policy (CSP): Restrict the types of content that can be loaded.

#### Cross-Site Request Forgery (CSRF)

CSRF exploits the trust a web application has in a user's browser by executing unauthorized actions.

*Example Scenario:*
1. User is logged into a banking site.
2. Attacker tricks the user into clicking a link that initiates a fund transfer without their knowledge.

*Prevention:*
- Use Anti-CSRF Tokens: Include unique tokens in forms to validate the authenticity of requests.

<a id="module52"></a>
### 5.2 Secure Coding Practices

#### Input Validation and Output Encoding

Input validation ensures that user input adheres to expected formats, preventing attacks like SQL Injection and XSS.

*Example Input Validation:*
- Validate email addresses with regular expressions.

```javascript
function isValidEmail(email) {
    const regex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    return regex.test(email);
}
```
Output encoding prevents malicious user input from being executed as code.

*Example Output Encoding:*
- Use HTML encoding to display user input safely.

```html
<p>{{ userProvidedInput | htmlEncode }}</p>
```

#### Authentication and Authorization Best Practices

Implementing robust authentication and authorization mechanisms is critical for web application security.

### Authentication Best Practices:

- **Password Hashing**: Hash and salt passwords using algorithms like bcrypt.
- **Multi-Factor Authentication (MFA)**: Add an additional layer of security with MFA.

### Authorisation Best Practices:
- **Principle of Least Privilege**: Assign the minimum level of access necessary.
- **Role-Based Access Control (RBAC)**: Assign permissions based on user roles.

### [Go to Index](index.md) | [Previous Module: Cryptography](Module4.md) | [Next Module: Malware and Threats](Module6.md)

*Secure the Future. Learn Cybersecurity.*

### -Ritwik Dadarwal ;)
