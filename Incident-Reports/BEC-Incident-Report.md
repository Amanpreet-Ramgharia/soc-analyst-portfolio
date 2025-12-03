# Business Email Compromise (BEC) – Simulated Incident Report

## Summary
A phishing email led to credential theft and unauthorized mailbox access. The attacker abused MFA prompts and created malicious inbox rules to forward emails externally.

## Timeline
- T0: User received invoice-themed phishing email with fake Microsoft 365 login page.
- T1: User entered credentials; attacker harvested username and password.
- T2: Multiple MFA prompts sent to user (MFA fatigue).
- T3: Successful sign-in from unfamiliar IP and country.
- T4: Inbox rule created to forward or hide messages.
- T5: Mailbox access events (MailItemsAccessed) confirmed suspicious reading of emails.

## Root Cause
User entered credentials into a phishing page; lack of user awareness and no conditional access controls for risky locations.

## Detection
- Sentinel alerts on impossible travel / risky sign-in.
- AuditLogs for `New-InboxRule`.
- MailItemsAccessed logs for unusual access patterns.

## Response
- Revoked all active sessions and refresh tokens for the account.
- Reset password and enforced MFA re-registration.
- Removed malicious inbox rules.
- Blocked attacker IPs and updated conditional access policies.

## Lessons Learned
- Enhance user awareness training.
- Strengthen conditional access for risky sign-ins.
- Implement dedicated BEC and inbox-rule analytic rules.
