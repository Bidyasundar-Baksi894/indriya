# Indriya — India Go-To-Market (GTM) Strategy

To scale Indriya in India, you need to target the sectors where human employees process massive volumes of AI-assisted tasks, and where the regulatory/financial cost of an error is devastating. 

Here is the exact playbook for scaling in the Indian market.

---

## 1. The Target Sectors (Who will buy this?)

### Tier 1: BFSI (Banking, Financial Services, and Insurance)
*   **Target Companies:** HDFC, ICICI, SBI, Bajaj Finserv, Muthoot Finance.
*   **The Use Case:** Indian banks have rapidly moved from manual credit checks to AI-driven Loan Origination Systems (LOS) that process alternative data (UPI, GST records). 
*   **The Problem:** RBI's new **FREE-AI Framework** mandates human oversight for credit decisions. Banks hire thousands of back-office analysts to review the AI's loan decisions. Under pressure to meet turnaround times (TAT), these analysts suffer from automation bias, blindly approving AI credit scores without reading the supporting documents.
*   **Why they buy:** To prove to the RBI that their human oversight is real, not just a rubber stamp.

### Tier 2: Indian IT Services & Consulting Giants
*   **Target Companies:** TCS, Infosys, Wipro, HCLTech, Tech Mahindra.
*   **The Use Case:** These companies have deployed massive internal AI tools (e.g., Wipro's ai360, Infosys Topaz) and over 300,000 Microsoft Copilot licenses to their developers and consultants.
*   **The Problem:** They are shifting to "outcome-based pricing" (getting paid for the work done, not the hours billed). If a Wipro developer blindly trusts AI-generated code that contains a security flaw, Wipro is liable. 
*   **Why they buy:** To enforce quality control at scale. Indriya acts as a guardrail ensuring their 500,000+ employees aren't just copy-pasting AI outputs without critical review.

### Tier 3: Global Capability Centers (GCCs) & BPOs
*   **Target Companies:** Genpact, EXL, WNS, and internal GCCs for global banks (e.g., J.P. Morgan India, Goldman Sachs Bengaluru).
*   **The Use Case:** Processing insurance claims, fraud alerts, and customer service tickets using AI triage.
*   **Why they buy:** They operate on strict SLAs and Average Handling Time (AHT) metrics. Indriya prevents the "Speed Paradox" where agents click too fast just to hit their daily targets.

---

## 2. The Deployment Workspaces (Where does Indriya sit?)

Indriya does not require companies to switch software. It sits as a silent layer on top of the tools they already use. In India, you will deploy the **Indriya Browser Extension** to monitor these three dominant platforms:

| The Workspace | Who Uses It in India | What Indriya Monitors |
|---------------|----------------------|-----------------------|
| **Salesforce** | Almost all large Indian enterprises (Tata Capital, Mahindra). | AI Lead Scoring, Next-Best-Action recommendations. Indriya tracks if salespeople are actually reading lead context before acting. |
| **ServiceNow** | The backbone of Indian IT giants (TCS, Infosys) for IT and HR ticketing. | AI ticket routing and resolution suggestions. Indriya tracks if L1 support agents are blindly applying AI fixes to critical servers. |
| **Custom Web Portals** | Indian Banks (HDFC, SBI) use proprietary web-based Loan Origination Systems (LOS). | AI credit approvals. Indriya forces a "Speed Gate" if an underwriter approves a high-risk loan in under 2 seconds. |

---

## 3. How to Pitch to TCS, Infosys, and Wipro

When you speak to a partner at an Indian IT giant, here is your exact pitch:

> *"You just deployed 100,000 Copilot licenses and built your own AI platforms like Infosys Topaz. Your developers are generating code 30% faster.* 
> 
> *But here is your new risk: **Automation Bias**. Your junior developers are trusting the AI too much. They are copy-pasting code and approving AI architectural suggestions without reading them. When that code breaks a client's system, your firm is liable.*
> 
> *Indriya is an Endpoint Behavioral Agent. We deploy via a silent browser extension. We monitor the speed and behavior of your developers when they interact with Topaz or Copilot. If a developer accepts 5 complex AI code suggestions in under 10 seconds, Indriya pops up and forces them to justify the decision.*
> 
> *We don't audit the code. **We audit the human.** We ensure your workforce remains critical thinkers, not just AI rubber-stamps."*

---

## 4. The GTM Action Plan

1. **Start with SOCs (Security Operations Centers):** The easiest initial sale. Cybersecurity teams in India already know they have an "Alert Fatigue" crisis. Sell the Micro-Simulation engine to CISO's to test their analysts.
2. **Expand to BFSI Back-Offices:** Use the RBI regulatory angle. Pitch Indriya to Chief Risk Officers at NBFCs (Non-Banking Financial Companies) like Bajaj Finserv.
3. **Enterprise Wide:** Once proven, pitch to CIOs as a mandatory governance layer for all enterprise AI tools (Salesforce, Copilot, etc.).
