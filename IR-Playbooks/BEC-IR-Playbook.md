# Business Email Compromise (BEC) IR Playbook

## 1. Preparation
- Ensure AuditLogs, SigninLogs, and Mailbox auditing are enabled.
- Define communication channels with Legal, HR, and Management.

## 2. Identification
- Trigger: Suspicious inbox rule creation, unusual sign-ins, user reports strange activity.
- Validate: Check recent sign-ins, locations, MFA prompts, and inbox rules.

## 3. Containment
- Temporarily disable or lock the compromised account if necessary.
- Revoke all active sessions and refresh tokens.
- Block malicious IP addresses and risky locations.

## 4. Eradication
- Remove malicious inbox rules and forwarding.
- Clean up unauthorized app registrations or consents.
- Ensure no additional accounts have been affected.

## 5. Recovery
- Reset password and enforce strong MFA.
- Restore mailbox content if emails were deleted or moved.
- Monitor the account closely for a defined period.

## 6. Lessons Learned
- Update BEC detections and training.
- Tighten conditional access and geo-based restrictions.
