# Sysmon + ELK Stack for Endpoint Monitoring

## 🧠 Summary
This project sets up Windows endpoint monitoring using Sysmon and forwards logs to an ELK stack (Elasticsearch, Logstash, and Kibana). It simulates a basic SIEM environment that helps detect and visualize potential attacker behavior.

## 🎯 Objectives
- Collect detailed Windows logs using Sysmon
- Use Winlogbeat to forward logs to Logstash
- Parse and visualize logs in Kibana
- Highlight security-relevant events for analysis

## 🛠️ Tools & Technologies
- Windows 10 VM (Target endpoint)
- Sysmon
- Winlogbeat
- ELK Stack (Ubuntu or Debian server)
- VirtualBox / VMware
- Basic firewall/network rules

## 📐 Architecture
(Insert a diagram here later, or describe like this:)

- Windows 10 VM runs Sysmon and Winlogbeat  
- Logs are forwarded to Logstash on a Linux VM  
- Logstash parses logs and stores them in Elasticsearch  
- Kibana visualizes the logs via a browser dashboard

## 📝 Steps to Reproduce
1. Install Windows 10 in VM
2. Install Sysmon with a custom config (e.g., SwiftOnSecurity)
3. Install and configure Winlogbeat
4. Set up Linux VM with ELK stack
5. Configure Logstash to parse incoming logs
6. Visualize key Windows event IDs in Kibana

## 🔒 Security Concepts Demonstrated
- Endpoint detection and response (EDR)
- SIEM setup and log forwarding
- MITRE ATT&CK behavior mapping (e.g., Event ID 4688 for process creation)

## 💡 Lessons Learned
- Why tuning logs matters more than just collecting them
- How to use dashboards to spot anomalous activity
- Log volume management and false positive reduction

## 📎 References
- [Sysmon Config by SwiftOnSecurity](https://github.com/SwiftOnSecurity/sysmon-config)
- [Elastic Stack Docs](https://www.elastic.co/guide/index.html)

