# Ransomware – Simulated Incident Report

## Summary
Endpoint activity consistent with ransomware pre-encryption and execution was observed, including mass file modification, credential theft attempts, and outbound C2 traffic.

## Timeline
- T0: User opened suspicious attachment.
- T1: Powershell-based downloader executed; C2 beacon established.
- T2: Attempted LSASS dump for credential theft.
- T3: Lateral movement to file server using WMI/PsExec.
- T4: Mass file rename and encryption on finance file share.
- T5: Ransom note dropped on multiple systems.
- T6: SOC isolated affected systems and initiated IR process.

## Root Cause
Phishing email delivered malware, which evaded initial prevention and executed in user context, followed by privilege escalation attempts and lateral movement.

## Detection
- Sentinel alerts on suspicious PowerShell, LSASS access, and mass file operations.
- MDE detections for ransomware behaviour and C2 communication.
- Network logs showing large outbound transfers to malicious IPs.

## Response
- Isolated infected hosts from the network.
- Revoked tokens and reset passwords for impacted accounts.
- Identified and terminated malicious processes.
- Validated and restored from clean backups where necessary.

## Lessons Learned
- Improve email filtering and sandboxing.
- Expand EDR coverage and hardening policies.
- Implement least-privilege and restrict lateral movement paths.
