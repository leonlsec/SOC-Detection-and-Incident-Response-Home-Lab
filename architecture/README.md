# Architecture — source and interpretation

The `architecture.svg` / `architecture.png` renders the historical lab and is embedded in the root README. `architecture.mmd` is an editable Mermaid flowchart; `architecture.dot` is an editable Graphviz DOT source for the SVG/PNG rendering. (The two source files use different layout systems but represent the same components and boundaries.)

**Data flows:** Windows Security Event Log → AMA with DCR-configured collection → Log Analytics (`SecurityEvent`) → Microsoft Sentinel analytics → Incident 4; and Windows Defender for Endpoint sensor → Defender XDR → Incident 3. These are **two separate pipelines** even though the Microsoft Defender portal can surface both.

**Management/control:** Azure Arc manages/onboards the non-Azure VM; DCR configures AMA collection. Neither is an independent event-storage destination.

**Local evidence only:** Sysmon and Wireshark were inspected on the Windows VM. Their cloud ingestion was **not** validated. These appear separately from Sentinel and Defender cloud feeds.

**Network model:** VMnet1 Host-only (`192.168.128.0/24`) connects the two VMs for authorized testing; Windows also used VMnet8 NAT (`192.168.144.0/24`) when controlled outbound/cloud connectivity was required. No bridged attack network or unsolicited-inbound NAT port forwarding was documented. The physical host and home LAN were **not** authorized targets.

**Historical status:** The Azure subscription was disabled after free-credit expiration in November 2026. The diagram describes verified historical implementation; present-day services must not be inferred from it.
