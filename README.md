# 🛡️ DDoS Mitigation & Firewall Policy – Real-World Case Study

This project documents a real-world incident where I identified and mitigated a DDoS attack by analyzing firewall logs and implementing targeted firewall policies to protect organizational infrastructure.

---

## 🔍 Scenario Overview

- 📍 **Company Size**: Small to mid-sized organization  
- 🚨 **Incident**: High traffic volume from multiple IPs caused service disruption. Firewall logs revealed patterns consistent with a DDoS attack.

---

## ⚙️ Tools & Technologies Used

- **Firewall**: FortiGate  
- **Firewall Log Viewer / Analyzer**  
- **Network Monitoring Concepts (TCP/IP, ports, SYN flood patterns)**  
- **Policy Management Interface** : GUI

---

## 🚦 My Response

### Step 1: Analyzed Firewall Logs  
- Detected a spike in traffic targeting our **public IP address** from multiple sources  
- Most of the incoming traffic was being blocked by the firewall  
- However, logs revealed that **a specific policy allowed access from the public IP to two internal servers**

### Step 2: Identified the Exposure  
- Traced the traffic flow and confirmed that the open policy was unintentionally allowing **external access to internal resources**  
- This bypassed the firewall’s default-deny behavior on other services and ports  
- Investigated the original intent of the policy and confirmed it was no longer needed

### Step 3: Mitigation  
- Immediately modified the misconfigured policy to block unauthorized access  
- Verified that the internal servers were no longer reachable via the public IP

### Step 4: Post-Resolution  
- Monitored firewall logs to confirm that all incoming traffic to the public IP was being properly denied  
- Documented the root cause, response actions.


---

## 📘 Lessons Learned

- Effective log analysis is crucial for identifying attack patterns early  
- Proper firewall configuration is the first line of defense in a DDoS scenario  
- Real-world experience helped reinforce threat detection and mitigation workflows
---

> 🔐 *This project is for educational purposes only. All sensitive details have been excluded or anonymized.*

---

📌 **Summary for Recruiters & Reviewers**:  
*This project demonstrates how I investigated unauthorized access through a misconfigured firewall policy tied to a public IP, and resolved it by analyzing logs, updating rules, and restoring secure access control.*

