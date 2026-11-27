# Recruiter Summary — SOC Detection & Incident Response Home Lab

**Independent practical cybersecurity project | 2026**

Built a controlled SOC practice environment with Windows 11 and Kali Linux VMs in VMware Workstation. Used Windows Security logs, Sysmon, Wireshark, Azure Monitor Agent, Microsoft Sentinel and Microsoft Defender for Endpoint/XDR to validate security telemetry and investigate authorized test activity.

The portfolio includes two evidence-backed investigations:

1. **[Sentinel PowerShell detection](../investigations/01-sentinel-powershell-detection/README.md):** Windows Event ID `4688`, a scheduled KQL analytic, a generated test incident, and a 34 → 12 → 1 event-correlation workflow.
2. **[Defender XDR behavior monitoring](../investigations/02-defender-xdr-behavior-monitoring/README.md):** blocked `BmTestOfflineUI` alert, process-tree analysis and documented analyst closure with an accurately distinguished incident-level classification.

**Demonstrated skills:** Windows Event analysis, SIEM/KQL, endpoint process investigation, EDR/XDR triage, virtual networking, troubleshooting and technical incident reporting.

**Scope:** Authorized home-lab simulations, not production SOC operations. The cloud environment is historical. The repository was published publicly on 27 November 2026.
