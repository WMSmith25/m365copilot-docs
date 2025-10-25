# Microsoft 365 Copilot Extensibility Quick Reference

A quick reference guide for navigating the Microsoft 365 Copilot extensibility documentation repository.

## Quick Start Commands

### Validation

```bash
# Run markdown linting (~3 seconds)
markdownlint docs --config .markdownlint.json --ignore **\node_modules\**

# Run spell checking (~3 seconds)
cspell --config cspell.json "docs/**/*.md"

# Clean unused images (~45-50 seconds)
pwsh scripts/CleanupUnusedImages.ps1
```

### Installation

```bash
# Install validation tools
npm install -g markdownlint-cli cspell

# Verify PowerShell Core
pwsh --version

# Verify Node.js and npm
node --version && npm --version
```

## Three Ways to Extend Copilot

1. **Copilot Connectors** - Add organizational data
2. **Agents** - Build AI assistants
3. **Copilot APIs** - Integrate programmatically

## Agent Types

### Declarative Agents

- Use Copilot's orchestrator and models
- Configure with JSON or TypeSpec
- Add knowledge and API plugins
- Best for: Most common scenarios

**Start Here**: `docs/overview-declarative-agent.md`

### Custom Engine Agents

- Bring your own orchestrator and models
- Use M365 Agents SDK or Teams AI Library
- Full control over agent behavior
- Best for: Complex, specialized scenarios

**Start Here**: `docs/overview-custom-engine-agent.md`

## Common Development Paths

### Path 1: Build a Declarative Agent with JSON

1. `docs/overview-declarative-agent.md`
2. `docs/build-declarative-agents.md`
3. `docs/build-declarative-agents-customize-behavior.md`
4. `docs/build-declarative-agents-add-knowledge.md`
5. `docs/declarative-agent-manifest-1.5.md`

### Path 2: Build a Declarative Agent with TypeSpec

1. `docs/overview-typespec.md`
2. `docs/build-declarative-agents-typespec.md`
3. `docs/typespec-scenarios.md`
4. `docs/typespec-authentication.md`

### Path 3: Add API Plugins to Agents

1. `docs/overview-api-plugins.md`
2. `docs/build-api-plugins-typespec.md` OR `docs/build-api-plugins-existing-api.md`
3. `docs/api-plugin-manifest-2.3.md`
4. `docs/openapi-document-guidance.md`

### Path 4: Build a Custom Connector

1. `docs/overview-copilot-connector.md`
2. `docs/build-your-first-connector.md`

### Path 5: Use Copilot APIs

1. `docs/copilot-apis-overview.md`
2. `docs/api/ai-services/retrieval/overview.md`
3. `docs/api/ai-services/search/overview.md`

## Manifest Versions (Latest)

- **Declarative Agent**: Version 1.5 (`docs/declarative-agent-manifest-1.5.md`)
- **API Plugin**: Version 2.3 (`docs/api-plugin-manifest-2.3.md`)

## Available Agent Templates

1. Career Coach
2. Customer Insight Assistant
3. Idea Coach
4. Interview Question Assistant
5. Learning Coach
6. Meeting Coach
7. Prompt Coach
8. Quiz Tutor
9. Scrum Assistant
10. Writing Coach

**Overview**: `docs/agent-templates-overview.md`

## Copilot Studio Options

### Lite Experience

- `docs/copilot-studio-lite.md`
- Quick agent building
- Template-based development
- Fine-tuned models support

### Full Experience

- `docs/copilot-studio-experience.md`
- Advanced features
- Business applications integration
- Power Automate flows

## Available APIs

### AI Services APIs

- **Retrieval API**: `docs/api/ai-services/retrieval/overview.md`
- **Search API**: `docs/api/ai-services/search/overview.md`
- **Chat API**: `docs/api/ai-services/chat/overview.md`
- **Meeting Insights API**: AI-generated meeting notes and action items
- **Interaction Export API**: Export user interactions for governance

### Admin APIs

- **Admin Settings**: `docs/api/admin-settings/`

## Agent Capabilities

Built-in features you can add to agents:

- **Code Interpreter**: `docs/code-interpreter.md`
- **Image Generator**: `docs/image-generator.md`
- **Knowledge Sources**: `docs/knowledge-sources.md`
- **Document Interaction**: `docs/declarative-agent-document-interaction.md`

## Essential Best Practices Documents

- `docs/declarative-agent-best-practices.md` - Agent development best practices
- `docs/declarative-agent-instructions.md` - Writing effective instructions
- `docs/instructions-api-plugins.md` - Instructions for agents with plugins
- `docs/openapi-document-guidance.md` - OpenAPI specification best practices
- `docs/optimize-content-retrieval.md` - Content retrieval optimization

## Testing and Debugging

- **Copilot Studio**: `docs/debugging-agents-copilot-studio.md`
- **VS Code/Agents Toolkit**: `docs/debugging-agents-vscode.md`

## Publishing and Management

- **Publishing**: `docs/publish.md`
- **Management**: `docs/manage.md`

## File Structure Cheat Sheet

```text
docs/
├── overview.md                      # Start here
├── agents-overview.md               # Agent types
├── overview-declarative-agent.md    # Declarative agents
├── overview-custom-engine-agent.md  # Custom engine agents
├── overview-api-plugins.md          # API plugins
├── overview-copilot-connector.md    # Connectors
├── copilot-apis-overview.md         # Copilot APIs
├── api/                             # API reference docs
│   ├── ai-services/                 # AI services APIs
│   └── admin-settings/              # Admin APIs
├── includes/                        # Reusable content
│   └── sample-manifests/            # Example JSON manifests
└── assets/                          # Images and resources
```

## Configuration Files

- `.markdownlint.json` - Linting rules
- `cspell.json` - Spell check dictionary
- `docs/docfx.json` - DocFX build config
- `.openpublishing.publish.config.json` - Publishing config
- `docs/TOC.yml` - Table of contents

## Troubleshooting Common Issues

### MD004 Lint Error

**Problem**: Using asterisks (*) for lists

**Solution**: Use dashes (-) instead

### Unknown Word in cspell

**Problem**: Valid word not recognized

**Solution**: Add to `cspell.json` "words" array

### Missing Newline (MD047)

**Problem**: File doesn't end with newline

**Solution**: Add single blank line at end of file

### Trailing Spaces (MD009)

**Problem**: Whitespace at end of lines

**Solution**: Remove trailing spaces

## YAML Front Matter Template

```yaml
---
title: Page title here
description: Brief description here
author: GitHub-username
ms.author: microsoft-alias
ms.topic: conceptual
ms.localizationpriority: medium
ms.date: 10/22/2025
---
```

## Key Resources

- **Published Docs**: <https://learn.microsoft.com/m365copilot/extensibility>
- **Style Guide**: <https://learn.microsoft.com/style-guide/welcome/>
- **Repository Index**: See `REPOSITORY_INDEX.md` for comprehensive reference
- **Contributing**: See `CONTRIBUTING.md`

## Support

- **FAQ**: `docs/faq.md`
- **Known Issues**: `docs/known-issues.md`
- **Feedback**: `docs/feedback.md`

## Statistics

- 178 Markdown files
- 16 YAML files
- 10+ agent templates
- 5+ manifest versions
- Multiple API services

---

For comprehensive repository documentation, see `REPOSITORY_INDEX.md`.
