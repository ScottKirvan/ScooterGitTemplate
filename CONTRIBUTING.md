# Contributing to ScooterGitTemplate

First off, thank you for considering contributing to ScooterGitTemplate! It's people like you that make this template better for everyone.

## Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check the existing issues to avoid duplicates. When you create a bug report, include as many details as possible using our bug report template.

**Guidelines for bug reports:**
- Use a clear and descriptive title
- Describe the exact steps to reproduce the problem
- Provide specific examples to demonstrate the steps
- Describe the behavior you observed and what you expected to see
- Include screenshots if applicable
- Note your environment (OS, version, etc.)

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion, use our feature request template and include:

- A clear and descriptive title
- A detailed description of the proposed feature
- Examples of how the feature would be used
- Why this enhancement would be useful

### Pull Requests

**Before submitting a pull request:**

1. Fork the repository and create your branch from `main`
2. If you've added code, add tests if applicable
3. Ensure your code follows the existing style
4. Make sure your commits follow the commit message conventions below
5. Update documentation as needed

## Commit Message Conventions

This project uses [Conventional Commits](https://www.conventionalcommits.org/) with [Semantic Versioning](https://semver.org/). Release-Please reads your commit messages to determine the next version number and generate the CHANGELOG automatically — so the type prefix matters.

| Prefix | Effect | Use for |
|--------|--------|---------|
| `feat:` | Bumps **MINOR** version | New features |
| `fix:` | Bumps **PATCH** version | Bug fixes and corrections |
| `docs:` | No version bump | Documentation only |
| `chore:` | No version bump | Maintenance, generated files |
| `refactor:` | No version bump | Code restructuring |
| `test:` | No version bump | Adding or updating tests |
| `feat!:` / `fix!:` / `xxx!:` | Bumps **MAJOR** version | Breaking changes |

**Examples:**
```
feat: add Rust .gitignore template
fix: correct workflow trigger in docs.yml
docs: update installation instructions
feat!: change template initialization to require manual trigger
```

> **Tip:** When in doubt between `feat:` and `fix:`, use `fix:` — it's the right call for corrections to existing behavior even when they close a tracked issue.

## Pull Request Process

1. Update README.md if your change affects user-facing behavior
2. CHANGELOG.md is updated automatically by Release-Please — do not edit it manually
3. The PR will be merged once approved by a maintainer
4. Your PR should pass all CI checks and have no merge conflicts

## Development Setup

1. Fork and clone the repository
2. Create a new branch for your feature or fix: `git checkout -b feat/your-feature origin/main`
3. Make your changes
4. Test by creating a new repository from your modified template fork and verifying the template-init workflow runs correctly
5. Submit a pull request

## Project Structure

```
ScooterGitTemplate/
├── .github/
│   ├── gitignore-templates/    # Ready-to-use .gitignore files
│   ├── release-please/         # Release-Please config and version manifest
│   └── workflows/              # GitHub Actions workflows
├── assets/
│   └── media/                  # Images and logos
├── docs/                       # VitePress documentation site
│   ├── .vitepress/             # VitePress config and theme
│   └── index.md                # Docs home page
├── notes/                      # CHANGELOG, VERSION, TODO
├── CLAUDE.md                   # AI agent context (optional)
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md             # This file
├── LICENSE.md
└── README.md
```

> **Note:** Issue templates, PR templates, and funding config live in the org-level [`ScottKirvan/.github`](https://github.com/ScottKirvan/.github) repo and apply here automatically via GitHub's community health file fallback.

## Testing Template Changes

When making changes to the initialization or release workflows, test by:

1. Creating a new repository from your modified template fork
2. Verifying `template-init.yml` runs successfully and all repository references are updated
3. Confirming the workflow deletes itself after completion
4. Making a conventional commit and verifying Release-Please creates the expected PR

## Questions?

Feel free to open an issue or reach out via:
- [LinkedIn](https://www.linkedin.com/in/scottkirvan/)
- [Discord](https://discord.gg/TN6XJSNK5Y)

Thank you for your contributions!
