# Antigravity MCPs & Agent Library

A comprehensive set of MCPs, specialized agents, and prompt templates for productive development with Google Antigravity.

This library is inspired by [Edmund's Claude Code setup](https://github.com/edmund-io/edmunds-claude-code) but adapted for Antigravity's agent-first architecture.

## Overview

This repository provides:

- **11 Specialized Agents**: Pre-configured agents for architecture, code quality, planning, and documentation
- **System Prompts**: Base system prompts and project brief templates
- **Command Patterns**: Reusable workflows for common development tasks
- **MCP Configurations**: Setup guides for integrating MCPs with your agents

## Quick Start

1. Clone this repo into your project or reference it when setting up a new Antigravity project
2. Copy the `.antigravity/` directory structure into your project
3. When starting a new Antigravity project, reference the appropriate agent prompts and system prompts from this library
4. Customize agents and prompts as needed for your specific tech stack and project requirements

## Directory Structure

```
.antigravity/
├── agents/                    # Specialized agent definitions
│   ├── architecture/          # System design & architecture agents
│   ├── code-quality/          # Code review, performance, security agents
│   ├── planning/              # Requirements, planning, research agents
│   └── documentation/         # Documentation & learning agents
├── commands/                  # Common command/workflow patterns
├── system-prompts/            # Base prompts and templates
└── README.md                  # This file
```

## Agents

### Architecture & Planning

- **system-architect**: Scalable system architecture design with trade-offs
- **backend-architect**: Backend systems with data integrity & security
- **frontend-architect**: Performant, accessible UI architecture
- **requirements-analyst**: Transform ideas into concrete specifications
- **tech-stack-researcher**: Technology choice recommendations with evidence

### Code Quality & Performance

- **refactoring-expert**: Systematic refactoring and clean code principles
- **performance-engineer**: Measurement-driven optimization strategies
- **security-engineer**: Vulnerability identification and security standards

### Documentation & Research

- **technical-writer**: Clear, comprehensive documentation generation
- **learning-guide**: Teaching programming concepts progressively
- **deep-research-agent**: Comprehensive research with adaptive strategies

## How to Use in Antigravity

### For Architecture Decisions

1. Start a new project in Antigravity
2. Copy the `system-architect` agent prompt into your project brief
3. Describe your project requirements
4. Let the agent plan the architecture, then use specialized agents (backend-architect, frontend-architect) for deeper dives

### For Feature Implementation

1. Use the `requirements-analyst` agent to transform your feature idea into specifications
2. Use `feature-plan` command to break it into implementation steps
3. Use `system-architect` or domain-specific architects to design the solution
4. Delegate implementation to Antigravity agents

### For Code Quality Reviews

1. Use the `refactoring-expert` agent to identify improvement areas
2. Use `performance-engineer` to measure and optimize
3. Use `security-engineer` to audit for vulnerabilities

## System Prompts

Each project should start with the **base-system-prompt** and be tailored with your specific project context using **project-brief-template**.

## MCPs & Tools

This library works with:

- **Filesystem MCP**: For reading/writing project files
- **Web Search MCP**: For research and tech stack decisions
- **Custom Tool MCPs**: As needed for your specific project

## Customization

Feel free to:

- Fork and customize agents for your tech stack
- Add new agents for domain-specific work
- Modify prompts based on your team's standards
- Extend with additional MCPs

## Tech Stack Notes

This library is designed to work with any modern tech stack. Examples include:

- Frontend: React, Vue, Angular, Svelte
- Backend: Node.js, Python, Go, Rust, Java
- Databases: PostgreSQL, MongoDB, Firebase
- Full-stack: Next.js, SvelteKit, Remix, etc.

## License

MIT - Use freely in your projects

## Contributing

Have improvements? Submit a PR or open an issue.

---

Created as a community resource for productive Antigravity development.
