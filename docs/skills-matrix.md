# Demonstrated SOC Skills Matrix

| Skill | Evidence in this repository | Boundaries |
| --- | --- | --- |
| Telemetry troubleshooting | Sentinel case: disabled Windows Process Creation auditing, Event `4688` source validation | Does not claim every Sysmon event reached Sentinel |
| SIEM detection engineering | Scheduled `SecurityEvent` KQL analytics rule and Sentinel Incident 4 | Historical test rule; not currently active |
| Log querying and correlation | ±5 minute 34-event context → 12 `4688` events → 1 account-matched event | Full original timeline query was not retained |
| Endpoint alert investigation | Defender `BmTestOfflineUI` alert, blocked behavior, Inc 3 | Authorized simulated behavior, not an intrusion |
| Process ancestry | `userinit.exe` → `explorer.exe` → `powershell.exe` process tree | Ancestors started earlier than the test |
| Advanced Hunting | Historical `AlertInfo` query and one result | Other Defender tables showed errors |
| Incident handling | Evidence-based expected activity verdict and saved Defender incident resolution | Sentinel pre-save screenshot alone not closure proof; no incident-driven endpoint isolation |
| Lab network security | Isolated VMnet1 host-only network and controlled Windows VMnet8 NAT | Host not target; no verified NAT port-forwarding |
| Security tools | Local Sysmon ProcessGuid and Wireshark DNS/TCP/TLS correlation | Local results are not automatically cloud telemetry |
| Documentation/evidence QA | Screenshots, source/crop SHA-256 evidence manifests, explicit uncertainty | Portfolio publication still pending |
