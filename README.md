# PortusSophia™ Lab Node

**Domain:** `lab.portussophia.com`
**Purpose:** Governance & Engineering operational workspace
**Classification:** Governance + Engineering Layer
**Tone:** Technical, cold, structure-only

---

## Repository Structure

```
/
├── _config.yml                    # Jekyll config
├── index.md                       # Lab overview
├── CNAME                          # Custom domain
├── README.md                      # This file
│
├── governance/
│   ├── standards/                 # PS-STD documents
│   │   ├── PS-STD-001_UICH.md
│   │   ├── PS-STD-060_Governance_Documentation.md
│   │   └── PS-STD-140_Repository_Topology.md
│   │
│   ├── witnesses/                 # LOGOS/DRACO templates
│   │   ├── logos-witness-template.md
│   │   └── draco-witness-template.md
│   │
│   ├── cycles/                    # Stewardship workflows
│   │   └── stewardship-cycle-template.md
│   │
│   ├── appeals/                   # Structural appeal templates
│   │   └── appeal-template.md
│   │
│   └── webkernel-topology.md     # PS-WEB-TOPOLOGY v1.0
│
├── engineering/
│   ├── ci/                        # CI workflows
│   │   ├── hash-generation.md
│   │   ├── uich-validation.md
│   │   └── drift-scanning.md
│   │
│   ├── scripts/                   # Validation tools
│   │   └── validation-tools.md
│   │
│   └── diagnostics/               # Drift models, risk maps
│       ├── boundary-checks.md
│       ├── drift-analysis.md
│       └── risk-mapping.md
│
└── recipes/                       # WebKernel engineering recipes
    └── node-activation-recipe.md
```

---

## Deployment Instructions

### Step 1: Create Repository

```powershell
gh repo create portussophia/portussophia-lab --public --description "PortusSophia™ Lab — Governance & Engineering operational workspace. Standards, witness cycles, CI workflows, structural integrity enforcement." --homepage "https://lab.portussophia.com"
```

### Step 2: Push Content

```powershell
# From this directory (site-public/lab-node/)
git init
git add .
git commit -m "Activate Lab Node — Governance & Engineering layer, Boundary (𝓑) secured"
git branch -M main
git remote add origin https://github.com/portussophia/portussophia-lab.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

In repository settings:
1. Navigate to **Settings → Pages**
2. Set **Source:** Deploy from branch `main` → `/ (root)`
3. Set **Custom domain:** `lab.portussophia.com`
4. Click **Save**
5. Wait ~5 minutes for GitHub to generate SSL certificate

### Step 4: Configure Cloudflare DNS

In Cloudflare dashboard for `portussophia.com` zone:

1. Navigate to **DNS**
2. Add or update record:
   - **Type:** CNAME
   - **Name:** `lab`
   - **Target:** `portussophia.github.io`
   - **TTL:** Auto
   - **Proxy:** DNS only (gray cloud) — for initial debugging
3. Delete any conflicting A records for `lab` subdomain

### Step 5: Configure Cloudflare SSL/TLS

In Cloudflare dashboard:
1. Navigate to **SSL/TLS → Overview**
2. Set **Mode:** Full (not Flexible)
3. Navigate to **SSL/TLS → Edge Certificates**
4. Ensure **Always Use HTTPS:** ✅ On
5. Ensure **Minimum TLS Version:** 1.2

### Step 6: Verify Deployment

```powershell
# Test DNS propagation
nslookup lab.portussophia.com

# Expected: CNAME → portussophia.github.io → A records

# Test HTTP response (wait 5-10 minutes for propagation)
curl -I https://lab.portussophia.com

