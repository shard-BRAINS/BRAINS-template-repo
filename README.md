<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/shard-BRAINS/.github/main/profile/brand-mark-dark-bg.png">
  <img alt="BRAINS" src="https://raw.githubusercontent.com/shard-BRAINS/.github/main/profile/brand-mark-light-bg.png" width="220">
</picture>

# BRAINS template repo

### The standard floor for every new BRAINS repository.

<br />

[![Status](https://img.shields.io/badge/status-ready-D99518?style=for-the-badge&labelColor=0A0A0A)](https://github.com/shard-BRAINS/BRAINS-template-repo)
[![Type](https://img.shields.io/badge/type-template-2A8B91?style=for-the-badge&labelColor=0A0A0A)](https://github.com/shard-BRAINS/BRAINS-template-repo/generate)
[![Licence](https://img.shields.io/badge/licence-MIT-0A0A0A?style=for-the-badge&labelColor=D99518)](LICENSE)
[![Discord](https://img.shields.io/badge/Discord-Community-5865F2?style=for-the-badge&logo=discord&logoColor=FFFFFF&labelColor=0A0A0A)](https://discord.gg/BEmTXXscBr)
[![Bluesky](https://img.shields.io/badge/Bluesky-%40brainscertified.com-D99518?style=for-the-badge&logo=bluesky&logoColor=FFFFFF&labelColor=0A0A0A)](https://bsky.app/profile/brainscertified.com)
[![BRAINS](https://img.shields.io/badge/BRAINS-Standards-D99518?style=for-the-badge&labelColor=0A0A0A)](https://github.com/shard-BRAINS)

<br />

[What you get ↓](#what-you-get) &nbsp;·&nbsp; [Use this template ↓](#use-this-template) &nbsp;·&nbsp; [README skeleton ↓](#project-readme-skeleton) &nbsp;·&nbsp; [Full recipe ↓](docs/using-this-template.md)

</div>

---

This is the starter for every new BRAINS repo. It ships the same checks we run on our own code: security, access, and readable prose.

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

## Use this template

1. Click **Use this template** in the GitHub UI to create a new repo, or copy `.github/`, `.vale/`, `.vale.ini`, `.markdownlint.json`, `.gitleaks.toml`, and `scripts/` into an existing repo.
2. Replace the `[PROJECT NAME]`, `[ONE-LINE DESCRIPTION]`, and `[OWNER]` placeholders below.
3. If the repo has a web UI, set the repo variable `HAS_WEB_UI=true` (Settings → Variables) to enable the accessibility job.
4. Turn on branch protection: require status checks (Scorecard, CodeQL, Trivy, Gitleaks, Vale, Readability) before merge.

See [docs/using-this-template.md](docs/using-this-template.md) for the full inheritance recipe.

## Project README skeleton

After cloning, replace this section with your own README. Keep the structure below — every BRAINS README starts with a plain-English lead and a clear "what next" section.

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
