# Microsoft 365 Copilot Extensibility Documentation Repository Index

This index provides a comprehensive summary of the Microsoft 365 Copilot extensibility documentation repository, highlighting key topics, structure, and resources.

## Repository Overview

**Purpose**: Source repository for Microsoft 365 Copilot extensibility documentation published to [Microsoft Learn](https://learn.microsoft.com/m365copilot/extensibility).

**Content Statistics**:

- 178 Markdown documentation files
- 16 YAML configuration files
- Documentation-only repository (no application code)
- Uses OpenPublishing system with DocFX for building and publishing

## Key Documentation Areas

### 1. Microsoft 365 Copilot Extensibility Overview

**Main Document**: `docs/overview.md`

Microsoft 365 Copilot can be extended in three primary ways:

- **Copilot Connectors**: Ingest and index organizational data from multiple sources
- **Agents**: AI-powered assistants for specialized workflows and automation
- **Microsoft 365 Copilot APIs**: Programmatic access to Copilot capabilities

### 2. Agents for Microsoft 365 Copilot

**Main Document**: `docs/agents-overview.md`

#### Declarative Agents

**Overview**: `docs/overview-declarative-agent.md`

Declarative agents utilize Copilot's orchestrator and models with custom instructions, knowledge, and actions.

**Key Topics**:

- Building with TypeSpec (TypeSpec-based development approach)
  - `docs/overview-typespec.md`
  - `docs/build-declarative-agents-typespec.md`
  - `docs/typespec-scenarios.md`
  - `docs/typespec-authentication.md`
  - `docs/typespec-decorators.md`
  - `docs/typespec-capabilities.md`
- Building with JSON (manifest-based approach)
  - `docs/build-declarative-agents.md`
  - `docs/build-declarative-agents-customize-behavior.md`
  - `docs/build-declarative-agents-add-knowledge.md`
  - `docs/build-declarative-agents-add-skills.md`

**Manifest References**:

- Version 1.5: `docs/declarative-agent-manifest-1.5.md`
- Version 1.4: `docs/declarative-agent-manifest-1.4.md`
- Version 1.3: `docs/declarative-agent-manifest-1.3.md`
- Version 1.2: `docs/declarative-agent-manifest-1.2.md`
- Version 1.0: `docs/declarative-agent-manifest-1.0.md`

**Best Practices**:

- `docs/declarative-agent-best-practices.md`
- `docs/declarative-agent-instructions.md`
- `docs/instructions-api-plugins.md`

#### Custom Engine Agents

**Overview**: `docs/overview-custom-engine-agent.md`

Custom engine agents use your own orchestrator and models for fully tailored solutions.

**Development Options**:

- **Microsoft 365 Agents SDK**: `docs/m365-agents-sdk.md`
  - Create and deploy: `docs/create-deploy-agents-sdk.md`
- **Teams AI Library**: `docs/teams-ai-library.md`
- **Microsoft Copilot Studio**: Full-featured agent development platform

**User Experience**:

- `docs/ux-custom-engine-agent.md`
- `docs/custom-engine-agent-asynchronous-flow.md`

#### Agent Templates

**Overview**: `docs/agent-templates-overview.md`

Pre-built agent templates for common scenarios:

1. **Career Coach**: `docs/agent-template-career-coach.md`
2. **Customer Insight Assistant**: `docs/agent-template-customer-insight.md`
3. **Idea Coach**: `docs/agent-template-idea-coach.md`
4. **Interview Question Assistant**: `docs/agent-template-interview-questions.md`
5. **Learning Coach**: `docs/agent-template-learning-coach.md`
6. **Meeting Coach**: `docs/agent-template-meeting-coach.md`
7. **Prompt Coach**: `docs/agent-template-prompt-coach.md`
8. **Quiz Tutor**: `docs/agent-template-quiz-tutor.md`
9. **Scrum Assistant**: `docs/agent-template-scrum-assistant.md`
10. **Writing Coach**: `docs/agent-template-writing-coach.md`

### 3. API Plugins

**Overview**: `docs/overview-api-plugins.md`

API plugins add custom actions and capabilities to declarative agents.

**Building API Plugins**:

- With TypeSpec: `docs/build-api-plugins-typespec.md`
- With new API: `docs/build-api-plugins-new-api.md`
- From existing API: `docs/build-api-plugins-existing-api.md`
- With Office JavaScript API: `docs/build-api-plugins-local-office-api.md`

**Advanced Features**:

- Authentication: `docs/api-plugin-authentication.md`
- Adaptive Card responses: `docs/api-plugin-adaptive-cards.md`
- Dialog boxes: `docs/adaptive-card-dialog-box.md`
- Confirmation prompts: `docs/api-plugin-confirmation-prompts.md`
- Debug locally: `docs/api-plugin-debug-local.md`

**Manifest References**:

- Version 2.3: `docs/api-plugin-manifest-2.3.md`
- Version 2.2: `docs/api-plugin-manifest-2.2.md`
- Version 2.1: `docs/api-plugin-manifest-2.1.md`

**Best Practices**:

- OpenAPI document guidance: `docs/openapi-document-guidance.md`

### 4. Copilot Connectors

**Overview**: `docs/overview-copilot-connector.md`

Copilot connectors ingest and index organizational data to enhance Copilot's knowledge.

**Key Resources**:

- Build your first connector: `docs/build-your-first-connector.md`
- Connectors with people data: `docs/build-connectors-with-people-data.md`
- Admin delegation: `docs/connector-admin-delegation.md`

### 5. Microsoft 365 Copilot APIs

**Overview**: `docs/copilot-apis-overview.md`

**API Documentation** (under `docs/api/`):

#### Retrieval API

- Overview: `docs/api/ai-services/retrieval/overview.md`
- Retrieve relevant information from Microsoft 365's semantic and lexical indexes

#### Search API

- Overview: `docs/api/ai-services/search/overview.md`
- Hybrid search across OneDrive content using natural language

#### Chat API

- Overview: `docs/api/ai-services/chat/overview.md`
- Send prompts directly to Copilot for conversational experiences

#### Interaction Export API

- Export user interactions with Copilot for governance and analytics

#### AI Meeting Insights API

- Access AI-generated notes, action items, and mentions from Teams meetings

#### Admin Settings API

- Located in `docs/api/admin-settings/`
- Manage Copilot admin settings programmatically

### 6. Copilot Studio Experiences

**Copilot Studio Lite**:

- Overview: `docs/copilot-studio-lite.md`
- Build agents: `docs/copilot-studio-lite-build.md`
- Fine-tuned models: `docs/copilot-studio-lite-tuned-models.md`
- Knowledge sources: `docs/copilot-studio-lite-knowledge.md`
- Share and manage: `docs/copilot-studio-lite-share-manage-agent.md`
- Availability: `docs/copilot-studio-lite-availability.md`

**Full Experience**:

- Copy to Copilot Studio: `docs/copy-agent-to-copilot-studio.md`
- Business applications: `docs/overview-business-applications.md`
- Copilot Studio experience: `docs/copilot-studio-experience.md`

### 7. Agent Capabilities and Features

**Capabilities**:

- Code interpreter: `docs/code-interpreter.md`
- Image generator: `docs/image-generator.md`
- Knowledge sources: `docs/knowledge-sources.md`
- Document interaction: `docs/declarative-agent-document-interaction.md`

**Configuration and Optimization**:

- Capabilities IDs: `docs/declarative-agent-capabilities-ids.md`
- Optimize content retrieval: `docs/optimize-content-retrieval.md`
- Enable user feedback: `docs/declarative-agent-enable-feedback.md`

**Localization**:

- Localize agents: `docs/localize-agents.md`

### 8. Testing and Debugging

- Debug with Copilot Studio: `docs/debugging-agents-copilot-studio.md`
- Debug with VS Code (Agents Toolkit): `docs/debugging-agents-vscode.md`

### 9. Publishing and Management

**Publishing**:

- Overview: `docs/publish.md`

**Management**:

- Overview: `docs/manage.md`

### 10. Getting Started and Planning

**Prerequisites and Setup**:

- Prerequisites: `docs/prerequisites.md`
- Planning guide: `docs/planning-guide.md`
- Cost considerations: `docs/cost-considerations.md`

**Conceptual Understanding**:

- Ecosystem: `docs/ecosystem.md`
- Agents are apps: `docs/agents-are-apps.md`
- Orchestrator: `docs/orchestrator.md`
- Data privacy and security: `docs/data-privacy-security.md`

**Resources**:

- Samples: `docs/samples.md`
- What's new: `docs/whats-new.md`
- What's new history: `docs/whats-new-history.md`

### 11. Additional Resources

**Support and Feedback**:

- FAQ: `docs/faq.md`
- Transparency FAQ: `docs/transparency-faq-declarative-agent.md`
- Known issues: `docs/known-issues.md`
- Feedback: `docs/feedback.md`

**Validation and Compliance**:

- RAI validation: `docs/rai-validation.md`
- Tool comparison: `docs/declarative-agent-tool-comparison.md`

**Advanced Topics**:

- Convert declarative to custom engine: `docs/convert-declarative-agent.md`
- Graph actions with Semantic Kernel: `docs/graph-actions-semantic-kernel.md`
- Message extension bots: `docs/overview-message-extension-bot.md`
- Bring agents to Copilot: `docs/bring-agents-to-copilot.md`

## Repository Structure

```text
/
├── docs/                           # Main documentation directory
│   ├── api/                        # API reference documentation
│   │   ├── ai-services/            # AI services APIs
│   │   │   ├── chat/               # Chat API docs
│   │   │   ├── retrieval/          # Retrieval API docs
│   │   │   ├── search/             # Search API docs
│   │   │   ├── meeting-insights/   # Meeting insights API docs
│   │   │   └── interaction-export/ # Interaction export API docs
│   │   ├── admin-settings/         # Admin settings API docs
│   │   ├── resources/              # API resource documentation
│   │   └── includes/               # API code snippets
│   ├── assets/                     # Images and supporting files
│   │   ├── images/                 # Documentation images
│   │   └── scripts/                # PowerShell utility scripts
│   ├── includes/                   # Reusable content snippets
│   │   └── sample-manifests/       # JSON manifest examples
│   ├── breadcrumb/                 # Breadcrumb navigation
│   ├── sdks/                       # SDK documentation
│   ├── TOC.yml                     # Table of contents
│   ├── docfx.json                  # DocFX configuration
│   ├── index.yml                   # Landing page
│   └── *.md                        # 98 top-level markdown files
├── scripts/                        # Repository maintenance scripts
│   └── CleanupUnusedImages.ps1     # Image cleanup utility
├── templates/                      # Documentation templates
├── redirects/                      # URL redirects configuration
├── .github/                        # GitHub workflows and settings
├── .markdownlint.json              # Markdown linting rules
├── cspell.json                     # Spell checking dictionary
├── .openpublishing.publish.config.json  # OpenPublishing configuration
├── .acrolinx-config.edn            # Content quality scoring
├── README.md                       # Repository readme
├── CONTRIBUTING.md                 # Contribution guidelines
└── REPOSITORY_INDEX.md             # This file
```

## Validation and Build Process

### Local Validation Tools

**Markdown Linting**:

```bash
markdownlint docs --config .markdownlint.json --ignore **\node_modules\**
```

- Expected time: ~3 seconds
- Must pass with zero errors before committing

**Spell Checking**:

```bash
cspell --config cspell.json "docs/**/*.md"
```

- Expected time: ~3 seconds
- Add valid words to `cspell.json`

**Image Cleanup**:

```bash
pwsh scripts/CleanupUnusedImages.ps1
```

- Expected time: ~45-50 seconds
- Removes unused images from assets directory

### CI/CD Validation

**OpenPublishing Build**: Runs automatically on pull requests (5-10 minutes)

**Acrolinx Content Quality**: Runs automatically on pull requests (2-5 minutes)

- Minimum score required: 80

**EOL Blocker Validation**: GitHub Actions workflow to prevent end-of-life issues

## Development Workflow

### Required Tools

- PowerShell Core (pwsh)
- Node.js and npm
- markdownlint-cli
- cspell
- Visual Studio Code (recommended)
- Learn Authoring Pack extension (recommended)

### Authoring Guidelines

**Style Guide**: Follow the [Microsoft Writing Style Guide](https://learn.microsoft.com/style-guide/welcome/)

**Markdown Conventions**:

- Use dashes (-) for unordered lists, not asterisks (*)
- Files must end with a single newline character
- No trailing whitespace
- No hard tabs (use spaces)
- Proper heading hierarchy (no skipped levels)

**YAML Front Matter** (required for all .md files):

```yaml
---
title: Page title
description: Brief description
author: GitHub username
ms.author: Microsoft alias
ms.topic: topic-type
ms.localizationpriority: priority-level
ms.date: MM/dd/yyyy
---
```

### Includes and Reusable Content

**Location**: `docs/includes/`

**Sample Manifests**: `docs/includes/sample-manifests/`

- Declarative agent manifests (versions 1.0-1.5)
- API plugin manifests (versions 2.1-2.3)

## Table of Contents (TOC) Structure

The `docs/TOC.yml` file organizes documentation into the following main sections:

1. Microsoft 365 Copilot extensibility (landing page)
2. Overview
3. Explore
4. What's new
5. Get started
6. Build an agent
   - Agents overview
   - Build a declarative agent
   - Build a custom engine agent
7. Add knowledge with Copilot connectors
8. Enhance AI solutions with Microsoft 365 Copilot APIs
9. Publish
10. Manage
11. FAQ
12. Known issues
13. Support and feedback

## Key Concepts and Terminology

**Agent**: An AI-powered assistant that extends Copilot with specialized knowledge and skills

**Declarative Agent**: An agent built using Copilot's orchestrator and models with custom configuration

**Custom Engine Agent**: An agent that uses custom orchestrators and models

**API Plugin**: Extends declarative agents with custom actions via OpenAPI specifications

**Copilot Connector**: Ingests and indexes organizational data for Copilot access

**TypeSpec**: A language for describing cloud service APIs and generating client libraries

**Orchestrator**: The engine that manages agent interactions with knowledge, skills, and autonomy

**Foundation Models**: LLMs powering agent reasoning and response generation

**Knowledge Sources**: Data sources that provide context to agents (SharePoint, OneDrive, files, etc.)

**Capabilities**: Built-in features like code interpreter and image generator

## Navigation Quick Reference

### For Beginners

Start with:

1. `docs/overview.md` - High-level overview of extensibility options
2. `docs/planning-guide.md` - Planning your extensibility solution
3. `docs/prerequisites.md` - Setting up your development environment
4. `docs/agents-overview.md` - Understanding agents

### For Declarative Agent Developers

Key files:

1. `docs/overview-declarative-agent.md` - Declarative agent overview
2. `docs/build-declarative-agents.md` - Building with JSON
3. `docs/build-declarative-agents-typespec.md` - Building with TypeSpec
4. `docs/declarative-agent-manifest-1.5.md` - Latest manifest reference

### For Custom Engine Agent Developers

Key files:

1. `docs/overview-custom-engine-agent.md` - Custom engine overview
2. `docs/m365-agents-sdk.md` - Using the SDK
3. `docs/teams-ai-library.md` - Using Teams AI library

### For API Plugin Developers

Key files:

1. `docs/overview-api-plugins.md` - API plugins overview
2. `docs/build-api-plugins-typespec.md` - Building with TypeSpec
3. `docs/api-plugin-manifest-2.3.md` - Latest manifest reference
4. `docs/openapi-document-guidance.md` - Best practices

### For Connector Developers

Key files:

1. `docs/overview-copilot-connector.md` - Connectors overview
2. `docs/build-your-first-connector.md` - Getting started

### For API Integration Developers

Key files:

1. `docs/copilot-apis-overview.md` - APIs overview
2. `docs/api/ai-services/retrieval/overview.md` - Retrieval API
3. `docs/api/ai-services/search/overview.md` - Search API

## Contributing

See `CONTRIBUTING.md` for detailed contribution guidelines.

**Quick Guidelines**:

- Run validation before submitting pull requests
- Follow Microsoft Writing Style Guide
- Use Visual Studio Code with Learn Authoring Pack
- Ensure Acrolinx score is 80 or higher
- No hard tabs, proper formatting
- Update `ms.date` when making technical updates

## License

- Content: Licensed under Creative Commons Attribution 4.0 International
- Code samples: Licensed under MIT License

See `LICENSE` and `LICENSE-CODE` for details.

## Support and Feedback

- Documentation feedback: `docs/feedback.md`
- Known issues: `docs/known-issues.md`
- FAQ: `docs/faq.md`

## Related Resources

- Published documentation: <https://learn.microsoft.com/m365copilot/extensibility>
- Microsoft Copilot Studio: <https://learn.microsoft.com/microsoft-copilot-studio/>
- Microsoft Graph: <https://learn.microsoft.com/graph/>
- Microsoft Teams: <https://learn.microsoft.com/microsoftteams/>

---

**Last Updated**: This index was generated on October 22, 2025, based on repository commit at time of indexing.

**Maintenance**: Update this index when significant structural changes are made to the repository or when new major documentation sections are added.