# Expected: 200 OK
```

---

## Content Guidelines (Strictest Boundary Enforcement)

### ✅ Allowed Content

- Governance standards (PS-STD documents)
- Engineering specifications
- Witness cycle templates (LOGOS, DRACO)
- CI workflows and automation
- Topology documentation
- Diagnostics and drift analysis
- Stewardship procedures
- System recipes

### ❌ Prohibited Content

**Per PS-GOV-LAB-NODE-REQUEST v1.0, this node MUST NOT include:**

- Canon artifacts (PS-CAN documents hosted elsewhere, referenced externally only)
- Narrative content (personal, emotional, historical)
- Founder identity content (resume, statements, personal reflections)
- Public orientation content (belongs to Public Node)
- Academic research essays (belongs to MIT Node)
- Interpretive/meaning-making narratives
- Any Sara-layer output unless governance-neutral

**Principle:**
This node is a **cold workspace**—structure, not story.

---

## Boundary Constraints (𝓑)

**PortusNexus™ Alignment:**
- **N₆ (Constraint):** Lab Node enforces constraints, does not interpret meaning
- **N₇ (Non-Totalization):** Lab Node serves governance, does not elevate above Founder authority

**Navigation Constraints:**
- ✅ Lab → MIT (research ↔ engineering)
- ✅ Lab → Public (optional footer: "For Developers")
- ✅ Lab → Main domain (global header)
- ❌ Lab → Founder (no narrative bleed)
- ❌ Lab → Private Archive (no access)
- ❌ Lab → Canon directly (references only)

**Upward Drift Prevention:**
Lab Node must not self-elevate or position governance above Founder authority.

---

## Maintenance

**Owner:** PeterGate (Governance Steward)
**Content Stewards:**
- LOGOS (structural standards)
- DRACO (risk diagnostics)
- PeterGate (CI workflows, engineering specs)

**Approval Authority:** Founder (all content changes require Founder approval)

**Update Process:**
1. Draft governance/engineering content locally
2. Review for Boundary compliance (no Canon/Narrative/Founder identity)
3. Submit to LOGOS structural review (if standard/template)
4. Obtain Founder approval
5. Commit and push to `main` branch
6. Verify deployment at `lab.portussophia.com`

---

## Governance Compliance

**Classification:** Governance + Engineering Layer
**Distribution:** Controlled Access (public repo, technical audience)
**Boundary Status:** ✅ Verified (strictest boundaries enforced)
**Trademarks:** All PortusSophia™ trademark entities include ™ symbol
**Controlled Lexical Element:** *"Here and Now!"* (if referenced, exact format required)

---

## Status

**Node Status:** Pending Deployment
**Last Updated:** 2025-12-04
**Files Generated:** Core structure (index, governance placeholders, engineering placeholders)
**Files TODO:** Populate governance/standards/, witnesses/, cycles/, appeals/, engineering/ci/, diagnostics/, recipes/

**Next Actions:**
1. Create `portussophia-lab` repository
2. Generate seed documents (PS-STD-001, witness templates, CI workflows)
3. Push content to repository
4. Enable GitHub Pages with custom domain `lab.portussophia.com`
5. Configure Cloudflare DNS (CNAME: `lab` → `portussophia.github.io`)
6. Configure Cloudflare SSL/TLS (Mode: Full)
7. Verify deployment
8. Update WebKernel Topology Map
9. Update Navigation Map
10. Record activation in Golden Trace

---

## Golden Trace Entry (Draft)

Upon successful deployment, record:

**Event:** Lab Node Activation
**Golden Trace ID:** GOLDEN-TRACE-0005 (pending)
**Comment:** "Lab Node established; governance and engineering layers online with Boundary (𝓑) secured."
**Validation:**
- Zero Canon hosting: ✅ Verified (references only)
- Zero Narrative bleed: ✅ Verified
- Zero Founder identity: ✅ Verified
- Strictest boundary enforcement: ✅ Verified
- N₆/N₇ alignment: ✅ Verified
- Clean layer separation: ✅ Verified

---

**PortusSophia™** — Governance-first architecture, preserved in *"Here and Now!"*
