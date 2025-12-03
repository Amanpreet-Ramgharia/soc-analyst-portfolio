# Windows Security Event ID Guide (SOC Focus)

## Logon & Authentication
- 4624: Successful logon
- 4625: Failed logon
- 4634: Logoff
- 4648: Logon with explicit credentials
- 4672: Special privileges assigned to new logon

## Kerberos
- 4768: Kerberos TGT requested
- 4769: Kerberos service ticket (TGS) requested
- 4771: Kerberos pre-authentication failed

## Account Management
- 4720: User account created
- 4726: User account deleted
- 4728: Member added to global security-enabled group
- 4729: Member removed from global security-enabled group

## System Events
- 1102: Audit log cleared
- 7045: New service installed

Use these IDs to build detections and investigate incidents.
