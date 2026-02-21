# Contract Intelligence — Agent Skills

> **A collection of AI agent skills for analyzing, drafting, and reviewing contract clauses across industries.**

Install with:

```bash
npx skills add YOUR_GITHUB_USERNAME/contract-intelligence
```

Or install a single skill:

```bash
npx skills add YOUR_GITHUB_USERNAME/contract-intelligence@confidentiality-general
```

---

## Available Skills

| Skill | Description | Industry |
|-------|-------------|----------|
| `confidentiality-general` | Analyze & draft NDA / confidentiality clauses | General |
| `indemnification-general` | Analyze & draft indemnification provisions | General |
| `limitation-of-liability-general` | Assess and redline liability cap clauses | General |
| `termination-general` | Draft termination rights and cure periods | General |
| `force-majeure-general` | Review force majeure scope and exclusions | General |
| `governing-law-general` | Advise on choice of law and jurisdiction | General |
| `dispute-resolution-general` | Draft arbitration / mediation clauses | General |
| `representations-and-warranties-mergers` | M&A reps & warranties analysis | Mergers |
| `payment-terms-general` | Structure invoicing and payment schedules | General |
| `intellectual-property-ownership-technology` | IP assignment and work-for-hire analysis | Technology |
| `non-compete-employment` | Review and draft non-compete / NCA clauses | Employment |
| `assignment-general` | Assess assignability of contract rights | General |
| `entire-agreement-general` | Identify integration / merger clause issues | General |
| `severability-general` | Analyze severability and savings provisions | General |
| `notice-general` | Draft and review notice requirements | General |
| `amendment-general` | Advise on amendment formalities | General |
| `waiver-general` | Review waiver language and no-waiver clauses | General |
| `insurance-construction` | Review construction insurance requirements | Construction |
| `compliance-with-laws-pharmaceuticals` | Pharma regulatory compliance obligations | Pharmaceuticals |
| `survival-general` | Identify surviving post-termination obligations | General |

---

## How to Use

Once installed, your agent will automatically activate the relevant skill
when you ask things like:

- *"Review the indemnification clause in this contract"*
- *"Draft a force majeure provision for my SaaS agreement"*
- *"What are the risks in this non-compete?"*
- *"Redline this limitation of liability clause to be more favorable to us"*

---

## Skill Structure

```
skills/
  {clause}-{industry}/
    SKILL.md             ← Skill definition + workflow
    scripts/
      playbook.md        ← Detailed legal playbook & precedent language
  {clause}-{industry}.zip  ← Packaged for distribution
```

---

## Disclaimer

> Output from these skills is for **informational purposes only** and does not
> constitute legal advice. Always have qualified legal counsel review contract
> language before execution.

---

## Contributing

1. Fork this repo
2. Add or improve a `SKILL.md` under `skills/{clause}-{industry}/`
3. Run `.\zip-skills.ps1` to update packages
4. Open a PR

---

## License

MIT
