# Sysmon Analysis Guide

## Key Event IDs
- 1: Process creation
- 3: Network connection
- 7: Image loaded (DLL)
- 10: Process access (useful for LSASS access detection)
- 11: File create
- 13: Registry value set
- 15: File stream created

## Process Analysis
- Build process trees by correlating ParentProcessId / ParentImage.
- Identify LOLBins such as powershell.exe, rundll32.exe, wmic.exe, mshta.exe.

## Network Analysis
- Use Event ID 3 to spot unusual outbound connections.
- Look for rare destinations, uncommon ports, and high volume.

## Tips
- Combine Sysmon with SecurityEvent logs for deeper investigations.
