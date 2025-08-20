# Customization Guide

## Overview

This guide explains how to customize Cursor Rules for your specific team, project, or organization. Learn how to adapt the framework while maintaining its core principles and effectiveness.

## Customization Principles

### **Core Framework Preservation**

- **Maintain Core Doctrine**: Keep the 5-phase operational workflow
- **Preserve Communication Standards**: Maintain professional, concise communication
- **Keep Safety Protocols**: Maintain read-write-reread and verification patterns
- **Sustain Learning Loop**: Preserve retrospective and improvement mechanisms

### **Adaptation Areas**

- **Domain-Specific Rules**: Add industry or technology-specific protocols
- **Team Culture**: Adapt communication style to team preferences
- **Project Requirements**: Include project-specific quality gates
- **Organizational Standards**: Incorporate company policies and procedures

## Rule Customization Levels

### **Level 1: Configuration Changes**

- Modify existing rule parameters
- Adjust thresholds and limits
- Change status markers and symbols
- Update file paths and naming conventions

### **Level 2: Rule Extensions**

- Add new rule categories
- Extend existing protocols
- Include additional verification steps
- Add domain-specific requirements

### **Level 3: Framework Modifications**

- Create new operational phases
- Develop custom communication protocols
- Implement specialized quality gates
- Design new document templates

## Customization Examples

### **Example 1: Frontend Development Team**

#### **Custom Rules Added**

```markdown
# Frontend-Specific Rules

## Quality Gates

- Lighthouse score >90
- Bundle size <500KB
- Accessibility compliance (WCAG 2.1 AA)
- Cross-browser compatibility testing

## Development Standards

- Component library usage mandatory
- Storybook documentation required
- Unit test coverage >90%
- E2E tests for critical user flows

## Performance Requirements

- First Contentful Paint <1.5s
- Largest Contentful Paint <2.5s
- Cumulative Layout Shift <0.1
```

#### **Modified Communication Protocol**

```markdown
# Frontend Communication Standards

## Status Markers

- 🎨 UI/UX changes
- 🚀 Performance improvements
- ♿ Accessibility fixes
- 📱 Responsive design updates
- 🧪 Test coverage improvements

## Technical Language

- Use frontend-specific terminology
- Include browser compatibility notes
- Reference design system components
- Mention performance metrics
```

### **Example 2: DevOps/Infrastructure Team**

#### **Custom Rules Added**

```markdown
# Infrastructure-Specific Rules

## Security Requirements

- Infrastructure as Code (IaC) mandatory
- Secret management with Vault
- Network security group validation
- Compliance scanning (SOC2, PCI-DSS)

## Monitoring Standards

- 99.9% uptime SLA
- Response time <200ms
- Error rate <0.1%
- Resource utilization <80%

## Deployment Protocols

- Blue-green deployment strategy
- Automated rollback triggers
- Canary deployment for high-risk changes
- Multi-region failover testing
```

#### **Modified Verification Protocol**

```markdown
# Infrastructure Verification

## Phase 3: Infrastructure Verification

- **Security Scanning**: Run compliance checks
- **Performance Testing**: Load test infrastructure
- **Disaster Recovery**: Test failover procedures
- **Monitoring Validation**: Verify alerting systems
- **Documentation Update**: Update runbooks and procedures
```

### **Example 3: Data Science Team**

#### **Custom Rules Added**

```markdown
# Data Science-Specific Rules

## Data Quality Gates

- Data validation schema compliance
- Statistical significance testing
- Model performance metrics
- Bias and fairness assessment

## Research Standards

- Reproducible research practices
- Version control for datasets
- Experiment tracking and logging
- Peer review for model changes

## Ethical Considerations

- Privacy impact assessment
- Bias detection and mitigation
- Transparency in model decisions
- Human oversight requirements
```

#### **Modified Planning Protocol**

```markdown
# Data Science Planning

## Phase 1: Research Planning

- **Hypothesis Definition**: Clear research questions
- **Data Requirements**: Data sources and quality needs
- **Methodology Selection**: Statistical approach justification
- **Success Metrics**: Model performance targets
- **Ethical Review**: Privacy and bias considerations
```

## Customization Process

### **Step 1: Assessment**

1. **Team Analysis**: Understand team composition and expertise
2. **Project Requirements**: Identify specific needs and constraints
3. **Existing Standards**: Review current processes and tools
4. **Gap Analysis**: Identify areas needing customization

### **Step 2: Design**

1. **Rule Structure**: Plan new rule categories and relationships
2. **Integration Points**: Identify where custom rules fit
3. **Dependencies**: Map rule dependencies and conflicts
4. **Testing Strategy**: Plan how to validate custom rules

### **Step 3: Implementation**

1. **Rule Creation**: Write custom rule files
2. **Integration**: Add rules to existing framework
3. **Testing**: Validate rules with team members
4. **Documentation**: Update documentation and examples

### **Step 4: Validation**

1. **Team Feedback**: Gather input on rule effectiveness
2. **Process Testing**: Test rules in real scenarios
3. **Quality Assessment**: Measure impact on outcomes
4. **Iteration**: Refine rules based on feedback

## Custom Rule Templates

