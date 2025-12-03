# Account Compromise IR Playbook

## 1. Preparation
- Ensure MFA, conditional access, and sign-in logging are enabled.

## 2. Identification
- Trigger: Unusual sign-ins, MFA fatigue reports, impossible travel alerts.
- Validate: Review SigninLogs, Risky sign-ins, and user confirmation.

## 3. Containment
- Revoke sessions and refresh tokens.
- Temporarily disable the affected account if high risk is confirmed.

## 4. Eradication
- Reset password and enforce MFA re-enrolment.
- Remove suspicious inbox rules or delegated permissions.
- Remove unauthorized devices or app registrations.

## 5. Recovery
- Re-enable account with monitoring.
- Educate the user on phishing and account hygiene.

## 6. Lessons Learned
- Tune detections for earlier identification.
- Strengthen conditional access and monitoring policies.
