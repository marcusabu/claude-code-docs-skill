# Claude Code Docs Plugin

A Claude Code plugin with comprehensive documentation about Claude Code features and configuration.

## Installation

```bash
# Add the marketplace from GitHub
/plugin marketplace add marcusabu/claude-code-docs-plugin

# Install the plugin
/plugin install claude-code-docs@marcusabu-claude-code-docs

# Local testing
claude --plugin-dir ./plugins/claude-code-docs
```

## What's Included

50+ documentation files covering skills, agents, hooks, MCP servers, settings, plugins, IDE integrations, and more.

**Note:** The docs are auto-synced daily via GitHub Actions, but the SKILL.md index is not yet auto-updated. This is [a work in progress](https://github.com/marcusabu/claude-code-docs-plugin/issues/2).

## Example Prompts

Once installed, try asking Claude things like:

- "Generate a skill that teaches Claude our codebase conventions and PR standards"
- "Create a hook that automatically runs my test suite whenever I edit source files"
- "Build an MCP server that lets Claude query our production database safely"
- "Set up an agent that reviews my code changes before I commit"
- "Create a plugin with custom slash commands for our team's daily workflows"
- "Configure Claude to use different models and permissions per project"

## Acknowledgments

Documentation sourced from [claude-code-docs](https://github.com/ericbuess/claude-code-docs) by Eric Buess.

## License

MIT
