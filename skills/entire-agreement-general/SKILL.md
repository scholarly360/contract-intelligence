---
name: entire-agreement-general
description: >
  Confirms that the written contract is the complete and final understanding, superseding all prior discussions and agreements.
  Prevents either party from relying on verbal promises, emails, or earlier drafts not included in the signed document.
---

# Entire Agreement Clause -- General

This skill provides expert-level analysis and drafting assistance for
**Entire Agreement** clauses in **General** contracts.

---

## When to Activate

Activate this skill when the user:

- Uploads or pastes a contract containing a Entire Agreement clause
- Asks to **draft**, **redline**, or **improve** a Entire Agreement clause
- Asks for a **risk assessment** of an existing Entire Agreement provision
- Mentions keywords: *entire agreement, integration clause, merger clause*

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
## Entire Agreement Clause Analysis

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

## Entire Agreement Playbook -- General

> See `scripts/playbook.md` for detailed clause-specific guidance,
> fallback positions, jurisdiction-specific notes, and precedent language.

---

## Important Notes

- Always caveat that output is not legal advice and should be reviewed by qualified counsel.
- Flag any provisions that may be unenforceable or jurisdiction-specific.
- When jurisdiction is unknown, apply general common-law principles and note assumptions.
