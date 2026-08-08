# CLAUDE.md — ScooterGitTemplate

## Current Status
Just created from the [ScooterGitTemplate](https://github.com/ScottKirvan/ScooterGitTemplate).
README and other files contain placeholder lorem ipsum — complete the customization
checklist in README.md before starting any other work.

## Working Conventions

- Never commit or push directly to `main`. Always branch first, then PR.
- Branch names must describe the work (e.g. `fix/login-timeout`, `feat/export-csv`).
- Rebase and merge PRs. After merge: `git checkout main && git pull`, delete the branch.
- Conventional commits: `feat:` / `fix:` / `docs:` / `chore:` / `refactor:` / `test:`.
  Breaking: `feat!:`.
- `feat:` is for genuinely new user-facing capabilities only. Bug fixes and corrections
  use `fix:`, even when they close a tracked issue.

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