### **Template 1: Domain-Specific Protocol**

```markdown
---
description: [Domain] development protocol
alwaysApply: false
---

## [Domain] Development Protocol

### Purpose

[Describe the specific purpose and scope]

### When to Use

- [List specific scenarios]
- [Include trigger conditions]

### Protocol Flow

1. **[Phase Name]**: [Description]
2. **[Phase Name]**: [Description]
3. **[Phase Name]**: [Description]

### Quality Gates

- [Specific quality requirements]
- [Domain-specific metrics]
- [Compliance requirements]

### Examples

[Include practical examples]
```

### **Template 2: Quality Gate Extension**

```markdown
---
description: [Domain] quality gates
alwaysApply: false
---

## [Domain] Quality Gates

### Code Quality

- [Specific coding standards]
- [Style requirements]
- [Documentation needs]

### Testing Requirements

- [Test coverage targets]
- [Testing methodologies]
- [Quality metrics]

### Performance Standards

- [Performance benchmarks]
- [Resource limits]
- [Scalability requirements]

### Security Requirements

- [Security standards]
- [Vulnerability scanning]
- [Compliance needs]
```

### **Template 3: Communication Protocol**

```markdown
---
description: [Domain] communication standards
alwaysApply: false
---

## [Domain] Communication Standards

### Status Markers

- [Custom status symbols]
- [Domain-specific indicators]
- [Progress markers]

### Technical Language

- [Domain terminology]
- [Standard abbreviations]
- [Reference formats]

### Documentation Standards

- [Document formats]
- [Required sections]
- [Quality criteria]
```

## Integration Strategies

### **Rule Hierarchy Management**

```
core.mdc (Always Applied)
├── concise.mdc (Always Applied)
├── no-absolute-right.mdc (Always Applied)
├── domain-specific.mdc (Conditional)
├── project-specific.mdc (Conditional)
└── team-custom.mdc (Conditional)
```

### **Conflict Resolution**

1. **Priority System**: Establish rule precedence
2. **Conditional Application**: Use context-based activation
3. **Rule Composition**: Combine multiple rules intelligently
4. **Override Mechanisms**: Allow specific rule overrides

### **Performance Considerations**

1. **Rule Caching**: Cache frequently used rules
2. **Lazy Loading**: Load rules only when needed
3. **Optimization**: Minimize rule evaluation overhead
4. **Monitoring**: Track rule performance impact

## Testing Custom Rules

### **Validation Methods**

1. **Unit Testing**: Test individual rule components
2. **Integration Testing**: Test rule interactions
3. **Scenario Testing**: Test rules in realistic situations
4. **User Testing**: Validate with actual team members

### **Quality Metrics**

1. **Rule Effectiveness**: Measure impact on outcomes
2. **User Satisfaction**: Gather feedback on rule usefulness
3. **Process Efficiency**: Measure time and effort savings
4. **Quality Improvement**: Track quality metric changes

### **Iteration Process**

1. **Data Collection**: Gather performance data
2. **Analysis**: Identify improvement opportunities
3. **Rule Updates**: Modify rules based on findings
4. **Validation**: Test updated rules
5. **Deployment**: Roll out improved rules

## Best Practices

### **Customization Guidelines**

1. **Start Small**: Begin with minimal changes
2. **Test Thoroughly**: Validate all custom rules
3. **Document Everything**: Maintain clear documentation
4. **Gather Feedback**: Continuously improve rules
5. **Maintain Consistency**: Ensure rule coherence

### **Common Pitfalls**

1. **Over-Customization**: Too many rules can reduce effectiveness
2. **Rule Conflicts**: Conflicting rules can cause confusion
3. **Performance Impact**: Complex rules can slow down AI
4. **Maintenance Overhead**: Custom rules require ongoing maintenance
5. **Team Resistance**: Rules that don't fit team culture will fail

### **Success Factors**

1. **Team Buy-in**: Ensure team understands and supports rules
2. **Gradual Implementation**: Introduce changes incrementally
3. **Clear Communication**: Explain rule purpose and benefits
4. **Regular Review**: Continuously assess and improve rules
5. **Training**: Provide training on new rules and processes

## Maintenance and Evolution

### **Rule Lifecycle Management**

1. **Version Control**: Track rule changes over time
2. **Change Management**: Formalize rule modification process
3. **Deprecation Strategy**: Plan for rule retirement
4. **Migration Planning**: Handle rule updates and changes

### **Continuous Improvement**

1. **Regular Assessment**: Periodically review rule effectiveness
2. **Feedback Integration**: Incorporate user feedback
3. **Performance Monitoring**: Track rule performance metrics
4. **Innovation**: Explore new rule types and approaches

### **Knowledge Management**

1. **Documentation Updates**: Keep documentation current
2. **Training Materials**: Develop training for new rules
3. **Best Practices**: Document successful rule patterns
4. **Lessons Learned**: Capture improvement insights

---

**Note**: This customization guide applies to the core rules from the [Autonomous Agent Prompting Framework](https://gist.github.com/aashari/07cc9c1b6c0debbeb4f4d94a3a81339e) by aashari. For information about customizing template-specific rules, see the [Template Rules Documentation](./template-rules/).
