# What's Included

## Copilot Instructions

The root `copilot-instructions.md` (`.github/copilot-instructions.md`) sets team-wide defaults covering project structure, C# code style, Blazor conventions, CSS best practices, Bicep patterns, and workflow standards. These apply automatically whenever Copilot is active in the workspace.

---

## Agents (`.github/agents/`)

Custom agent modes that give Copilot a focused persona and toolset for a specific domain. Invoke them from the Copilot Chat panel with `@agent-name`.

| Agent | Purpose |
|---|---|
| `azure-principal-architect` | Azure Well-Architected Framework guidance |
| `azure-saas-architect` | Multi-tenant SaaS on Azure |
| `azure-iac-generator` | Bicep / Terraform / ARM / Pulumi generation |
| `azure-verified-modules-bicep` | IaC with Azure Verified Modules (Bicep) |
| `azure-verified-modules-terraform` | IaC with Azure Verified Modules (Terraform) |
| `bicep-plan` / `bicep-implement` | Two-phase Bicep planning and implementation |
| `github-actions-expert` | Secure CI/CD workflow authoring |
| `devops-expert` | DevOps infinity-loop guidance |
| `expert-dotnet-software-engineer` | Modern .NET / C# engineering |
| `expert-react-frontend-engineer` | React 19 + TypeScript frontend |
| `CSharpExpert` | C# code generation and review |
| `csharp-mcp-expert` / `typescript-mcp-expert` | MCP server development |
| `semantic-kernel-dotnet` / `-python` | Semantic Kernel AI apps |
| `microsoft-agent-framework-dotnet` / `-python` | Microsoft Agent Framework |
| `dba` / `ms-sql-dba` | Database administration |
| `security-engineer` | Security review and remediation |
| `playwright-tester` | Playwright test generation |
| `debug` | Focused debugging sessions |
| `implementation-plan` / `plan` | Structured implementation planning |
| `prd` | Product Requirements Documents |
| `task-planner` / `task-researcher` | Task decomposition and research |
| `ado-boards` | Azure DevOps Boards management |
| `context7` | Up-to-date library documentation lookups |
| `gilfoyle` | Code review with sardonic technical rigor |
| `Thinking-Beast-Mode` | Deep, unconstrained problem-solving |
| `api-architect` | API design mentorship |
| `search-ai-optimization-expert` | SEO / AEO / GEO optimization |

---

## Skills (`.github/skills/`)

Reusable, domain-specific skill bundles that load best-practice context on demand. Over 100 skills covering:

- **Azure** — deployment, validation, cost optimization, resource health, RBAC, Kubernetes, Postgres, Static Web Apps, App Insights
- **Infrastructure as Code** — Bicep, Terraform, AVM modules, multi-stage Dockerfiles, containerization
- **.NET / C#** — async patterns, EF Core, MSTest, xUnit, NUnit, TUnit, design patterns, best practices
- **Testing** — Playwright automation, Jest, web app testing, agentic evaluation
- **Documentation** — README generation, ADRs, specifications, implementation plans, OO component docs
- **GitHub** — Issues, PRs, Actions workflows, gh CLI, git-flow, conventional commits
- **AI / Agents** — Copilot SDK, MCP server generation (C#, TypeScript, Python, Swift), prompt engineering, declarative agents
- **Web** — React, Fluent UI Blazor, web forms, markdown-to-html, game engine
- **DevOps** — Rollout plans, Azure DevOps CLI, pipeline translation
- **Database** — SQL optimization, SQL code review
- **Miscellaneous** — Architecture blueprints, technology stack docs, folder structure generators, refactoring

---

## Instructions (`.github/instructions/`)

Always-on behavioral rules that shape every Copilot response for a given file type or context.

| File | Applied To |
|---|---|
| `accessibility-auditor.instructions.md` | `**/*.html` |
| `code-reviewer.instructions.md` | All files |
| `concept-explainer.instructions.md` | All files |
| `debugging-tutor.instructions.md` | All files |
| `github-actions-helper.instructions.md` | All files |
| `issue-manager.instructions.md` | All files |
| `pull-request-assistant.instructions.md` | All files |

---

## Prompts (`.github/prompts/`)

Reusable prompt templates for common, repeatable workflows:

| Prompt | Purpose |
|---|---|
| `Phase1-Plan-Migration` → `Phase6-SetupCICD` | End-to-end migration phases |
| `generate-playwright-tests` / `PlayWright` | Test generation |
| `refactor-guidelines` | Guided refactoring |
| `test-for-quality` | Quality-focused test review |
| `translate-workflow-to-pipeline` | GitHub Actions ↔ Azure DevOps |
| `GetStatus` | Project status summary |
