# Elastic SIEM Home Lab with Kali Linux

## Project Overview

This project demonstrates how to build a basic SIEM home lab using Elastic Cloud and Kali Linux.

The lab collects logs from a Kali Linux virtual machine using Elastic Agent, stores them in Elasticsearch, visualizes them in Kibana, and creates alerts for suspicious activity.

To simulate attacker behavior, Nmap scans were executed on the Kali machine and detected inside the Elastic SIEM environment.

---

## Objectives

* Collect endpoint logs from Kali Linux
* Detect suspicious Nmap activity
* Analyze logs in Kibana
* Create a dashboard to visualize activity
* Create an alert rule for Nmap scans

---

## Tools Used

* Elastic Cloud
* Elasticsearch
* Kibana
* Elastic Agent
* Elastic Defend
* Kali Linux
* Nmap
* VirtualBox
* KQL

---

## Architecture

```text
Kali Linux VM → Elastic Agent → Elasticsearch → Kibana → Alerts
```

<img width="1536" height="1024" alt="elastic architecture final" src="https://github.com/user-attachments/assets/d82df429-1cda-4e9e-9c6c-1dab89993266" />
<img width="1441" height="959" alt="image" src="https://github.com/user-attachments/assets/e1b8fb4c-e6b9-43bb-b336-bda8cae61b56" />


---

## Screenshots

### 1. Fleet Agent Connected

Show that the Kali agent is healthy and connected.

[Add Fleet agent screenshot here]

### 2. Discover Logs

Show logs being collected from the Kali machine.

[Add Discover logs screenshot here]

### 3. Nmap Detection Query

Show the query:

```text
process.name: "nmap"
```

[Add Nmap query screenshot here]

### 4. Dashboard

Show the graph/dashboard of Nmap activity.

[Add dashboard screenshot here]

### 5. Alert Rule

Show the Nmap detection rule.

[Add detection rule screenshot here]

### 6. Alert Generated

Show that the alert became active after running Nmap.

[Add active alert screenshot here]

---

## Skills Demonstrated

* SIEM configuration
* Log analysis
* Endpoint monitoring
* KQL searching
* Dashboard creation
* Alert creation
* Linux troubleshooting
* Basic threat detection

---

## Challenges Faced

* Downloaded the wrong Elastic Agent version initially
* VM storage became full during setup
* Process logs were not visible until integrations were added
* Needed troubleshooting before Nmap logs appeared

---

## Resume Value

This project demonstrates hands-on SOC analyst skills using the Elastic Stack.

It shows experience with:

* Elasticsearch
* Kibana
* Log monitoring
* Detection rules
* Alerts
* Endpoint visibility

This is a good beginner SOC project and is worth adding to a resume, especially for SOC Analyst L1, Security Analyst, and internship roles.

---

## Conclusion

This project helped build practical experience with Elastic SIEM by collecting, analyzing, visualizing, and detecting endpoint activity from a Kali Linux system.
