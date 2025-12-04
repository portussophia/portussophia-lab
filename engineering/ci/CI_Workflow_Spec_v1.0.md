---
uid: "LAB-CI-0001"
title: "Lab CI Workflow Specification"
version: "v1.0"
classification: "Engineering Spec — CI"
author: "Founder"
custos: "PeterGate"
canonical_path: "/engineering/ci/CI_Workflow_Spec_v1.0.md"
---

# Lab CI Workflow Specification

## 1. Purpose

Define CI workflows for the Lab Node to:
- validate UICH headers,
- run drift scans,
- compute and verify hashes,
- check topology compliance,
- flag violations for governance review.

## 2. Pipelines

1. **uich-validate**
   - Checks all governed files for valid PS-STD-001 headers.

2. **hash-and-compare**
   - Generates SHA-256 and compares to recorded canonical values (if present).

3. **topology-check**
   - Confirms file placement aligns with PS-STD-140 / PS-WEB-TOPOLOGY.

4. **drift-scan**
   - Detects unexpected additions, removals, or relocations in critical directories.

## 3. Outputs

Each run must produce:
- machine-readable report (JSON/YAML),
- human-readable summary,
- clear exit codes (0 = ok, 1+ = advisory/failed).

## 4. Routing

- LOGOS receives structural issues.
- DRACO receives high-risk drifts.
- PeterGate receives governance violations.
- Founder receives any event affecting Canon integrity.
