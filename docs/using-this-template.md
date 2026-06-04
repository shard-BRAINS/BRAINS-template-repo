# Using this template

Two paths. Pick whichever fits.

## Path A — New repository

1. From the GitHub UI, click **Use this template → Create a new repository**.
2. Pick the new owner and name. Keep the `BRAINS-` or `shard-` prefix per the org naming convention.
3. After creation, edit `README.md` and replace the `[PROJECT NAME]`, `[ONE-LINE DESCRIPTION]`, and `[OWNER]` placeholders.
4. In **Settings → Branches**, turn on branch protection for `main`:
   - Require a pull request before merging
   - Require these status checks: `Scorecard analysis`, `CodeQL`, `Trivy filesystem + config scan`, `Gitleaks secret scan`, `Vale prose lint`, `Flesch-Kincaid grade check`, `Markdownlint`
5. In **Settings → Variables**, if the repo has a web UI:
   - Add `HAS_WEB_UI` = `true`
   - Optionally add `STATIC_DIR` (default `./public`)
6. Add a Scorecard badge to the README using the URL shown in the workflow summary after the first run.

## Path B — Existing repository

Copy these files into the existing repo, then PR:

```text
.github/workflows/scorecard.yml
.github/workflows/codeql.yml
.github/workflows/trivy.yml
.github/workflows/gitleaks.yml
.github/workflows/vale.yml
.github/workflows/readability.yml
.github/workflows/markdownlint.yml
.github/workflows/a11y.yml         (only if HAS_WEB_UI applies)
.github/dependabot.yml
.github/PULL_REQUEST_TEMPLATE.md
.github/ISSUE_TEMPLATE/
.vale.ini
.vale/styles/BRAINS/
.markdownlint.json
.gitleaks.toml
scripts/readability_check.py
SECURITY.md
CODE_OF_CONDUCT.md
CONTRIBUTING.md
```

Do not overwrite an existing `README.md` or `LICENSE` automatically. Adjust the README skeleton by hand so the plain-English lead is in place.

Run CI on the PR. Expect the first run to surface real findings — that is the point. Fix them before merging, or open follow-up issues for anything that cannot be fixed in the same PR.

## Calibration

The thresholds in `.github/workflows/readability.yml` are set to Grade 8 (public copy) and Grade 10 (technical docs). These are deliberately strict. If a specific file legitimately needs to sit higher (e.g., a research-grade methodology document), add the marker near the top:

```html
<!-- readability: skip -->
```

Use the skip marker sparingly. Every skip is a small admission that the doc is not accessible to the audience BRAINS exists to serve.

## Vale rule pack

The `.vale/styles/BRAINS/` rule pack encodes the BRAINS brand guidelines mechanically: protected phrases, the Do/Don't language table, deficit-framing detection, banned metaphors (the puzzle-piece motif), and brand capitalisation. Updating the brand guidelines means updating these YAML files. The skill `brains-brand` is the editorial source of truth; the Vale rules are the CI enforcement.

## When you outgrow the template

Some repos will need a stricter CI than the template provides — for example, a production SaaS will want full SBOM generation, signed releases, and SLSA provenance. Add those, but do not remove anything from the template. The floor is the floor.
