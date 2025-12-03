# Ransomware IR Playbook

## 1. Preparation
- Ensure backups are recent and tested.
- Verify EDR and logging coverage across critical systems.

## 2. Identification
- Trigger: Mass file modification, ransom notes, unusual CPU/IO activity.
- Validate: Check EDR alerts, file events, and user reports.

## 3. Containment
- Immediately isolate affected hosts from the network.
- Disable compromised accounts and revoke tokens.
- Block C2 IPs and domains at the firewall.

## 4. Eradication
- Remove ransomware binaries, scripts, and persistence mechanisms.
- Patch exploited vulnerabilities and misconfigurations.
- Scan the environment for similar indicators.

## 5. Recovery
- Restore systems from known-good backups.
- Rebuild high-risk systems (domain controllers, critical servers) if needed.
- Validate integrity and monitor for reinfection.

## 6. Lessons Learned
- Improve segmentation, EDR tuning, and backup strategy.
- Review user awareness training and phishing defences.
