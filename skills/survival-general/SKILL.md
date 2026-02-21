---
name: survival-general
description: >
  Analyze, draft, and review Survival clauses for General contracts.
  Use when the user mentions survival clause, surviving provisions, post-termination obligations, or asks to review, redline,
  or generate this clause type. Returns structured risk assessment,
  plain-language summary, and suggested alternative language.
---

# Survival Clause -- General

This skill provides expert-level analysis and drafting assistance for
**Survival** clauses in **General** contracts.

---

## When to Activate

Activate this skill when the user:

- Uploads or pastes a contract containing a Survival clause
- Asks to **draft**, **redline**, or **improve** a Survival clause
- Asks for a **risk assessment** of an existing Survival provision
- Mentions keywords: *survival clause, surviving provisions, post-termination obligations*

---

## Workflow

### Step 1 -- Intake

Ask the user (if not already provided):

1. **Which party** are you representing? *(e.g., vendor, client, buyer, seller)*
2. **Jurisdiction** governing the contract? *(e.g., New York, California, England & Wales)*
3. **Is this a draft for review or should I generate fresh language?**

### Step 2 -- Analysis

If reviewing existing language, output the following structure:

```
## Survival Clause Analysis

### Plain-Language Summary
[2-3 sentence plain-English description of what the clause does]

### Key Provisions Identified
- [Provision 1]
- [Provision 2]

### Risk Assessment
| Item | Risk Level | Notes |
|------|-----------|-------|
| [item] | High / Medium / Low | [explanation] |

### Recommended Redlines
[Specific suggested changes with rationale]

### Market Standard Comparison
[How this clause compares to typical General market standard]
```

### Step 3 -- Drafting

If generating new language, produce:

1. **Balanced version** (neither party-favored)
2. **Favorable to client** version
3. **Negotiation notes** -- what the other side will likely push back on

---

## Survival Playbook -- General

> See `scripts/playbook.md` for detailed clause-specific guidance,
> fallback positions, jurisdiction-specific notes, and precedent language.

---

## Important Notes

- Always caveat that output is not legal advice and should be reviewed by qualified counsel.
- Flag any provisions that may be unenforceable or jurisdiction-specific.
- When jurisdiction is unknown, apply general common-law principles and note assumptions.
