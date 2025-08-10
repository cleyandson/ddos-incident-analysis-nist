# DDoS Incident Analysis and Network Hardening Proposal

<div align="right">
<a href="./README-PT.md">Ver em Português 🇧🇷</a>
</div>

## Project Overview

A practical case study developed as part of the [Google Cybersecurity Professional Certificate](https://www.coursera.org/google-certificates/cybersecurity-certificate), focused on analyzing a security incident and applying the NIST Cybersecurity Framework to guide the response. The objective was to analyze a Distributed Denial of Service (DDoS) attack, identify the root vulnerability, and propose an effective network hardening plan to prevent future incidents.

---

## The Scenario

The analysis was based on an incident where a multimedia company's network services were disrupted for two hours. The investigation revealed that the outage was caused by a denial-of-service attack that exploited a critical vulnerability in the organization's network infrastructure:

**Misconfigured Firewall:** The company's firewall lacked rules to filter or rate-limit ICMP packets, allowing a malicious actor to overwhelm the network with a *ping flood* attack.

---

## Analysis Methodology

To investigate and respond to the scenario, the following methodology, based on the NIST CSF, was applied:

* **Incident Analysis:** Investigation of the security event to determine the attack type, entry vector, and impact on the organization's services.
* **Root Cause Analysis (RCA):** Assessment of the network configuration to identify the specific security flaw (the misconfigured firewall) that allowed the attack to succeed.
* **NIST Framework Application:** Utilization of the five functions of the NIST Cybersecurity Framework (Identify, Protect, Detect, Respond, and Recover) to structure the analysis and improvement recommendations.
* **Technical Documentation:** Consolidation of all findings and recommendations into a formal Incident Report and Hardening Plan.

---

## Incident Report and Hardening Plan (PDF)

The full report, detailing the incident analysis, the application of the NIST framework, and the technical justifications for each recommendation, can be found at the link below.

* 📄 **[Incident Report Analysis - English Version (PDF)](https://github.com/cleyandson/ddos-incident-analysis-nist/blob/08ef4f39fd823ed6d2ef508a2425bee0a612a40b/Documents/%5BEN%5D%20Incident%20report%20analysis.pdf)**

---

## Hardening Recommendations

Based on the root cause analysis, the following remediation actions were recommended to mitigate the identified risks:

* **Implementation of Firewall Rules (Rate Limiting):** Configure the firewall to limit the ingress rate of ICMP packets. This measure serves as the first line of defense and directly prevents the network from being overwhelmed by the same type of attack.
* **Enablement of Source IP Verification:** Implement source IP verification (anti-spoofing) on the firewall to block packets with forged IP addresses, a common tactic in DDoS attacks.
* **Deployment of IDS/IPS:** Add an Intrusion Detection and Prevention System (IDS/IPS) to actively inspect traffic and block packets based on known threat signatures or suspicious behavior.
* **Continuous Network Monitoring:** Implement network monitoring software to establish a baseline of normal traffic and generate automatic alerts for anomalies, increasing the speed and efficiency of detection.

---

## Skills Demonstrated

This project highlights the following essential cybersecurity skills:

-   ✅ **Security Incident Analysis**
-   ✅ **NIST CSF Framework Application**
-   ✅ **Network Hardening**
-   ✅ **Root Cause Analysis (RCA)**
-   ✅ **Technical Report Writing**
-   ✅ **Security Policy and Control Recommendation**

---

## Contact

* **LinkedIn:** [Cleyandson Fragoso](https://www.linkedin.com/in/cleyandson-fragoso/)
* **Email:** cleyandsontech@gmail.com
