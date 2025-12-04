---
uid: "PS-WEB-TOPOLOGY"
title: "WebKernel Topology Specification"
version: "v1.0"
classification: "Governance Spec — Topology"
author: "Founder"
custos: "PeterGate"
canonical_path: "/governance/webkernel/PS-WEB-TOPOLOGY_v1.0.md"
---

# WebKernel Topology Specification (PS-WEB-TOPOLOGY v1.0)

## 1. Purpose

Define the four-site ecosystem:

1. `portussophia.com` — Public Orientation Node
2. `mit.portussophia.com` — Academic / Research Node
3. `lab.portussophia.com` — Engineering & Governance Node
4. `founder.portussophia.com` — Professional Identity Node

## 2. Audience Mappings

| Node | Primary Audience | Secondary Audience | Content Tone |
|------|------------------|-------------------|--------------|
| **portussophia.com** | General public, friends, family | Philosophical readers | Accessible, high-level, orientation |
| **mit.portussophia.com** | Academic, institutional review | Researchers, peer reviewers | Formal, research-focused, zero narrative |
| **lab.portussophia.com** | Stewards, engineers, auditors | Developers, institutional reviewers | Technical, cold, structure-only |
| **founder.portussophia.com** | Professional contacts, collaborators | Media, institutional partners | Professional, direct, auditable |

## 3. Content Restrictions

### portussophia.com (Public Orientation Node)

**Allowed:**
- High-level architecture overviews
- Non-technical explanations of principles
- Public announcements and milestones
- Orientation summaries
- Navigation to other nodes

**Prohibited:**
- Canon documents (reserved for main site canonical layer)
- Governance artifacts (witness cycles, integrity seals)
- Internal deliberation records
- Private narrative or personal history
- Academic research details (reserved for MIT node)

---

### mit.portussophia.com (Academic / Research Node)

**Allowed:**
- Research artifacts and formal methods documentation
- Governance architecture documentation
- Witness cycle methodologies
- Integrity ledger examples (Golden Trace)
- Postulates and formal constraints (PortusNexus™ N₁–N₇)
- Academic citations and references

**Prohibited:**
- Personal narrative or Founder biographical details
- Public orientation content (reserved for public node)
- Internal deliberation records
- Funding vector or commercial information
- Interpretive WebKernel narratives

---

### lab.portussophia.com (Governance & Engineering Node)

**Allowed:**
- Governance standards (PS-STD series)
- Witness templates (LOGOS, DRACO)
- CI workflows and automation specs
- Engineering specifications
- Topology documentation
- Diagnostics, drift analysis, risk mapping
- Stewardship procedures

**Prohibited:**
- Canon artifacts (references only, no hosting)
- Personal narrative (emotional, historical content)
- Founder identity content (resume, statements)
- Public orientation content (belongs to public node)
- Academic research essays (belongs to MIT node)
- Interpretive/meaning-making narratives

---

### founder.portussophia.com (Professional Identity Node)

**Allowed:**
- Professional identity and background
- Mission and vision statements
- Problem statement and institutional context
- **Institutional Genesis document** (exclusive to this node)
- Resume / CV
- Professional portfolio
- Contact information for professional inquiries

**Prohibited:**
- Canon artifacts (reserved for main site)
- Governance artifacts (witness cycles, risk assessments)
- Golden Trace entries (external links only)
- Internal narrative (raw, private, vulnerable content)
- Funding vector or commercial details
- Lab materials (governance standards, CI workflows)

---

## 4. Navigation Rules

### Allowed Navigation Paths

- **Public → MIT** (research references)
- **Public → Founder** (professional identity)
- **Public → Main Site** (canonical content)
- **MIT → Public** (orientation summaries)
- **MIT → Main Site** (canonical references)
- **Lab → MIT** (research ↔ engineering)
- **Lab → Public** (optional footer: "For Developers")
- **Lab → Main Site** (global header)
- **Founder → Public** (orientation)
- **Founder → MIT** (research)
- **Founder → Main Site** (canonical content)

### Prohibited Navigation Paths

- **Public → Canon** (no direct access to immutable content)
- **Public → Governance** (no navigation to witness cycles)
- **MIT → Private Archive** (boundary separation)
- **Lab → Founder** (no narrative bleed)
- **Lab → Private Archive** (no access)
- **Lab → Canon directly** (references only)
- **Any upward drift** that self-elevates governance above Founder authority

---

## 5. Change Control

All topology modifications MUST:

1. Be submitted as a governance request (PS-GOV format)
2. Include drift analysis (boundary impact assessment)
3. Pass Ratio–Fides witness check when applicable
4. Obtain Governance Steward (PeterGate) approval
5. Be logged in Golden Trace ledger

**Change Types:**

- **Minor:** Clarifications, typo fixes, formatting (no witness required)
- **Moderate:** Content restriction updates, navigation changes (LOGOS witness required)
- **Major:** Node purpose changes, audience remapping (LOGOS + DRACO witness required)

---

## 6. Compliance

**Node Activation Requirements:**

Each node MUST:
- Have dedicated GitHub repository
- Include CNAME file with custom domain
- Enable GitHub Pages (main branch, root folder)
- Configure Cloudflare DNS (CNAME record)
- Pass boundary compliance check
- Receive Golden Trace activation entry

**Ongoing Compliance:**

- Quarterly topology audits
- Drift detection via CI workflows
- Boundary violation alerts routed to PeterGate
- Annual LOGOS structural review

---

## 7. Metadata

**Version History:**
- v1.0 (2025-12-04): Initial four-node topology specification

**Related Standards:**
- PS-STD-001 (UICH Standard)
- PS-STD-060 (Governance Documentation)
- PS-STD-140 (Repository Topology)

**Stewardship:**
- Author: Founder
- Custos: PeterGate (Governance Steward)
- Witnesses: LOGOS (structural), DRACO (boundary risk)
