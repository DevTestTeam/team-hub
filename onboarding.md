---
title: Software Engineering Onboarding
layout: default
---

# 🛠️ Software Engineering Onboarding: Git & Project Workflow

Welcome to the team! 🎉 We're excited to have you onboard. This document will guide you through our Git workflow using the **trunk-based development strategy**, including our **commit message template**. It’s designed for new engineers — no prior professional Git experience required.

---

## 📚 Overview

- We use **Git** for source control.
- All code lives in a single branch: `main`.
- We develop using **short-lived feature branches** that are merged quickly.
- We work through **pull requests** (PRs) and code reviews.

---

## 🌳 Trunk-Based Branching Strategy

In this workflow, the `main` branch (aka "trunk") is always stable, always deployable, and frequently updated.

```
main   ← central branch
 │
 ├── jdoe/my-first-feature
 ├── jdoe/fix-login-issue
```

### 🔑 Key Rules

- **Branch off from `main`** for every task.
- Use **short-lived branches** (ideally < 2 days).
- Open a PR as soon as possible.
- Use **feature flags** for incomplete features.
- **Never commit directly to `main`** — use a PR.

---

## 🏷️ Branch Naming Convention

Use this format:

```
<yourname>/<short-description>
```

Examples:
- `jdoe/add-logout-button`
- `jdoe/update-readme`
- `jdoe/fix-auth-bug`

---

## 📝 Commit Message Template

We use structured commit messages to keep history clean and understandable.

**Format:**

```
<type>(<scope>): <short description>

<body>
```

**Example:**

```
feat(auth): add logout functionality

Implements logout API and clears session tokens on the frontend.
Hidden behind a feature flag until tested.

Resolves: JIRA-4321
```

### Common Types

- `feat`: New functionality
- `fix`: Bug fix
- `docs`: Documentation only
- `style`: Code formatting (no logic change)
- `refactor`: Code change with no functional difference
- `test`: Test code only
- `chore`: Maintenance (build scripts, tooling, etc)

---

## 🔁 Pull Request Process

1. Create your short-lived branch from `main`.
2. Commit regularly and push to GitHub.
3. Open a **Pull Request** (PR) to `main`.
4. Use a meaningful title and description.
5. Link any Jira issues using `Resolves: JIRA-####`.
6. Request a review from your mentor or a teammate.
7. Once approved and CI passes, the PR will be merged.

---

## ✅ Tips for Success

- Keep branches small and focused.
- Rebase or pull `main` regularly to avoid conflicts.
- Use draft PRs to get early feedback.
- Ask questions early and often.
- Write clean, understandable commit messages.
- Review others’ code to learn and contribute.

---

## 📎 Resources

- [GitHub Docs: Branches](https://docs.github.com/en/get-started/quickstart/github-flow)
- [Trunk-Based Development Overview](https://trunkbaseddevelopment.com/)
- Ask your onboarding buddy or mentor for a walkthrough!

---

We’re glad you’re here — let’s build something great together! 🚀
