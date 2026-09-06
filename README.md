# ScooterGitTemplate [![starline](https://raw.githubusercontent.com/ScottKirvan/ScooterGitTemplate/refs/heads/starlines/ScottKirvan/ScooterGitTemplate/starline.svg)](https://github.com/qoomon/starlines)
<div align="center">

  <img src="assets/media/logo.jpg" alt="logo" width="200" height="auto" />
    <h1><a href="https://github.com/ScottKirvan/ScooterGitTemplate">ScottKirvan/ScooterGitTemplate</a></h1>
  <h3>Nulla nobis dicta iste minus dolor repellendus aspernatur atque</h3>
  
  
<!-- Badges -->
<p>
  <a href="https://github.com/ScottKirvan/ScooterGitTemplate/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/ScottKirvan/ScooterGitTemplate" alt="contributors" />
  </a>
  <a href="">
    <img src="https://img.shields.io/github/last-commit/ScottKirvan/ScooterGitTemplate" alt="last update" />
  </a>
  <a href="https://github.com/ScottKirvan/ScooterGitTemplate/network/members">
    <img src="https://img.shields.io/github/forks/ScottKirvan/ScooterGitTemplate" alt="forks" />
  </a>
  <a href="https://github.com/ScottKirvan/ScooterGitTemplate/stargazers">
    <img src="https://img.shields.io/github/stars/ScottKirvan/ScooterGitTemplate" alt="stars" />
  </a>
  <a href="https://github.com/ScottKirvan/ScooterGitTemplate/issues/">
    <img src="https://img.shields.io/github/issues/ScottKirvan/ScooterGitTemplate" alt="open issues" />
  </a>
  <a href="https://github.com/ScottKirvan/ScooterGitTemplate/blob/main/LICENSE.md">
    <img src="https://img.shields.io/github/license/ScottKirvan/ScooterGitTemplate.svg" alt="license" />
  </a>
  <a href="https://discord.gg/TN6XJSNK5Y">
    <!--<img src="https://img.shields.io/discord/704680098577514527?style=flat-square&label=%F0%9F%92%AC%20discord&color=00ACD7">-->
    <img src="https://img.shields.io/discord/1052011377415438346?style=flat-square&label=discord&color=00ACD7">
  </a>
</p>
   
<h4>
    <a href="https://tinyurl.com/3vf7whyd">View Demo</a>
  <span> · </span>
    <a href="https://github.com/ScottKirvan/ScooterGitTemplate/blob/main/README.md">Documentation</a>
  <span> · </span>
    <a href="https://github.com/ScottKirvan/ScooterGitTemplate/issues/new?template=bug_report.md">Report Bug</a>
  <span> · </span>
    <a href="https://github.com/ScottKirvan/ScooterGitTemplate/issues/new?template=feature_request.md">Request Feature</a>
  </h4>
</div>

**ScooterGitTemplate** is voluptatibus magni nemo est. Nulla nobis dicta iste minus dolor repellendus aspernatur atque. Earum expedita aut inventore tempora fugiat deleniti. Molestias minima nam expedita beatae totam ipsa reprehenderit animi. Occaecati quibusdam beatae ducimus voluptate ut doloribus vitae amet. Quia ut ut voluptate dignissimos adipisci dolorum rem.

## Getting Started with This Template

>[!IMPORTANT]
> **Customization Checklist** — After creating a repository from this template, update these items:
>
> - [ ] Update the project description (line 5 above and in repository settings)
> - [ ] Replace `assets/media/logo.jpg` with your project logo
> - [ ] Update or remove the "View Docs" link (line 35)
> - [ ] Update or remove the Discord badge/link (lines 28–31)
> - [ ] Choose and apply a `.gitignore` from `.github/gitignore-templates/` (see [gitignore templates](.github/gitignore-templates/))
> - [ ] Fill in `project_context`, `header`, `footer`, and `emoji` TODOs in `.github/workflows/release.yml` and `.github/workflows/pre-release-staging.yml`
> - [ ] Fill in the Features, Installation, and Usage sections below
> - [ ] Review and update the [Code of Conduct](CODE_OF_CONDUCT.md) contact information
> - [ ] Enable GitHub Pages in repository settings (source: GitHub Actions) for your docs site
> - [ ] Review and customize `CLAUDE.md` if using AI coding agents, or delete it if not
> - [ ] Remove or update this checklist section

