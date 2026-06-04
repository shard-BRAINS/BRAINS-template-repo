<!-- markdownlint-disable MD041 (brand banner starts with a centered HTML block) -->
<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/shard-BRAINS/.github/main/profile/brand-mark-dark-bg.png">
  <img alt="BRAINS" src="https://raw.githubusercontent.com/shard-BRAINS/.github/main/profile/brand-mark-light-bg.png" width="220">
</picture>

# BRAINS template repo

<!-- markdownlint-disable-next-line MD001 (intentional tagline subtitle) -->
### The standard floor for every new BRAINS repository

<br />

[![Status](https://img.shields.io/badge/status-ready-D99518?style=for-the-badge&labelColor=0A0A0A)](https://github.com/shard-BRAINS/BRAINS-template-repo)
[![Type](https://img.shields.io/badge/type-template-2A8B91?style=for-the-badge&labelColor=0A0A0A)](https://github.com/shard-BRAINS/BRAINS-template-repo/generate)
[![Licence](https://img.shields.io/badge/licence-MIT-0A0A0A?style=for-the-badge&labelColor=D99518)](LICENSE)
[![Discord](https://img.shields.io/badge/Discord-Community-5865F2?style=for-the-badge&logo=discord&logoColor=FFFFFF&labelColor=0A0A0A)](https://discord.gg/BEmTXXscBr)
[![Bluesky](https://img.shields.io/badge/Bluesky-%40brainscertified.com-D99518?style=for-the-badge&logo=bluesky&logoColor=FFFFFF&labelColor=0A0A0A)](https://bsky.app/profile/brainscertified.com)
[![BRAINS](https://img.shields.io/badge/BRAINS-Standards-D99518?style=for-the-badge&labelColor=0A0A0A)](https://github.com/shard-BRAINS)
[![BRAINS Certified Gold](https://img.shields.io/badge/BRAINS%20Certified-Gold-D99518?style=for-the-badge&labelColor=0A0A0A)](CERTIFIED.md)

<br />

[What you get ↓](#what-you-get) &nbsp;·&nbsp; [Use this template ↓](#use-this-template) &nbsp;·&nbsp; [README skeleton ↓](#project-readme-skeleton) &nbsp;·&nbsp; [Full recipe ↓](docs/using-this-template.md)

</div>

---

This is the starter for every new BRAINS repo. It ships the checks we run on our own code: security, access, and clear prose.

> **Reliable, affirming, inclusive.**

**The BRAINS standard floor for any new repository — [from BRAINS](https://github.com/shard-BRAINS), built by neurodivergent minds, for neurodivergent people.**

---

## What you get

| Layer | Tools |
|---|---|
| Security floor | OpenSSF Scorecard, CodeQL, Trivy, Gitleaks, Dependabot |
| Prose voice and brand | Vale with the BRAINS rule pack (Do/Don't, protected phrases, anti-deficit) |
| Readability | Flesch-Kincaid grade gate (Grade 8 public, Grade 10 technical) |
| Markdown hygiene | markdownlint with BRAINS defaults |
| Accessibility (opt-in) | axe-core and Pa11y for any repo with a web surface |
| Governance | ND-affirming Code of Conduct, Security policy, Contributing guide |

All of these run on push and pull request. None of them require paid services.

## BRAINS Certified · Gold

Meet the standard floor and your repo earns the **BRAINS Certified · Gold** mark. One tier only. Clear the minimum, wear the Gold tag, and get listed.

<p align="center">
  <img src="assets/badges/brains-certified-gold.svg" alt="BRAINS Certified — Gold Standard" height="86">
</p>

To earn Gold, a repo must:

- Pass every standard check on `main` — Scorecard, CodeQL, Trivy, Gitleaks, Vale, Readability, and Markdownlint.
- Ship the ND-affirming governance files — Code of Conduct, Security policy, and Contributing guide.

When you qualify:

1. Add the Gold badge to your README.
2. Open a [certification request](../../issues/new?template=certification-request.yml). A maintainer checks the evidence and adds your row.

See the full list of [certified repositories](CERTIFIED.md).

## Use this template

1. Click **Use this template** in the GitHub UI to make a new repo. Or copy `.github/`, `.vale/`, `.vale.ini`, `.markdownlint.json`, `.gitleaks.toml`, and `scripts/` into an existing one.
2. Replace the `[PROJECT NAME]`, `[ONE-LINE DESCRIPTION]`, and `[OWNER]` placeholders below.
3. Got a web UI? Set the repo variable `HAS_WEB_UI=true` (Settings → Variables) to turn on the access checks.
4. Turn on branch protection. Require the standard checks before merge.

See [docs/using-this-template.md](docs/using-this-template.md) for the full setup guide.

## Project README skeleton

After cloning, swap this for your own README. Keep the shape below. Every BRAINS README opens with a plain lead and a clear next step.

```markdown
# [PROJECT NAME]

[ONE-LINE DESCRIPTION in plain English. Aim for Grade 8 reading level.
What is this, in a sentence a busy reader can understand at a glance.]

## What this is

[Two or three short paragraphs. Who it is for, what problem it solves,
what it does not do.]

## Quick start

[The shortest path from "I just cloned this" to "I see it working".]

## How it works

[The next layer of detail. Diagrams welcome. Avoid jargon on first use.]

## Contributing

See CONTRIBUTING.md.

## Security

See SECURITY.md.

## License

[MIT by default — change if needed.]
```

## License

MIT. See `LICENSE`.
