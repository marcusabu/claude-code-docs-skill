# Claude Code Docs Skill

A Claude Code plugin providing comprehensive documentation about Claude Code features, configuration, and best practices.

## Project Structure

```
.claude-plugin/
├── plugin.json           # Plugin metadata (name, version, author)
skills/
└── claude-code/
    ├── SKILL.md          # Skill definition with frontmatter
    └── docs/             # Official Claude Code documentation
        └── *.md          # 50+ documentation files
```

## Key Files

- **plugin.json** - Plugin manifest defining name, description, version
- **SKILL.md** - Skill configuration with description for when to activate
- **docs/** - Comprehensive Claude Code documentation synced from official sources

## Development

### Testing Locally

```bash
claude --plugin-dir .
```

### Validating Structure

```bash
/plugin validate .
```

### Adding Documentation

1. Add markdown files to `skills/claude-code/docs/`
2. Update `docs_manifest.json` if syncing from URLs
3. Reference new docs in `SKILL.md` if significant

## Conventions

- Documentation files follow official Claude Code naming
- SKILL.md contains quick reference guides for common patterns
- The `docs/` directory is the authoritative reference source

## Git Conventions

Commit format: `<type>(<scope>?): <message>`

**Types:**
- `feat` - New features or capabilities
- `docs` - Documentation changes
- `fix` - Bug fixes
- `test` - Test-related changes

**Examples:**
```
feat: add GitHub Actions workflow for auto-sync
feat(workflow): auto-bump minor version on doc changes
docs(readme): add example prompts section
fix: detect untracked files in workflow change check
```

**Rules:**
- Subject line only, no body
- Lowercase message, no period at end
- Scope is optional, use for specific areas (workflow, readme)
