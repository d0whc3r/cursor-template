# Rules Overview

## What are Cursor Rules?

Cursor Rules are `.mdc` files that define AI behavior patterns in Cursor IDE. They transform the AI from a simple command executor into an **Autonomous Principal Engineer** following disciplined, evidence-first workflows.

## Rule System Architecture

### 1. **Core Doctrine** (`core.mdc`)

- **Purpose**: Central "constitution" governing all AI behavior
- **Scope**: Universal, technology-agnostic principles
- **Installation**: Must be installed as primary system instruction
- **Behavior**: Defines identity, research protocols, safety guardrails, professional standards

### 2. **Communication Protocols** (`concise.mdc`, `no-absolute-right.mdc`)

- **Purpose**: Establish professional communication standards
- **Scope**: Language patterns, tone, information density
- **Behavior**: Radical conciseness, professional language, fact-based reporting

### 3. **Task Execution Protocols** (`request.mdc`, `refresh.mdc`, `retro.mdc`)

- **Purpose**: Structured workflows for different task types
- **Scope**: Task-specific execution patterns
- **Behavior**: Phased execution, verification, self-audit

### 4. **Steering Documents** (`steering/*.mdc`)

- **Purpose**: Generate structured documents for decision-making
- **Scope**: Product strategy, technical architecture, organizational structure
- **Behavior**: Template-based document generation

### 5. **Verification Protocols** (`testing.mdc`)

- **Purpose**: Define protocols for testing and quality assurance
- **Scope**: Automated testing, manual verification, quality gates
- **Behavior**: Ensures code quality and adherence to standards

## How Rules Work

### **Rule Hierarchy**

```
core.mdc (Always Applied)
├── concise.mdc (Always Applied)
├── no-absolute-right.mdc (Always Applied)
├── request.mdc (Conditional)
├── refresh.mdc (Conditional)
├── retro.mdc (Conditional)
├── steering/*.mdc (Conditional)
└── testing.mdc (Conditional)
```

### **Rule Application**

- **Always Applied**: Core behavioral patterns active in every interaction
- **Conditional**: Activated by specific playbooks or user requests
- **Stackable**: Multiple rules can be combined for complex behaviors

### **Rule Execution Flow**

1. **Installation**: Core rules establish baseline behavior
2. **Activation**: Playbooks activate specific protocols
3. **Execution**: AI follows established patterns
4. **Verification**: Self-audit ensures compliance
5. **Evolution**: Retro sessions improve rules over time

## Rule Categories

### **Behavioral Rules**

- Define how AI thinks, communicates, and operates
- Establish professional standards and safety protocols
- Create consistent interaction patterns

### **Workflow Rules**

- Define structured approaches to different task types
- Ensure systematic problem-solving
- Maintain quality and consistency

### **Output Rules**

- Define document and code generation patterns
- Establish formatting and structure standards
- Ensure professional presentation

## Benefits of Using Rules

### **For Developers**

- **Consistency**: Predictable AI behavior across projects
- **Quality**: Systematic approaches to problem-solving
- **Efficiency**: Reduced need for repetitive instructions
- **Learning**: AI improves over time through structured feedback

### **For Teams**

- **Alignment**: Shared development protocols
- **Onboarding**: New team members inherit established patterns
- **Quality Assurance**: Consistent code and documentation standards
- **Knowledge Retention**: Rules capture team best practices

### **For Organizations**

- **Scalability**: Rules can be shared across multiple projects
- **Compliance**: Enforce development standards and practices
- **Innovation**: AI learns and improves organizational processes
- **Risk Management**: Systematic approaches reduce development risks

## Rule Lifecycle

### **1. Installation**

- Core rules establish baseline behavior
- Rules become active immediately
- AI begins operating under new protocols

### **2. Operation**

- AI follows established patterns
- Rules guide decision-making and execution
- Consistent behavior across interactions

### **3. Evaluation**

- Retro sessions assess rule effectiveness
- Identify areas for improvement
- Capture lessons learned

### **4. Evolution**

- Rules are updated based on feedback
- New patterns are incorporated
- System becomes more effective over time

## Integration with Cursor IDE

### **File Placement**

- Rules are placed in `.cursor/rules/` directory
- Cursor automatically recognizes and applies rules
- Rules can be project-specific or global

### **Rule Format**

- **File Extension**: `.mdc` (Markdown with Cursor extensions)
- **Metadata**: YAML frontmatter for configuration
- **Content**: Markdown with specific directives and examples

### **Activation Methods**

- **Automatic**: Core rules activate on project open
- **Manual**: Playbooks activate specific protocols
- **Conditional**: Rules activate based on context or user input

---

_This overview is based on the [Autonomous Agent Prompting Framework](https://gist.github.com/aashari/07cc9c1b6c0debbeb4f4d94a3a81339e) by aashari_
