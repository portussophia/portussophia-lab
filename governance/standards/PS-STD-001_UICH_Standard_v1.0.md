---
uid: "PS-STD-001"
title: "Universal Inter-Canon Header (UICH) Standard"
version: "v1.0"
classification: "Governance Standard — Structural"
author: "Founder"
custos: "PeterGate (Governance Steward)"
status: "Draft-Operational"
canonical_path: "/governance/standards/PS-STD-001_UICH_Standard_v1.0.md"
---

# PS-STD-001 — Universal Inter-Canon Header (UICH) Standard

## 1. Purpose

Define a **universal header block** for all PortusSophia™ artifacts so that:
- every file is self-identifying,
- governance can locate and classify artifacts reliably,
- integrity and lineage can be traced across all nodes (public, MIT, lab, founder).

## 2. Scope

Applies to:
- all Canon documents,
- all Governance artifacts,
- all WebKernel-facing specs,
- all Witness, Stewardship, and Appeal templates.

## 3. Required Header Fields

Every governed document MUST include at minimum:

- `uid` — unique identifier
- `title`
- `version`
- `author`
- `custos` (if applicable)
- `date_generated_utc` or `last_updated_utc`
- `canonical_path`
- `classification`
- `distribution`
- `integrity` block (if hashed)

## 4. YAML Placement

- Header MUST appear at top of file.
- Header MUST be valid YAML wrapped in `---` fences.
- No textual content may precede the header.

## 5. Integrity

When a file is sealed:
- `integrity.sha256_canonical` MUST be populated.
- `integrity.sealed_utc` MUST be recorded.

(Details of sealing process are covered by PS-STD-060.)

## 6. Compliance

Any file without a valid UICH header:
- may not be treated as Canon or Governance,
- may not be referenced in Golden Trace without remediation.
