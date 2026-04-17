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


---

## Screenshots

### 1. Fleet Agent Connected

<img width="1783" height="726" alt="image" src="https://github.com/user-attachments/assets/51290381-ceb8-40d9-ab89-3309dd7d2845" />


### 2. Discover Logs

<img width="1915" height="932" alt="image" src="https://github.com/user-attachments/assets/b1cfc2ba-932a-45a5-8a8c-ed4d85211724" />



### 3. Nmap Detection Query

Show the query:

```text
process.name: "nmap"
```

<img width="1793" height="816" alt="image" src="https://github.com/user-attachments/assets/e09d470c-1f11-4b4b-b3a7-b5af80ae4188" />



### 4. Dashboard

<img width="1919" height="875" alt="image" src="https://github.com/user-attachments/assets/1e19e213-b8bb-4435-a90c-a0d712d3ddd5" />


### 5. Alert Rule

<img width="1489" height="874" alt="image" src="https://github.com/user-attachments/assets/f1037f85-cf6b-4e3d-a2cd-b73b8fb539f8" />


### 6. Alert Generated

<img width="1493" height="266" alt="image" src="https://github.com/user-attachments/assets/2f66d216-c058-40d7-b5e2-14d39c7e4bac" />


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
