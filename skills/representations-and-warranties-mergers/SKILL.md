---
name: representations-and-warranties-mergers
description: >
  Analyze, draft, and review Representations and Warranties clauses for Mergers contracts.
  Use when the user mentions reps and warranties, merger representations, or asks to review, redline,
  or generate this clause type. Returns structured risk assessment,
  plain-language summary, and suggested alternative language.
---

# Representations and Warranties Clause -- Mergers

This skill provides expert-level analysis and drafting assistance for
**Representations and Warranties** clauses in **Mergers** contracts.

---

## When to Activate

Activate this skill when the user:

- Uploads or pastes a contract containing a Representations and Warranties clause
- Asks to **draft**, **redline**, or **improve** a Representations and Warranties clause
- Asks for a **risk assessment** of an existing Representations and Warranties provision
- Mentions keywords: *reps and warranties, merger representations*

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
## Representations and Warranties Clause Analysis

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
[How this clause compares to typical Mergers market standard]
```

### Step 3 -- Drafting

If generating new language, produce:

1. **Balanced version** (neither party-favored)
2. **Favorable to client** version
3. **Negotiation notes** -- what the other side will likely push back on

---

## Representations and Warranties Playbook -- Mergers

> See `scripts/playbook.md` for detailed clause-specific guidance,
> fallback positions, jurisdiction-specific notes, and precedent language.

---

## Important Notes

- Always caveat that output is not legal advice and should be reviewed by qualified counsel.
- Flag any provisions that may be unenforceable or jurisdiction-specific.
- When jurisdiction is unknown, apply general common-law principles and note assumptions.
