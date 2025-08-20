# Task Protocols

## Overview

Task protocols are structured workflows that activate specific AI behaviors for different types of tasks. These protocols ensure consistent, disciplined execution following the Autonomous Principal Engineer framework.

## Protocol Types

### **1. Standard Operating Protocol (`request.mdc`)**

#### **Purpose**

Standard procedure for constructive work: building features, refactoring code, or making planned changes.

#### **When to Use**

- New feature development
- Code refactoring
- System improvements
- Planned architectural changes
- Bug fixes with clear scope

#### **Protocol Flow**

##### **Phase 0: Reconnaissance & Mental Modeling**

- **Directive**: Non-destructive system scan
- **Output**: Concise digest (≤ 200 lines)
- **Constraint**: No mutations permitted

##### **Phase 1: Planning & Strategy**

- **Objective Restatement**: Clear success criteria
- **Impact Surface**: All affected components identified
- **Strategy Justification**: Technical approach explanation
- **Clarification Threshold**: Only for critical ambiguities

##### **Phase 2: Execution & Implementation**

- **Read-Write-Reread**: Verify every file modification
- **Safety Wrappers**: All commands use timeout protection
- **System-Wide Ownership**: Update all affected consumers
- **Incremental Approach**: Systematic, verifiable changes

##### **Phase 3: Verification & Autonomous Correction**

- **Quality Gates**: Execute all relevant tests and checks
- **Autonomous Fixes**: Self-diagnose and resolve failures
- **End-to-End Testing**: Verify primary workflows
- **Regression Prevention**: Ensure no unintended side effects

##### **Phase 4: Zero-Trust Self-Audit**

- **Fresh Evidence**: Re-verify final state
- **Regression Hunting**: Test related features
- **System Consistency**: Confirm all components working
- **Final Verdict**: Success/failure assessment

#### **Usage Example**

```
User: "Add user authentication to the API"

AI Response:
Acknowledged. Initiating Phase 0: Reconnaissance.

[AI performs systematic investigation]

**Reconnaissance Digest**
- Repository: Node.js/Express API
- Current state: No authentication system
- Dependencies: Express, bcrypt, jsonwebtoken available
- Architecture: RESTful endpoints, middleware pattern

**Execution Plan**
1. Implement user model with password hashing
2. Create authentication middleware
3. Add login/register endpoints
4. Update existing endpoints with auth protection
5. Add comprehensive tests

[AI proceeds with systematic implementation]
```

### **2. Root Cause Analysis Protocol (`refresh.mdc`)**

#### **Purpose**

Deep bug diagnosis when simple fixes have failed. Used for persistent, complex issues requiring systematic investigation.

#### **When to Use**

- Bugs that persist after simple fixes
- Complex system failures
- Performance issues requiring deep analysis
- Intermittent problems
- System-wide issues affecting multiple components

#### **Protocol Characteristics**

- **Deep Investigation**: Exhaustive system analysis
- **Pattern Recognition**: Identify root causes, not symptoms
- **Systematic Testing**: Methodical elimination of possibilities
- **Comprehensive Fixes**: Address underlying issues, not surface problems

#### **Usage Example**

```
User: "The API is randomly failing with 500 errors"

AI Response:
⚠️ Initiating deep bug diagnosis protocol.

**Phase 0: Deep Reconnaissance**
- Analyzing error logs and patterns
- Investigating system dependencies
- Checking resource utilization
- Examining error correlation with system state

**Root Cause Analysis**
- Error pattern: Correlated with high memory usage
- Memory leaks identified in database connection pooling
- Connection cleanup not properly implemented
- Fix: Implement proper connection lifecycle management

[AI implements comprehensive fix]
```

### **3. Retrospective Protocol (`retro.mdc`)**

#### **Purpose**

Metacognitive self-improvement loop. Captures learnings and improves the core doctrine based on session experience.

#### **When to Use**

- End of development sessions
- After completing major features
- When identifying process improvements
- Regular improvement cycles
- After encountering unexpected issues

#### **Protocol Flow**

1. **Session Analysis**: Review completed work and interactions
2. **Learning Extraction**: Identify durable lessons and patterns
3. **Doctrine Assessment**: Evaluate rule effectiveness
4. **Improvement Proposals**: Suggest rule updates or additions
5. **Knowledge Integration**: Incorporate learnings into future sessions

#### **Usage Example**

```
User: "Let's do a retro on this session"

AI Response:
🔄 Initiating retrospective analysis.

**Session Review**
- Task: Implemented user authentication system
- Duration: 2 hours
- Phases completed: All 5 phases successfully
- Quality gates: All tests passing

**Learning Extraction**
- Database connection patterns need standardization
- Authentication middleware could be more reusable
- Test coverage improved development confidence

**Doctrine Assessment**
- Core protocols effective for feature development
- Communication protocols maintained professional tone
- Verification protocols prevented regressions

**Improvement Proposals**
- Add database connection management rule
- Enhance middleware reusability guidelines
- Strengthen test coverage requirements

[AI updates relevant rules]
```

## Protocol Selection Guide

### **Choose `request.mdc` When**

- Starting new development work
- Making planned changes
- Building features or components
- Refactoring existing code
- Implementing improvements

### **Choose `refresh.mdc` When**

- Simple fixes haven't resolved issues
- Problems are complex or persistent
- System behavior is unpredictable
- Performance issues require deep analysis
- Multiple components are affected

### **Choose `retro.mdc` When**

- Completing development sessions
- Identifying process improvements
- Capturing lessons learned
- Updating development protocols
- Maintaining rule effectiveness

## Protocol Combination

### **Stackable Usage**

- **Primary Protocol**: Choose main protocol for task type
- **Optional Directives**: Add specific behavior modifiers
- **Custom Rules**: Incorporate project-specific requirements

### **Example Combinations**

```
Primary: request.mdc (feature development)
+ Directive: concise.mdc (radical conciseness)
+ Custom: project-specific coding standards

Result: Systematic feature development with concise communication
```

## Status Markers

### **Progress Indicators**

- **✅**: Objective completed successfully
- **⚠️**: Recoverable issue encountered and fixed
- **🚧**: Blocked, awaiting input or resource

### **Usage in Reports**

```
**Final Report**
- **Changes Applied:**
  - ✅ `modified`: `/src/auth/userService.js`
  - ✅ `modified`: `/src/auth/authMiddleware.js`
- **Verification Evidence:**
  - ✅ All tests passing
  - ✅ API endpoints responding correctly
- **Final Verdict:**
  - `Self-Audit Complete. System state verified. Mission accomplished.`
```

## Best Practices

### **Protocol Selection**

1. **Assess Task Complexity**: Simple vs. complex requirements
2. **Consider Failure History**: Previous attempts and outcomes
3. **Evaluate System State**: Current stability and health
4. **Match Protocol to Need**: Choose appropriate workflow

### **Execution Quality**

1. **Follow All Phases**: Don't skip verification steps
2. **Maintain Documentation**: Keep chat logs for reference
3. **Use Status Markers**: Clear progress indication
4. **Complete Self-Audit**: Always verify final state

### **Continuous Improvement**

1. **Regular Retros**: End sessions with improvement analysis
2. **Rule Evolution**: Update protocols based on learnings
3. **Pattern Recognition**: Identify effective approaches
4. **Knowledge Sharing**: Document successful strategies

---

_Task protocols are based on the [Autonomous Agent Prompting Framework](https://gist.github.com/aashari/07cc9c1b6c0debbeb4f4d94a3a81339e) by aashari_
