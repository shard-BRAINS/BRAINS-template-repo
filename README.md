# BRAINS template repo

This is the starter for every new BRAINS repository. It ships the security, accessibility, and readability checks BRAINS commits to on its own work.

> **Why this exists.** BRAINS Certified holds AI systems to standards of safety, accessibility, and neuro-affirming design. We hold our own code to the same standards. This template makes that the default, not an aspiration.

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
