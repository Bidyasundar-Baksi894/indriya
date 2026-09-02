# Indriya v2.0 — Endpoint Behavioral Security Agent

## What Indriya Actually Is

Indriya is **not** a standalone dashboard. It is an **Endpoint Behavioral Agent** — a lightweight software agent installed on every workstation in an enterprise. It runs silently in the background and hooks into whatever AI-powered tools the employee uses.

Think of it as:
- **CrowdStrike** monitors the machine for malware → **Indriya** monitors the human for cognitive bias
- **Grammarly** sits in background and checks your writing → **Indriya** sits in background and checks your thinking
- **IT Phishing Tests** send fake emails to test security awareness → **Indriya** sends fake AI outputs to test cognitive awareness

### How It Works (Technically)
```
┌─────────────────────────────────────────────────┐
│              EMPLOYEE WORKSTATION                │
│                                                  │
│  ┌──────────┐  ┌──────────┐  ┌──────────────┐   │
│  │Salesforce│  │  Splunk  │  │Bloomberg Term│   │
│  │  (CRM)   │  │  (SIEM)  │  │  (Trading)   │   │
│  └────┬─────┘  └────┬─────┘  └──────┬───────┘   │
│       │              │               │           │
│  ┌────▼──────────────▼───────────────▼───────┐   │
│  │         INDRIYA AGENT (Background)        │   │
│  │  • Tracks clicks, approvals, rejections   │   │
│  │  • Measures response velocity             │   │
│  │  • Injects micro-simulation traps         │   │
│  │  • Triggers cognitive friction guardrails  │   │
│  └────────────────────┬──────────────────────┘   │
│                       │                          │
└───────────────────────┼──────────────────────────┘
                        │ (encrypted telemetry)
                        ▼
            ┌───────────────────────┐
            │  INDRIYA CLOUD / HQ   │
            │  (Admin Dashboard)    │
            │  • Command Center     │
            │  • Team Analytics     │
            │  • Compliance Reports │
            └───────────────────────┘
```

---

## The Three Pillars (Unchanged)

### Pillar 1: Passive Monitoring
The agent silently hooks into AI-powered tools and tracks:
- **Override Rate** — how often a human rejects an AI suggestion
- **Response Velocity** — how fast they approve (too fast = blind trust)
- **Pattern Drift** — behavioral changes over time (Monday vs Friday fatigue)

### Pillar 2: Micro-Simulations ("Cognitive Phishing")
The agent occasionally injects **fake AI outputs** into the employee's real workflow:
- A deliberately flawed AI recommendation to see if they catch it
- A high-confidence false positive to test blind trust
- A low-confidence true positive to test alert fatigue
- The employee never knows which outputs are real and which are tests

### Pillar 3: Automated Guardrails ("Cognitive Friction")
When the agent detects dangerous behavior, it automatically intervenes:
- **Speed Gate** — If approval < 3s, force a "Type your reasoning" popup
- **Confidence Override** — If rejecting a Critical alert, require co-sign
- **Fatigue Break** — If fatigue index > 80, trigger mandatory micro-break

---

## Updated Dashboard Architecture (8 Pages)

### ★ NEW: Page 0 — Employee Workstation Simulator
**This is the centerpiece of the entire demo.**

A full-screen simulated employee workstation showing a fake Salesforce-style AI tool. The employee is reviewing AI-generated lead scores and approving/rejecting them.

**What happens during the demo:**
1. You (as the presenter) play the role of the employee
2. The screen looks like a normal CRM / SIEM tool — no sign of Indriya anywhere
3. You start approving AI suggestions quickly (clicking approve, approve, approve...)
4. After 4-5 rapid approvals, the screen subtly dims and an **Indriya Guardrail Overlay** slides in from the bottom:
   > 🛡️ **Indriya Cognitive Friction Activated**
   > "You approved 5 AI recommendations in 8 seconds.
   > Response velocity: 1.6s avg (threshold: 3.0s)
   > Please type your reasoning for the last approval to continue."
5. You type a reason and hit submit. The overlay disappears. Normal work resumes.
6. At one point, a **Micro-Simulation Trap** is silently injected — a clearly wrong AI recommendation with high confidence. If you approve it blindly, Indriya logs it silently (no popup — the employee never knows it was a test).
7. You then say to the audience: "Now let me show you what the CISO sees..." and switch to the Admin Dashboard (Command Center), where all of this behavior is aggregated.

### Page 1: Login Screen
- Enterprise login with Indriya branding
- `demo@indriya.ai` / `rise2026`

### Page 2: Command Center (Home Dashboard)
- Live Threat Feed, 3 Pillar Status Cards, Org-Wide Risk Gauge, Alert Fatigue Trend
- *(Already built in Day 1)*

### Page 3: Passive Monitor
- Live Activity Stream, Override Rate Dashboard, Velocity Heatmap, Pattern Drift
- *(Already built in Day 1)*

### Page 4: Micro-Simulation Engine
- Trap Library, Deploy Trap button, Trap Results Feed, Catch Rate chart

### Page 5: Guardrails Control Panel
- Active Guardrails List, Live Intervention Log, Simulated Cognitive Friction

### Page 6: Analyst Deep-Dive
- Radar Chart, Behavioral Timeline, Trap History, Recommended Interventions

### Page 7: Reports & Compliance
- Executive Summary, EU AI Act, NIST AI RMF, Export PDF

---

## Updated 5-Day Build Schedule

| Day | Date | Focus | Deliverable |
|-----|------|-------|-------------|
| 1 | ~~Fri Aug 29~~ ✅ | ~~Login + Command Center + Passive Monitor~~ | ✅ Done |
| **2** | **Sat Aug 30** | **★ Employee Workstation Simulator** — the fake CRM/SIEM with live guardrail overlay and silent trap injection | The jaw-drop demo moment |
| **3** | **Sun Aug 31** | **Micro-Simulation Engine** — Trap Library, deploy traps, results feed, catch rate chart | Cognitive phishing control panel |
| **4** | **Mon Sep 1** | **Guardrails Control Panel + Analyst Deep-Dive** — togglable rules, intervention log, radar charts | Intelligence layer |
| **5** | **Tue Sep 2** | **Reports & Compliance + Final Polish** — EU AI Act, NIST, PDF export, presentation mode | Stage-ready |

> [!IMPORTANT]
> **Sep 3-5** reserved for rehearsal, bug fixes, and packing.

---

## Updated Pitch Flow (3 Minutes)

This is the new pitch sequence for the RISE Conclave:

| Time | What You Show | What You Say |
|------|--------------|-------------|
| 0:00-0:15 | Title slide | "Indriya is an endpoint behavioral agent. We install on every workstation and silently monitor how humans interact with AI." |
| 0:15-0:30 | Problem slide | "Companies lose millions because employees either blindly trust AI or ignore it." |
| **0:30-1:30** | **★ Employee Workstation Simulator** | "Let me show you. I'm an employee using Salesforce right now. Watch — I'll approve a few AI suggestions quickly..." *(click click click)* "...and Indriya just caught me." *(guardrail popup appears)* |
| 1:30-2:00 | Switch to Admin Dashboard | "Now let me show you what the CISO sees on their end..." *(show Command Center with all the data)* |
| 2:00-2:30 | Market + Business Model | "We charge per-seat. Every workstation with AI tools is our market." |
| 2:30-3:00 | The Ask | "Raising seed to validate and deploy." |

> [!IMPORTANT]
> The **Employee Workstation Simulator** (0:30-1:30) is the single most important minute of your entire pitch. This is where investors go from "interesting concept" to "I need to invest in this." It makes the invisible visible.
