# Hi, I'm Alex 👋

Self-taught **cybersecurity** learner based in Tbilisi, Georgia — focused on
blue-team / SOC skills, detection engineering, and practical home-lab work.

I learn by building complete, connected systems rather than isolated exercises.
My main project is a full **attack → detect → automate** pipeline, built from
scratch on a QEMU/KVM home lab:

## 🔗 Featured projects

### 🛡️ [wazuh-soc-lab](https://github.com/Alexander-Remnitz/wazuh-soc-lab) — *detect*
A home SOC built on **Wazuh** (SIEM/XDR). Detects five attack types launched
from Kali against an isolated vulnerable target — port scan, SSH brute force,
web directory brute force, file-integrity tampering, and a **custom detection
rule** I wrote and validated myself — all mapped to MITRE ATT&CK, with
dashboard evidence and honest troubleshooting notes.

`Wazuh` · `SIEM` · `detection engineering` · `MITRE ATT&CK` · `Ubuntu` · `libvirt`

### 🤖 [ai-soc-bot](https://github.com/Alexander-Remnitz/ai-soc-bot) — *automate*
A **local, private AI** that triages the Wazuh alerts above using an on-device
LLM via **Ollama** — no cloud, no API keys, no data leaving the machine. Pulls
alerts over an SSH tunnel, groups duplicates, and produces a structured triage
(summary, severity, false-positive check, next step) as a report.

`Python` · `Ollama` · `local LLM` · `security automation` · `SSH tunnelling`

### ⚔️ Red-team CTF lab — *attack* (private)
An original boot-to-root CTF target I designed and built (web foothold →
privilege escalation → root), used as the "attacker's-eye" side of the pipeline
above. Kept private so it isn't spoiled.

## 🧰 Tools & focus

`Wazuh` · `Kali Linux` · `QEMU/KVM · libvirt` · `Linux (Arch / Debian / Ubuntu)` ·
`Python` · `Bash` · `Git` · `Ollama` · `MITRE ATT&CK` · `detection engineering`

## 🌱 Currently

Deepening blue-team skills and growing the home lab. Open to learning,
collaboration, and SOC-analyst opportunities.
