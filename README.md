# Agent Skills

A collection of reusable [Agent Skills](https://docs.anthropic.com/en/docs/claude-code/skills).

## Usage

To use these skills, symlink or copy this directory to `~/.claude/skills`:

```bash
ln -s /path/to/this/repo ~/.claude/skills
```

## Available Skills

| Skill | Description |
|-------|-------------|
| [commit-messages](commit-messages/SKILL.md) | Write clear commit messages (requires [git-hunks](https://github.com/rockorager/git-hunks)) |
| [compiler-explorer](compiler-explorer/SKILL.md) | Optimize functions by generating and analyzing compiler assembly output |
