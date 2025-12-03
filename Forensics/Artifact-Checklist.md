# Windows Forensic Artifact Checklist

## On-Host Artifacts
- Prefetch files
- $MFT (Master File Table)
- Registry hives (SAM, SYSTEM, SECURITY, SOFTWARE, NTUSER.DAT)
- Shimcache / Amcache
- Scheduled tasks
- Services and drivers

## Log Sources
- Windows Security Log
- Sysmon Operational Log
- PowerShell Operational Log
- Application and System Logs

## Network & Cloud
- Firewall logs
- Proxy logs
- VPN logs
- Identity provider logs (Azure AD / Entra ID)

## Goals
- Reconstruct attacker timeline.
- Confirm initial access vector.
- Identify lateral movement and persistence.
- Support IR reports and legal requirements.
