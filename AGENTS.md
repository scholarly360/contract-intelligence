# AGENTS.md — Contract Intelligence Skills Repo

This file provides guidance to AI coding agents working within this repository.

## Repository Purpose

This is an **Agent Skills package** following the [Agent Skills specification](https://github.com/vercel-labs/skills).
It contains reusable contract analysis skills for AI agents.

## Repository Structure

```
contract-intelligence/
├── README.md                          ← Public-facing documentation
├── AGENTS.md                          ← This file (agent guidance)
├── scaffold-skills.ps1                ← Windows: generate skill scaffolding
├── zip-skills.ps1                     ← Windows: package skills as .zip
└── skills/
    ├── {clause}-{industry}/
    │   ├── SKILL.md                   ← Skill definition (REQUIRED)
    │   └── scripts/
    │       └── playbook.md            ← Detailed legal playbook
    └── {clause}-{industry}.zip        ← Distribution package (REQUIRED)
```

## Naming Conventions

- Skill directories: `{clause}-{industry}` in kebab-case (e.g., `confidentiality-general`)
- `SKILL.md` — always uppercase, always this exact filename
- Zip file — must match directory name: `{skill-name}.zip`

## SKILL.md Requirements

Every `SKILL.md` must have valid YAML frontmatter:

```yaml
---
name: skill-name          # kebab-case, matches directory name
description: >            # One sentence — this is what the agent uses for routing
  Activate when the user mentions X, Y, or Z.
---
```

Keep `SKILL.md` under 500 lines. Move detailed content to `scripts/playbook.md`.

## Adding a New Skill

1. Create `skills/{clause}-{industry}/` directory
2. Add `SKILL.md` with frontmatter + workflow
3. Add `scripts/playbook.md` with legal reference content
4. Run `.\zip-skills.ps1` to create the `.zip` package
5. Commit both the folder AND the `.zip`

## Modifying an Existing Skill

1. Edit the relevant `SKILL.md` or `scripts/playbook.md`
2. Re-run `.\zip-skills.ps1` to regenerate the `.zip`
3. Commit both changes together

## Legal Disclaimer Requirement

Every `SKILL.md` MUST include this or equivalent language:
> Output is for informational purposes only and does not constitute legal advice.

## Do Not

- Do not store real client contracts or PII in this repo
- Do not hardcode jurisdiction-specific advice without caveats
- Do not exceed 500 lines in any single `SKILL.md`
