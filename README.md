# clean

A repository equipped with a suite of AI-powered code analysis and documentation agents.

## Overview

This repository contains a set of specialised GitHub Copilot agents (defined in `.github/agents/`) that orchestrate comprehensive source-code analysis and documentation generation tasks.

## Available Agents

| Agent | Purpose |
|-------|---------|
| `orchestrator` | Main coordinator — launches and combines output from all specialist agents |
| `code-documentor` | Generates source-code documentation and extracts business logic |
| `code-assessor` | Assesses code quality, identifies technical debt, and suggests improvements |
| `architecture-analyzer` | Produces cloud and component architecture diagrams |
| `ast-analyzer` | Generates Abstract Syntax Trees and structural analysis |
| `uml-generator` | Creates UML diagrams (Class, Sequence, Use Case) in Mermaid format |
| `bpmn-generator` | Generates BPMN 2.0 process diagrams from workflow analysis |
| `ddl-generator` | Produces SQL DDL files from workflow and field documentation |
| `arc42-documentor` | Synthesises all analyses into an Arc42 architecture document |
| `documentation-analyzer` | Audits existing documentation quality and identifies gaps |
| `executive-summary` | Creates concise executive summaries for decision-makers |
| `all-in-one-agent` | Single-pass agent combining documentation, quality, and diagram generation |

## Usage

Invoke any agent from a GitHub Copilot chat by referencing its name, for example:

```
/agent orchestrator analyse the codebase and generate full documentation
```

Or trigger a targeted specialist:

```
/agent uml-generator create a class diagram for the payment module
```

## Getting Started

1. Open a Copilot chat session in this repository.
2. Call `/agent orchestrator do start docu` to run a full documentation pass.
3. Review the generated artefacts committed back to the repository.

## Repository Structure

```
.
├── README.md                  # This file
└── .github/
    └── agents/                # Agent definition files
        ├── orchestrator.agent.md
        ├── code-documentor.agent.md
        ├── code-assessor.agent.md
        ├── architecture-analyzer.agent.md
        ├── ast-analyzer.agent.md
        ├── uml-generator.agent.md
        ├── bpmn-generator.agent.md
        ├── ddl-generator.agent.md
        ├── arc42-documentor.agent.md
        ├── documentation-analyzer.agent.md
        ├── executive-summary.agent.md
        └── all-in-one-agent.md
```
