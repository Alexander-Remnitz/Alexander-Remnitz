# Hi, I'm Alex

Self-taught **cybersecurity and AI practitioner** focused on hands-on security labs, red-team methodology, SOC/detection engineering, and local AI security automation.

I have studied cybersecurity and AI independently for several years and learn primarily by building complete, connected systems rather than isolated exercises. My current home-lab portfolio follows one pipeline:

## Attack → Detect → Automate

### ⚔️ [PROJECT ZERO CTF](PROJECT_ZERO_SHOWCASE.md) — *attack*
An original multi-stage boot-to-root CTF target I designed and built on **QEMU/KVM + libvirt**. It covers reconnaissance, web exploitation, a low-privilege foothold, credential analysis, a user pivot, and a custom Linux privilege-escalation path. The full author repository remains private to protect credentials, flags, and the solution; the linked showcase is spoiler-free.

`Kali Linux` · `Debian` · `Apache/PHP` · `Linux privilege escalation` · `libvirt` · `Bash`

### 🛡️ [wazuh-soc-lab](https://github.com/Alexander-Remnitz/wazuh-soc-lab) — *detect*
A home SOC built on **Wazuh** with attacks launched from Kali against the PROJECT ZERO target. The lab validates **six detection scenarios**, including SSH brute force, web directory brute force, realtime file-integrity monitoring, privileged activity, a custom Wazuh detection rule, and port-scan detection through **Suricata**. The work includes MITRE ATT&CK mapping, dashboard evidence, custom detection content, and troubleshooting notes.

A key part of this project was identifying that the host-based Wazuh agent could not directly see a raw SYN scan, then adding Suricata network telemetry and a custom signature to close that visibility gap.

`Wazuh` · `Suricata` · `SIEM` · `detection engineering` · `MITRE ATT&CK` · `Ubuntu` · `libvirt`

### 🤖 [ai-soc-bot](https://github.com/Alexander-Remnitz/ai-soc-bot) — *automate*
A **Python** security-automation tool that pulls Wazuh alerts over an SSH tunnel and uses a locally hosted **Ollama** model for structured Tier-1-style triage. Alert content remains inside the local lab environment rather than being sent to a third-party cloud LLM API. The bot groups duplicate events, validates structured model output, and produces terminal/Markdown reports.

`Python` · `Ollama` · `local LLM` · `security automation` · `Wazuh` · `SSH tunnelling`

## Tools & areas of focus

`Cybersecurity` · `Artificial Intelligence` · `Red Teaming` · `Penetration Testing` · `SOC` · `Detection Engineering` · `Wazuh` · `Suricata` · `Kali Linux` · `QEMU/KVM` · `libvirt` · `Linux (Arch / Debian / Ubuntu)` · `Python` · `Bash` · `Git` · `Ollama` · `MITRE ATT&CK`

## Current direction

I am continuing to develop practical cybersecurity and AI skills and am working toward my first professional opportunity in the industry. My strongest interests are offensive security/red-team work, detection engineering, and the intersection of AI with cybersecurity.
