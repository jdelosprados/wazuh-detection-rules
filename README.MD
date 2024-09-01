# Wazuh SIEM Custom Rules

## Overview

This repository contains templates for Wazuh SIEM detection rules that I used to cut false positive alerts in half across millions of alerts. You can adapt these rules to tune your own SIEM. Focus on filtering out known benign activities and prioritizing high-severity events to help your security team concentrate on the most critical and actionable alerts.

## Rules Overview

**High-Priority Events**  
**Rule ID:** 100001  
Focuses on high-severity attacks, reducing false positives by ignoring lower-priority events.

**Known Benign Alerts**  
**Rule ID:** 100002  
Suppresses alerts from known benign sources to reduce unnecessary noise.

**True Positive Detection**  
**Rule ID:** 100003  
Generates detailed alerts for critical authentication failures.

**Frequency-Based Alerts**  
**Rule ID:** 100004  
Triggers alerts based on the frequency of medium-severity system events to reduce noise.

**Unusual Activity**  
**Rule ID:** 100005  
Detects patterns like multiple failed login attempts, which may indicate a brute-force attack.

**Suspicious Network Activity**  
**Rule ID:** 100006  
Flags unusual network traffic that could signal a potential threat.

**Unauthorized File Changes**  
**Rule ID:** 100007  
Detects unauthorized changes to critical files, indicating potential tampering.

**High CPU Usage**  
**Rule ID:** 100008  
Monitors high CPU usage, which might suggest resource abuse or an ongoing attack.

## Reminders

Before adding or modifying rules, back up your existing configuration files. After implementation, monitor the SIEM dashboard closely to ensure the rules work as expected, and keep your rule configurations well-documented for clarity and future reference.
