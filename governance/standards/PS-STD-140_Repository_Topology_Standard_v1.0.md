---
uid: "PS-STD-140"
title: "Repository Topology Standard"
version: "v1.0"
classification: "Governance Standard — Topology"
author: "Founder"
custos: "PeterGate (Governance Steward)"
status: "Draft-Operational"
canonical_path: "/governance/standards/PS-STD-140_Repository_Topology_Standard_v1.0.md"
---

# PS-STD-140 — Repository Topology Standard

## 1. Purpose

Define how PortusSophia™ content is distributed across:
- `portussophia.com` (Public)
- `mit.portussophia.com` (Academic)
- `lab.portussophia.com` (Governance & Engineering)
- `founder.portussophia.com` (Professional Identity)

## 2. Topology Rules

- Each subdomain MUST correspond to one GitHub repo.
- Each repo MUST include a UICH-compliant topology or manifest file.
- Content classification MUST respect node-specific restrictions.

## 3. Change Control

Any topology change MUST:
1. be submitted as a governance request,
2. include a drift analysis,
3. pass Ratio–Fides witness check when applicable,
4. obtain Governance Steward approval,
5. be logged in Golden Trace.

## 4. Node-Specific Restrictions

### portussophia.com (Public Orientation)

**Allowed:**
- High-level architecture overviews
- Non-technical explanations
- Public announcements
- Orientation summaries

**Prohibited:**
- Canon documents
- Governance artifacts
- Internal witness cycles
- Private narrative
- Academic research details

### mit.portussophia.com (Academic / Research)

**Allowed:**
- Research artifacts
- Formal methods documentation
- Integrity ledger examples
- Postulates and constraints
- Witness cycle methodologies

**Prohibited:**
- Personal narrative
- Founder identity content
- Internal deliberation records
- Funding vector information

### lab.portussophia.com (Governance & Engineering)

**Allowed:**
- Governance standards
- Witness templates
- CI workflows
- Engineering specifications
- Topology documentation
- Diagnostics and risk analysis

**Prohibited:**
- Canon artifacts (references only)
- Personal narrative
- Founder identity content
- Public orientation content
- Academic research essays
- Interpretive/meaning-making narratives

### founder.portussophia.com (Professional Identity)

**Allowed:**
- Professional identity and background
- Problem statement
- Institutional Genesis document (exclusive)
- Mission and vision
- Resume/CV
- Professional portfolio

**Prohibited:**
- Canon artifacts
- Governance artifacts
- Golden Trace entries (external links only)
- Internal narrative (raw, private)
- Funding vector details
- Lab materials
