# Copilot Agents

> A curated collection of reusable GitHub Copilot agent instruction files for **VS Code** and **IntelliJ IDEA** — built for professional software teams.

---

## What Is This?

Each `.md` file in the `/agents` directory is a self-contained **agent instruction set** you can load into GitHub Copilot Chat to give it a focused persona, specialized behavior, and domain expertise — no plugins required.

Think of each agent as a **senior expert on-call** for a specific engineering task.

---

## How to Use

### VS Code
**Option A — Attach as context in Copilot Chat:**
```
> Attach file → agents/code-reviewer.md
```
Then ask your question normally. Copilot uses the agent's instructions as context.

**Option B — Workspace-level default agent:**
Copy any agent's content into `.github/copilot-instructions.md` in your project root.

**Option C — Reference inline:**
```
#file:agents/code-reviewer.md Review this PR diff
```

### IntelliJ IDEA (with GitHub Copilot Plugin)
1. Open **Copilot Chat** panel (`View → Tool Windows → GitHub Copilot`)
2. Paste the contents of any agent `.md` file as a system prompt or prefix message
3. Continue chatting — Copilot will adopt the agent persona for the session

---

## Agent Catalog

| Agent | File | Best For |
|---|---|---|
| Code Reviewer | [`agents/code-reviewer.md`](agents/code-reviewer.md) | PR reviews, quality gates |
| Architecture Advisor | [`agents/architecture-advisor.md`](agents/architecture-advisor.md) | System design, trade-offs |
| Test Engineer | [`agents/test-engineer.md`](agents/test-engineer.md) | Unit, integration, E2E tests |
| Security Auditor | [`agents/security-auditor.md`](agents/security-auditor.md) | Vulnerability scanning, OWASP |
| Docs Writer | [`agents/docs-writer.md`](agents/docs-writer.md) | READMEs, Javadoc, JSDoc |
| Refactoring Expert | [`agents/refactoring-expert.md`](agents/refactoring-expert.md) | Clean code, SOLID, DRY |
| Debug Detective | [`agents/debug-detective.md`](agents/debug-detective.md) | Root cause analysis, logs |
| API Designer | [`agents/api-designer.md`](agents/api-designer.md) | REST, GraphQL, OpenAPI |
| Database Optimizer | [`agents/database-optimizer.md`](agents/database-optimizer.md) | SQL, indexes, query plans |
| DevOps Engineer | [`agents/devops-engineer.md`](agents/devops-engineer.md) | CI/CD, Docker, Kubernetes |
| Performance Profiler | [`agents/performance-profiler.md`](agents/performance-profiler.md) | Bottlenecks, memory, CPU |
| Onboarding Guide | [`agents/onboarding-guide.md`](agents/onboarding-guide.md) | New devs, codebase walkthrough |
| Spring Boot Upgrade | [`agents/springboot-upgrade.md`](agents/springboot-upgrade.md) | Spring Boot 2.x → 3.x, Jakarta EE migration |

---

## Agent File Format

Each agent follows a consistent structure:

```markdown
# Agent Name
**Role:** ...
**Expertise:** ...

## Behavior
...

## Rules
...

## Output Format
...
```

---

