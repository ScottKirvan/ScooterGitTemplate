# CLAUDE.md — ScooterGitTemplate

## Working Conventions

- Never commit or push directly to `main`. Always branch first, then PR.
- Branch names must describe the work (e.g. `fix/login-timeout`, `feat/export-csv`).
  No random characters, UUIDs, or generated suffixes to ensure uniqueness — if a name
  is already taken, pick a more specific descriptive name instead.
- Conventional commits: `feat:` / `fix:` / `docs:` / `chore:` / `refactor:` / `test:`.
  Breaking: `feat!:`.
- `feat:` is for genuinely new user-facing capabilities only. Bug fixes and corrections
  use `fix:`, even when they close a tracked issue.
- Unit tests must be written alongside all new code. All bug fixes require red/green
  tests — a failing test that reproduces the bug, then the fix that makes it pass.
- CI, lint, and formatting must all pass before committing or opening a PR.

## No Shortcuts

Nothing is deferred without explicit permission from the project owner. A known issue
is still a bug — do not mark it "won't fix", "by design", or "out of scope" unilaterally.

If a library or package cannot meet a requirement in the spec, the answer is to find
an alternative or do the work from first principles — not to defer the requirement or
revise the spec to fit the limitation. The spec defines what the project needs; the
implementation serves the spec, not the other way around.

## Attribution

No attribution of any kind in commit messages, PR bodies, or issue text — no
"Generated with", "Co-Authored-By", "Created by Claude", or any AI/tool credit lines.

**Verify by reading the repo, not from memory.** Tooling (GitHub Actions, IDE plugins)
can inject attribution without the agent's knowledge. Before finalizing any commit or PR:
- Run `git log` and read the actual commit messages
- Read the actual PR body text
- Remove any attribution found, regardless of source

## GitHub Issues and PRs

Issue and PR templates live in `ScottKirvan/.github` and apply to this repo automatically.

- Bug reports → `[BUG]` title prefix, `bug_report.md` sections
- Feature requests → `[FEATURE]` title prefix, `feature_request.md` sections
- General → `[GENERAL]` title prefix, `general_report.md` sections
- PRs → fill all checklist sections; no attribution anywhere in the body

Before creating any issue: check for duplicates first (`gh issue list --state open --limit 100`).
Create issues only when explicitly asked — don't preemptively file future work.

## Sub-Agent Workflow

When using sub-agents for implementation:

- Brief sub-agents on **what** to build, not **how** — implementation decisions belong
  to the sub-agent, which serves as an independent second opinion on the approach.
- Sub-agents follow all conventions in this file except they do not create PRs.
- The launching agent reviews the sub-agent's diff and tests before creating the PR.
  This review is a genuine code review, not a compliance check — evaluate correctness,
  spec alignment, and test quality independently.
- Simple issues found in review may be fixed directly. Significant deviations from spec
  or complex problems go back to the sub-agent rather than being patched over.
- The launching agent creates the PR only after review passes.
