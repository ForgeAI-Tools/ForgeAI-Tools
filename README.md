# Forge AI Tools

**Local AI, automation, security visibility, and operations engineering.**

Built by Michael Anderson — CompTIA Security+ Certified | AI Engineer in progress

---

## Overview

Forge AI Tools is a practical AI and automation lab focused on locally deployable systems, secure operations, infrastructure visibility, and AI-assisted workflows.

The project is built around a simple operating principle:

```text
Build useful tools. Secure the environment. Observe what matters. Automate carefully. Keep human authority in the loop.
```

Current development focuses on an AI-assisted operations stack that combines local services, security telemetry, workflow automation, and advisory LLM review.

---

## Core Systems

### Omnys

Omnys is the local operations and security visibility layer. It is designed to collect evidence, summarize system state, surface visibility gaps, and support human-reviewed operational workflows.

Current Omnys focus areas:

- Wazuh visibility checks
- UDM Pro / TheWall syslog visibility
- Local report and event artifact generation
- n8n workflow bridge integration
- Advisory handoff to Qwen
- Read-only security and operations observation

### Forge Server

Forge Server is the primary local application, automation, and AI services host. It supports project workloads, local scripts, service orchestration, and evidence collection.

Current Forge Server responsibilities:

- Local application hosting
- Automation workflows
- Omnys probes and reports
- Wazuh deployment support
- n8n workflow hosting
- Local infrastructure tooling

### TheWall

TheWall is the local network gateway and perimeter visibility source. It provides network-level telemetry and supports external SIEM forwarding into the Forge environment.

Current TheWall focus areas:

- Network gateway visibility
- Syslog forwarding
- UDM Pro event collection
- Security monitoring support
- Perimeter validation for approved local lab testing

### Qwen

Qwen is a local advisory LLM running through Ollama. It is used for human-reviewed operational summaries, investigation notes, and advisory response drafting.

Qwen guardrails:

- Advisory-only
- No trading authority
- No firewall authority
- No secret handling
- No direct remediation authority
- Human review required before action

### Shadow Ops

Shadow Ops is the controlled lab validation track for authorized visibility and detection testing. It exists to confirm that local monitoring, logging, and advisory workflows can observe approved test activity without disruption.

Shadow Ops is limited to owned local lab systems and does not include exploit attempts, credential testing, public IP scanning, wireless disruption, stealth, evasion, or unauthorized targets.

### Ops Console

Ops Console is the planned local operator command surface for dashboards, probe execution, event markers, response drafts, and status review.

The intended console model is fast access, not bypassed control. Buttons and shortcuts should trigger safe scripts, dashboards, markers, or draft-generation workflows only.

---

## Current Architecture

```text
UDM Pro / TheWall -> Forge rsyslog -> Omnys evidence path
Wazuh -> Omnys visibility probe -> local reports and events
Omnys -> n8n attention bridge -> Qwen advisory workflow
Human operator -> review, approve, document, and act
```

Core doctrine:

```text
Omnys observes.
Wazuh stores security events.
TheWall provides network telemetry.
n8n routes workflows.
Qwen advises.
Human approval remains required.
```

---

## Current Milestones

### Confirmed

- Wazuh services running on the Forge Server
- Wazuh alert evidence available locally
- Omnys Wazuh visibility probe operational
- Forge Server and local workstation telemetry visible in Wazuh sample window
- Omnys-to-n8n attention bridge operational
- UDM Pro / TheWall external SIEM forwarding confirmed
- UDM Pro CEF syslog routed into local Omnys evidence path

### In Progress

- UDM Pro / TheWall visibility probe
- Sensitive-field redaction for network telemetry summaries
- Omnys probe organization and module refactor
- Shadow Ops authorized visibility training checklist
- Ops Console macro keypad command surface design

---

## Featured Projects

### Professor Robin — AI-Powered Certification Tutor

Professor Robin is a voice-enabled AI tutoring assistant built with Flask, Ollama, Whisper, and text-to-speech support. It is designed to support active recall, certification study, and local AI-assisted learning workflows.

Key capabilities:

- Voice input through speech-to-text
- Voice output through text-to-speech
- Local LLM support through Ollama
- Browser-based Flask interface
- Tutor-style persona and structured study flow

### NEX — AI-Assisted Development Companion

NEX is a local AI-assisted development companion for system design, code generation, document analysis, and structured reasoning workflows.

Focus areas:

- Memory persistence
- File ingestion and summarization
- Structured reasoning responses
- Threaded UI interaction
- Engineering workflow support

### Om-Call — AI Communication Prototype

Om-Call is a multilingual AI communication prototype for real-time translation and call-center workflow simulation using generative AI and voice processing.

Focus areas:

- Translation workflows
- Voice simulation
- Communication support
- AI-assisted service desk concepts

### Gravity

Gravity is a private executive-assistant concept focused on task support, personal operations, and future AI-assisted productivity workflows.

---

## Security and Governance Principles

Forge AI Tools is designed around practical security boundaries:

- Read-only observation by default
- Human approval before remediation
- No credential testing outside authorized lab scope
- No public target scanning
- No automated firewall changes from advisory systems
- No secrets sent to advisory LLM workflows
- Local evidence remains local unless redacted
- Sensitive telemetry is summarized before advisory review

The long-term goal is to make the environment harder to discover, harder to misuse, easier to observe, and faster to recover.

---

## Technology Stack

### AI and Automation

- Python
- Flask
- Ollama
- Qwen models
- OpenAI Whisper
- pyttsx3
- n8n
- REST APIs

### Security and Infrastructure

- Wazuh SIEM
- UDM Pro / TheWall
- Syslog / rsyslog
- Linux services
- Bash
- PowerShell
- VLANs and VPN concepts

### Frontend and Interface Prototypes

- React
- TypeScript
- Vite
- Tailwind CSS
- Canvas API
- HTML / CSS

### Identity and Enterprise Concepts

- IAM / PAM concepts
- Okta
- SailPoint
- Microsoft Entra ID
- HIPAA, SOX, and NIST-aligned thinking

---

## Certifications

| Certification | Status |
| --- | --- |
| CompTIA Security+ (SY0-701) | Active 2025-2028 |
| Oracle Cloud Infrastructure AI Foundations | Active 2025-2027 |

---

## Project Status

Active development.

Current emphasis is on building a local AI-assisted operations and security visibility stack with disciplined guardrails, practical telemetry, human-reviewed advisory workflows, and professional documentation.

---

## Connect

- Website: [forgeai.tools](http://forgeai.tools)
- Email: michael@forgeai.tools
- LinkedIn: [Michael Anderson](https://www.linkedin.com/in/iammichaelanderson)
- GitHub: [ForgeAI-Tools](https://github.com/ForgeAI-Tools)

---

*Building the tools. Securing the systems. Automating the future.*
