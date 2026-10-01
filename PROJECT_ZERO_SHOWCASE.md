# PROJECT ZERO — Red-Team CTF Showcase

PROJECT ZERO is an original **boot-to-root cybersecurity training lab** I designed and built to practice offensive-security methodology in a controlled, self-owned environment.

The full repository stays private because it contains the author solution, lab credentials, flags, and exact exploitation details. This public overview intentionally excludes those spoilers.

## What I built

- A headless **Debian** target VM on **QEMU/KVM + libvirt**
- A dedicated isolated lab network for attacker ↔ target traffic
- A custom **Apache/PHP** web application with an intentionally designed multi-stage attack path
- A reproducible provisioning workflow so the target can be rebuilt from a clean system
- A separate Kali attacker VM used to validate the complete chain
- Documentation for architecture, reset/recovery, intended vulnerabilities, and isolation controls

## High-level attack chain

```text
Reconnaissance
      ↓
Web discovery / authentication weakness
      ↓
Authenticated web exploitation
      ↓
Low-privilege web foothold
      ↓
Credential discovery and offline analysis
      ↓
Local user pivot
      ↓
Custom Linux privilege-escalation path
      ↓
root
```

The exact credentials, flags, vulnerable code paths, and privilege-escalation solution are intentionally omitted from this public version.

## Environment

```text
Omarchy / Arch-based host
        │
        ├── Kali attacker VM
        │     └── isolated lab NIC
        │
        └── Debian target VM (mr-axe)
              ├── isolated lab NIC
              └── maintenance NIC used only for provisioning/administration
```

The maintenance and Internet-facing links are disabled during active attack testing so intentionally vulnerable services remain inside the controlled lab.

## Skills demonstrated

- Linux administration and permissions
- QEMU/KVM and libvirt networking
- Network isolation design
- Web reconnaissance and enumeration
- Authentication-security concepts
- Web exploitation concepts
- Shell access and Linux enumeration
- Credential discovery and offline password analysis
- Linux privilege escalation
- Bash automation and reproducible provisioning
- Git-based lab documentation
- Offensive-security lab design

## Connected blue-team work

PROJECT ZERO also became the attack source for my public **Wazuh SOC Lab**. Instead of keeping the offensive and defensive work separate, I used attacks against this target to generate real telemetry, build detections, identify monitoring gaps, and validate custom Wazuh/Suricata detection content.

That creates the first two parts of my portfolio pipeline:

```text
PROJECT ZERO CTF          Wazuh SOC Lab          AI SOC Bot
     attack        →          detect       →       automate
```

- [Wazuh SOC Lab](https://github.com/Alexander-Remnitz/wazuh-soc-lab)
- [AI SOC Bot](https://github.com/Alexander-Remnitz/ai-soc-bot)

## Safety note

All offensive testing is performed only against systems I own inside the dedicated lab environment. The deliberately vulnerable target is not intended for exposure to public or untrusted networks.