>[!TIP]
> **Automatic initialization**: When you create a new repository from this template, a GitHub Actions workflow automatically updates all repository references, URLs, and badges in the README with your new repository information, then deletes itself. No manual find-and-replace needed.

## Key Features

**Automated Release Management**: The `release.yml` workflow uses [Release-Please](https://github.com/googleapis/release-please) for automated versioning and CHANGELOG updates driven by [Conventional Commits](https://www.conventionalcommits.org/). AI-generated release notes (via Gemini) and Discord notifications are wired in. See [CONTRIBUTING.md](CONTRIBUTING.md) for commit conventions.

**VitePress Documentation Site**: The `docs/` folder contains a [VitePress](https://vitepress.dev/) site that deploys to GitHub Pages via the `docs.yml` workflow. Enable Pages in your repo settings (source: GitHub Actions) to publish it.

**Pre-release Staging**: The `pre-release-staging.yml` workflow lets you generate and review AI-drafted release notes on a staging branch before the release goes out.

**Template Initialization**: The `template-init.yml` workflow runs once on your first push to a derived repo, substitutes all repository references throughout the project, enables the release workflow, and then deletes itself.

**.gitignore Templates**: The `.github/gitignore-templates/` folder contains ready-to-use `.gitignore` files for Unreal Engine, Unity, Python, Node.js, C++, and general development. See the [templates README](.github/gitignore-templates/) for usage.

**AI Agent Context (optional)**: The included `CLAUDE.md` gives AI coding agents (e.g. [Claude Code](https://claude.ai/code)) a starting set of engineering standards — branching conventions, commit discipline, test-driven development, verification discipline, and a no-shortcuts ethos. The project name is automatically substituted on initialization. Customize it as your project evolves, or delete it if you're not using AI agents.

## Repo Layout

```
ScooterGitTemplate/
├── .github/
│   ├── gitignore-templates/    # Ready-to-use .gitignore files (Unreal, Unity, Python, Node, C++)
│   ├── release-please/         # Release-Please configuration and version manifest
│   └── workflows/              # GitHub Actions workflows (see Key Features above)
├── assets/
│   └── media/                  # Images and logos
├── docs/                       # VitePress documentation site
├── notes/                      # CHANGELOG, VERSION, TODO
├── CLAUDE.md                   # AI agent context (optional)
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE.md
└── README.md
```

> **Note:** Issue templates, PR templates, and funding config live in the org-level [`ScottKirvan/.github`](https://github.com/ScottKirvan/.github) repo and apply here automatically via GitHub's community health file fallback.

Features
--------
Installation
------------
Usage
-----

Contributions / Contact
-----------------------
- Please [file an issue](https://github.com/ScottKirvan/ScooterGitTemplate/issues/new), or [grab a fork](https://github.com/ScottKirvan/ScooterGitTemplate/fork), hack away, and submit a [pull request](https://github.com/ScottKirvan/ScooterGitTemplate/pulls).
- Contact me at [linkedin.com/in/scottkirvan/](https://www.linkedin.com/in/scottkirvan/)
- You can also contact me at my [discord](https://discord.gg/TN6XJSNK5Y) server, I'm cptvideo.

Credits
-------
**[ScooterGitTemplate](https://github.com/ScottKirvan/ScooterGitTemplate)** — Copyright (c) 2025 [Scott Kirvan](https://github.com/ScottKirvan). [MIT License](LICENSE.md).

Project Link:  [ScooterGitTemplate](https://github.com/ScottKirvan/ScooterGitTemplate)  
[CHANGELOG](notes/CHANGELOG.md)  
[TODO](notes/TODO.md)
