# my.copilot.skills

This is a centralized collection of GitHub Copilot **agents**, **skills**, **instructions**, and **prompts** for team-wide use. Instead of duplicating Copilot configurations across every application repository, this repo serves as the single source of truth — open it alongside any project repo in VS Code to instantly get access to the full toolkit.

## Why a Separate Repo?

> [!IMPORTANT]
> Application repositories should **not** contain their own `.github/agents`, `.github/skills`, or `.github/prompts` folders, unless they are under development or unique to a project. Keep those common concerns here so the team maintains one place to add, update, and share Copilot customizations.

Benefits:
- One place to update agents/skills — all teams get the latest automatically
- Application repos stay lean and focused on their own source code
- Consistent Copilot behavior across every project

---

## Getting Started

### 1. Clone both repos

```bash
# Your application repo
git clone https://github.com/<your-org>/<your-app-repo>.git

# This skills repo
git clone https://github.com/<your-org>/my.copilot.skills.git
```

### 2. Open as a multi-root workspace in VS Code

Open this folder alongside your application in VS Code using the **File → Add Folder to Workspace…** menu option.  Once both folders are added, use the command **Workspaces: Save Workspace As…** to save a `<repo-name>.code-workspace` file that includes both folders.

Or - you can manually create a `<repo-name>.code-workspace` file that includes both folders:

```json
{
  "folders": [
    { "path": "../<your-app-repo>" },
    { "path": "../my.copilot.skills" }
  ]
}
```

Once both folders are open in the same VS Code workspace, GitHub Copilot automatically discovers agents, skills, instructions, and prompts from **all** workspace folders.

> [!TIP]
> Save the `<repo-name>.code-workspace` file inside your application repo (e.g. `MyApp.code-workspace`) and commit it so teammates can open the same setup with a single double-click.

---

## What's Included

See [What's Included](./WHATS_INCLUDED.md) for the full list of agents, skills, instructions, and prompts included in this repo.

---

## Repository Structure

```
my.copilot.skills/
└── .github/
    ├── copilot-instructions.md   # Team-wide Copilot defaults
    ├── agents/                   # Custom agent mode files (.agent.md)
    ├── instructions/             # Always-on instruction files (.instructions.md)
    ├── prompts/                  # Reusable prompt templates (.prompt.md)
    └── skills/                   # Skill bundles (each skill has its own folder + SKILL.md)
```

---

## Contributing

To add a new agent, skill, instruction, or prompt:

1. Create a branch from `main`
2. Add your file(s) in the appropriate `.github/` subfolder
3. Follow the existing naming convention (`kebab-case.agent.md`, `kebab-case.instructions.md`, etc.)
4. Open a pull request — the PR assistant instructions will guide the review format
