# Module 15: Cloud Security

<a id="module151"></a>
### Cloud Computing Basics

Cloud computing has become integral to modern IT infrastructure. Understanding its basics is crucial for securing cloud environments.

#### Models (IaaS, PaaS, SaaS)

1. **Infrastructure as a Service (IaaS):**
   - Provides virtualized computing resources over the internet.
   - Example IaaS Providers: AWS, Azure, Google Cloud
   - Example Command (AWS CLI):
     ```
     aws ec2 describe-instances
     ```

2. **Platform as a Service (PaaS):**
   - Offers a platform allowing developers to build, deploy, and manage applications.
   - Example PaaS Providers: Heroku, Google App Engine
   - Example Deployment:
     ```
     git push heroku master
     ```

3. **Software as a Service (SaaS):**
   - Delivers software applications over the internet.
   - Example SaaS Applications: Office 365, Salesforce

#### Deployment Models (Public, Private, Hybrid)

1. **Public Cloud:**
   - Resources are owned and operated by a third-party cloud service provider.
   - Example Public Cloud Providers: AWS, Azure, Google Cloud

2. **Private Cloud:**
   - Resources are used exclusively by a single organization.
   - Example Private Cloud Solutions: VMware, OpenStack

3. **Hybrid Cloud:**
   - Combination of public and private clouds, allowing data and applications to be shared between them.
   - Example Hybrid Cloud Setup:
     ```
     # Integration of on-premise data center with AWS services.
     ```

<a id="module152"></a>
### 15.2 Securing Cloud Infrastructure

Securing cloud infrastructure involves a shared responsibility model and robust identity and access management practices.

#### Shared Responsibility Model

1. **Provider Responsibilities:**
   - Cloud providers manage the security of the cloud infrastructure.
   - Example Provider Responsibilities:
     ```
     # AWS manages security of the cloud, including the hardware, software, networking, and facilities.
     ```

2. **User Responsibilities:**
   - Users are responsible for securing their data and applications in the cloud.
   - Example User Responsibilities:
     ```
     # Users must configure security groups, manage access controls, and encrypt sensitive data.
     ```

#### Identity and Access Management (IAM)

1. **IAM Concepts:**
   - Understand IAM concepts like users, groups, roles, and policies.
   - Example IAM Policy:
     ```
     # Define an IAM policy allowing read-only access to S3 buckets.
     ```

2. **Multi-Factor Authentication (MFA):**
   - Enable MFA to add an extra layer of security to user accounts.
   - Example MFA Setup:
     ```
     # Configure MFA for AWS IAM users.
     ```

### [Go to Index](index.md) | [Previous Module: Incident Response and Forensics](Module14.md) | [Next Module: IoT Security](Module16.md)

*Secure the Future. Learn Cybersecurity.*

### -Ritwik Dadarwal ;)
