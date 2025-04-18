# Workshop Exercise: Managing Inventories and Credentials in Ansible Automation Controller

## Objective
This workshop provides practical experience with managing inventories and credentials in  automation controller. You’ll learn how to navigate a preloaded inventory, understand its structure, and set up machine credentials for accessing managed hosts.

## Table of Contents
1. [Introduction to Inventories](#1-introduction-to-inventories)
2. [Exploring the 'Workshop Inventory'](#2-exploring-the-workshop-inventory)
3. [Understanding Machine Credentials](#3-understanding-machine-credentials)
4. [Additional Credential Types](#4-additional-credential-types)
5. [Conclusion](#5-conclusion)

**IMPORTANT**
Before we start, by default, the controller detects automatically the client's language and therefore it may be displayed in french, depending on you laptop's configuration. As all exercises are written in english, it will be much more easier for you if the controller uses also english. To force the controller to switch in english, **add "?lang=en" at the end of controller url**. This has to be done only once.

![Lang](images/change_lang.png)

### 1. Introduction to Inventories
In automation controller, inventories define and organize the hosts your playbooks will target. They can be static (a fixed list of hosts) or dynamic (sourced from external systems).


### 2. Exploring the _Workshop Inventory_
The _Workshop Inventory_ is preloaded in your lab environment, representing a static inventory configuration.

- **Accessing the Inventory:** Navigate to **Automation Execution → Infrastructure → Inventories** in the web UI, and select _Workshop Inventory_.
- **Viewing Hosts:** Navigate to **Automation Execution → Infrastructure → Hosts** to see the predefined hosts, similar to those in a traditional Ansible inventory file.

![Hosts](images/hosts.png)


### 3. Understanding Machine Credentials
Machine credentials are essential for establishing secure SSH connections to managed hosts.

- **Accessing Credentials:** Navigate to **Automation Execution → Infrastructure→ Credentials** and select _Workshop Credentials_.
- **Credential Details:** The 'Workshop Credentials' is configured with:
  - **Credential Type:** Machine (for SSH).
  - **Username:** A predefined user, such as `ec2-user`.
  - **SSH Private Key:** Encrypted, providing secure access to hosts.

### 4. Additional Credential Types
Automation controller supports over 30 different credential types for various automation tasks. Here are a few common ones:

- **Network Credentials:** For managing network devices.
- **Source Control Credentials:** For accessing source control systems.
- **Amazon Web Services (AWS) Credentials:** For integrating with AWS services.

These credential types enhance the flexibility and security of your automation efforts.

### 5. Conclusion
This workshop introduces the essential concepts of inventories and credentials within Ansible Automation Controller. Mastering these components is critical for effectively managing your automation environments and ensuring secure access to your infrastructure.

---
**Navigation**
<br>[Previous Exercise](../2.1-Introduction to Ansible Automation Platform) | [Next Exercise](../2.3-Projects & job templates)  
[Click here to return to the Ansible for Red Hat Enterprise Linux Workshop](../README.md#section-2---ansible-tower-exercises)

