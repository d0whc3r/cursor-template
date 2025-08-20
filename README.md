# Cursor Rules Template

> **⚠️ IMPORTANT:** This README is for the template repository only. It will NOT appear in projects created from this template.

## What is this?

A **GitHub template repository** that provides standardized AI development rules for [Cursor](https://cursor.sh) IDE. These rules establish consistent AI behavior patterns across development teams and projects.

## Repository Structure

```
.cursor/
├── rules/
│   ├── core.mdc              # Autonomous principal engineer doctrine
│   ├── concise.mdc           # Radical conciseness communication protocol
│   ├── no-absolute-right.mdc # Professional communication guidelines
│   ├── request.mdc           # Standard task execution protocol
│   ├── refresh.mdc           # Deep bug diagnosis protocol
│   ├── retro.mdc             # Post-session retrospective protocol
│   └── steering/             # Specialized steering document generators
│       ├── generator.mdc     # Generic steering document structure
│       ├── product.mdc       # Product strategy steering
│       ├── structure.mdc     # Organizational structure steering
│       └── tech.mdc          # Technical architecture steering
└── mcp.json                  # MCP server configuration
```

## How to Use This Template

### 1. Create New Repository

- Click "Use this template" on GitHub
- Choose "Create a new repository"
- Your new repo will inherit all rules and configurations

### 2. Customize Rules (Optional)

- Modify `.cursor/rules/*.mdc` files to match your team's needs
- Add/remove steering document types
- Adjust MCP server configurations

### 3. Start Development

- Clone your new repository
- Open in Cursor IDE
- AI will automatically follow your established rule patterns

## Key Features

### **Autonomous Development Protocol**

- **Phase 0:** Reconnaissance & mental modeling
- **Phase 1:** Planning & strategy
- **Phase 2:** Execution & implementation
- **Phase 3:** Verification & autonomous correction
- **Phase 4:** Zero-trust self-audit

### **Communication Standards**

- Radical conciseness (maximum signal, minimum noise)
- Professional, non-sycophantic language
- Structured data over prose
- Fact-based reporting

### **Quality Assurance**

- Read-before-write protocols
- System-wide impact analysis
- Autonomous error correction
- End-to-end verification

## MCP Server Integration

This template includes pre-configured MCP servers:

- **Context7:** Enhanced documentation access
- **Sequential Thinking:** Advanced problem-solving
- **Git:** Version control operations

## Documentation

For comprehensive information about how these rules work and how to use them effectively, see the **[Documentation](./docs/)** folder. The documentation includes:

- **Rules Overview** - Understanding the rule system architecture
- **Core Rules** - Essential behavioral patterns and protocols
- **Task Protocols** - Specialized execution workflows
- **Steering Documents** - Document generation templates
- **Usage Examples** - Practical implementation scenarios
- **Customization Guide** - Adapting rules for your team

## Customization Guide

### Adding New Rules

1. Create `.mdc` file in `.cursor/rules/`
2. Follow existing rule structure patterns
3. Use `alwaysApply: true/false` for global vs. conditional rules

### Modifying Existing Rules

- Core rules (`core.mdc`, `concise.mdc`) should remain stable
- Task-specific rules can be customized per project needs
- Maintain rule hierarchy and dependencies

### Rule Categories

- **Always Applied:** Core behavioral patterns
- **Conditional:** Context-specific protocols
- **Steering:** Document generation templates

## Best Practices

1. **Version Control:** Commit rule changes with clear messages
2. **Team Alignment:** Review rule modifications with team members
3. **Documentation:** Update this README when adding new rule types
4. **Testing:** Verify rules work correctly in new projects

## Support

- **Issues:** Report bugs or request features via GitHub Issues
- **Discussions:** Share usage patterns and best practices
- **Contributions:** Submit pull requests for rule improvements

---

**Note:** This template is designed for teams using Cursor IDE with AI assistance. Ensure all team members understand the established protocols before deployment.
