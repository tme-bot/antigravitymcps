# How to Use the Antigravity MCPs Library

This guide explains how to use this library effectively in your Antigravity projects.

## Getting Started with a New Project

### Step 1: Clone or Copy the Library

```bash
git clone https://github.com/tme-bot/antigravitymcps.git
# Or copy the .antigravity directory into your project
```

### Step 2: Start with the Base System Prompt

1. Open `.antigravity/system-prompts/base-system-prompt.md`
2. Read through the core principles and development process
3. Customize the Project Brief section with your specific project details
4. Use this as your initial brief when creating a new Antigravity project

### Step 3: Create Your Project Brief

Fill in the Project Brief Template with your project details:

```markdown
# Project: [Your Project Name]

## Vision
[What you're building and why]

## Goals
- [Goal 1]
- [Goal 2]

## Requirements
- [Requirement 1]
- [Requirement 2]

[... complete the template ...]
```

### Step 4: Start Your Antigravity Project

In Google Antigravity, create a new project and paste your customized base system prompt + project brief as your Mission Brief.

## Using the Specialized Agents

### When Do You Need Each Agent?

**Starting a new project?** → Start with **system-architect** or **requirements-analyst**

**Designing backend systems?** → Use **backend-architect**

**Building user interfaces?** → Use **frontend-architect**

**Making technology choices?** → Ask **tech-stack-researcher**

**Your code feels messy?** → Consult **refactoring-expert**

**Performance is slow?** → Engage **performance-engineer**

**Need to secure something?** → Ask **security-engineer**

**Need to explain something?** → Use **learning-guide** or **technical-writer**

### How to Use an Agent

1. **Identify the Task**: What are you trying to accomplish?
2. **Find the Right Agent**: Look in `.antigravity/agents/[category]/`
3. **Copy the Agent Prompt**: Get the full prompt text
4. **Create a Task in Antigravity**: 
   - Describe what you need done
   - Paste the agent prompt into your task
   - Provide your specific context and requirements
5. **Let the Agent Work**: Antigravity will execute with that specialized prompt
6. **Review and Iterate**: Ask follow-up questions or request adjustments

## Example Workflows

### Workflow 1: Starting a New Web Application

1. Create Project Brief with vision and goals
2. Use **requirements-analyst** to refine requirements
3. Use **system-architect** to design overall architecture
4. Use **backend-architect** to design API and database
5. Use **frontend-architect** to design UI components
6. Use **tech-stack-researcher** for specific technology questions
7. Begin implementation with Antigravity agents

### Workflow 2: Building a Feature

1. Use **requirements-analyst** to define feature requirements
2. Use **system-architect** or domain-specific architect to design
3. Implement the feature with Antigravity
4. Use **refactoring-expert** to improve code quality
5. Use **security-engineer** for security review
6. Use **performance-engineer** for optimization
7. Use **technical-writer** to document the feature

### Workflow 3: Code Review & Improvement

1. Use **refactoring-expert** to identify improvements
2. Use **security-engineer** to check for vulnerabilities
3. Use **performance-engineer** to spot optimization opportunities
4. Use **tech-stack-researcher** to validate dependencies
5. Make improvements based on recommendations

## File Organization

```
.antigravity/
├── agents/
│   ├── architecture/
│   │   ├── system-architect.md          # Overall system design
│   │   ├── backend-architect.md         # Backend/API design
│   │   └── frontend-architect.md        # UI/component design
│   ├── code-quality/
│   │   ├── refactoring-expert.md        # Code improvement
│   │   ├── performance-engineer.md      # Performance optimization
│   │   └── security-engineer.md         # Security review
│   ├── planning/
│   │   ├── requirements-analyst.md      # Requirement refinement
│   │   ├── feature-planner.md           # Feature breakdown
│   │   └── tech-stack-researcher.md     # Technology recommendations
│   └── documentation/
│       ├── technical-writer.md          # Documentation
│       └── learning-guide.md            # Teaching/explaining
├── commands/
│   └── [Common workflow patterns]
└── system-prompts/
    ├── base-system-prompt.md            # Start here
    └── project-brief-template.md        # Fill this out
```

## Tips for Success

### Tip 1: Be Specific in Your Briefs

Instead of: "Build an API"
Try: "Build a REST API for a social media app that handles user posts with 100K daily users"

### Tip 2: Include Context

- What's the tech stack?
- What are performance requirements?
- Who are the users?
- What's the timeline?

### Tip 3: Use Agents Sequentially

Chain agents together for better results:
1. Start with requirements-analyst
2. Then system-architect
3. Then domain-specific architects
4. Then implementation

### Tip 4: Reference This Library

When asking Antigravity for something, you can say:
"Use the system-architect approach from the Antigravity MCPs library"
"Follow the backend-architect guidelines for API design"

### Tip 5: Iterate and Refine

- Start with high-level design
- Get feedback from Antigravity agents
- Refine based on their suggestions
- Move to implementation

### Tip 6: Keep Standards

Reference the base system prompt's Code Standards:
- Type safety (TypeScript, no `any`)
- Testing (unit tests for critical logic)
- Performance (measure before optimizing)
- Security (validate input)
- Maintainability (clear names, good structure)
- Accessibility (WCAG 2.1 AA for UIs)

## Customizing the Library

Feel free to:

- **Add Project Templates**: Create `.antigravity/templates/` with templates for common project types
- **Add Examples**: Create `.antigravity/examples/` with real project examples
- **Modify Agents**: Customize agents for your team's preferences
- **Add Domain Agents**: Create new agents for your specific domain
- **Create Workflows**: Document common patterns you discover

## Common Questions

**Q: Which agent should I start with?**
A: Start with requirements-analyst to clarify what you're building, then system-architect for overall design.

**Q: Can I use multiple agents on the same task?**
A: Yes! That's recommended. Use specialized agents in sequence for better results.

**Q: Should I copy the entire agent prompt?**
A: Yes, copy the full prompt into Antigravity when starting a task with that agent.

**Q: Can I modify the agents?**
A: Absolutely. Customize them for your team's preferences and tech stack.

**Q: How do I track decisions?**
A: Keep a DECISIONS.md file in your project documenting why you made key choices.

## Contributing Back

If you create useful agents, workflows, or templates, consider:
- Creating a pull request to share improvements
- Documenting what works well for your use cases
- Suggesting modifications to existing agents

## Next Steps

1. **Read the README**: Open the main README.md for overview
2. **Read base-system-prompt.md**: Understand the approach
3. **Skim the agents**: Get familiar with what's available
4. **Create your first project brief**: Customize for your project
5. **Try an agent**: Pick a task and use the relevant agent
6. **Iterate**: Refine based on results

---

Happy building with Antigravity! 🚀
