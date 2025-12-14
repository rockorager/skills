---
name: commit-messages
description: Write clear commit messages. Use when asked to write a commit message, prepare a commit, or describe changes for version control.
---

# Commit Messages

Write clear, informative commit messages following conventional commit format.

## Workflow

### 1. Analyze the Changes

```bash
# View staged changes
git diff --cached

# View all uncommitted changes
git diff HEAD

# See changed files summary
git status --short
```

### 2. Write the Message

**Commit Message Format:**
- Limit the first line (title) to 60 characters maximum
- Use a short prefix for readability with git log --oneline (do not use "fix:" or "feature:" prefixes)
- Use only lowercase letters for the commit title except when quoting symbols or known acronyms
- Address only one issue/topic per commit
- Use imperative mood (e.g. "make xyzzy do frotz" instead of "makes xyzzy do frotz")

**Commit Message Body:**
- Use the body to explain what your patch does and why it is useful
- Even for one-line fixes, the description may span multiple paragraphs
- Use proper English syntax, grammar and punctuation
- Write in imperative mood as if giving orders to the codebase

**Commit Trailers:**
- If fixing a ticket, use appropriate commit trailers
- If fixing a regression from another commit, add a "Fixes:" trailer with the commit id and title

### 3. Commit

```bash
git commit -m "type(scope): subject" -m "body paragraph"
```
