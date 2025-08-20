# Usage Examples

## Overview

This document provides practical examples of how to use Cursor Rules in real development scenarios. Each example demonstrates the complete workflow from rule activation to task completion.

## Example 1: Feature Development

### **Scenario**

Adding user authentication to a Node.js API application.

### **User Request**

```
"Add user authentication to our API with JWT tokens, password hashing, and protected routes"
```

### **AI Response with Rules Applied**

#### **Phase 0: Reconnaissance**

```
Acknowledged. Initiating Phase 0: Reconnaissance.

**Reconnaissance Digest**
- Repository: Node.js/Express API
- Current state: No authentication system
- Dependencies: Express, bcrypt, jsonwebtoken available
- Architecture: RESTful endpoints, middleware pattern
- Database: PostgreSQL with Sequelize ORM
- Testing: Jest framework with supertest
- Quality gates: ESLint, Prettier, test coverage >80%
```

#### **Phase 1: Planning**

```
**Execution Plan**
1. Implement user model with password hashing
2. Create JWT authentication middleware
3. Add login/register endpoints
4. Update existing endpoints with auth protection
5. Add comprehensive tests
6. Update documentation

**Impact Surface**
- New files: `/src/auth/`, `/src/models/User.js`
- Modified: `/src/app.js`, `/src/routes/`
- Tests: `/tests/auth/`, `/tests/integration/`
- Dependencies: bcrypt, jsonwebtoken, express-rate-limit
```

#### **Phase 2: Execution**

```
**Implementing User Model**
✅ Created `/src/models/User.js` with password hashing
✅ Added user validation and error handling
✅ Implemented password comparison methods

**Creating Authentication Middleware**
✅ Created `/src/auth/jwtMiddleware.js`
✅ Added token validation and user extraction
✅ Implemented rate limiting for auth endpoints

**Adding Authentication Endpoints**
✅ Created `/src/routes/auth.js`
✅ Implemented login/register with validation
✅ Added password strength requirements

**Protecting Existing Routes**
✅ Updated `/src/routes/api.js` with auth middleware
✅ Added role-based access control
✅ Maintained backward compatibility
```

#### **Phase 3: Verification**

```
**Running Quality Gates**
✅ ESLint: No errors or warnings
✅ Prettier: Code formatting consistent
✅ Tests: All 15 tests passing (100% coverage)
✅ Security: No vulnerabilities detected

**End-to-End Testing**
✅ Registration endpoint working
✅ Login endpoint returning JWT tokens
✅ Protected routes requiring authentication
✅ Password hashing verified
✅ Rate limiting functional
```

#### **Phase 4: Self-Audit**

```
**Final Report**
- **Changes Applied:**
  - ✅ `created`: `/src/models/User.js`
  - ✅ `created`: `/src/auth/jwtMiddleware.js`
  - ✅ `created`: `/src/routes/auth.js`
  - ✅ `modified`: `/src/routes/api.js`
  - ✅ `created`: `/tests/auth/`
  - ✅ `modified`: `/package.json`

- **Verification Evidence:**
  - ✅ All tests passing (15/15)
  - ✅ ESLint and Prettier clean
  - ✅ API endpoints responding correctly
  - ✅ Authentication flow verified

- **Final Verdict:**
  - `Self-Audit Complete. System state verified and consistent. Mission accomplished.`
```

## Example 2: Bug Diagnosis and Fix

### **Scenario**

API randomly returning 500 errors under load.

### **User Request**

```
"The API is randomly failing with 500 errors when we have more than 100 concurrent users"
```

### **AI Response with Rules Applied**

#### **Deep Investigation Protocol**

```
⚠️ Initiating deep bug diagnosis protocol.

**Phase 0: Deep Reconnaissance**
- Analyzing error logs and patterns
- Investigating system dependencies
- Checking resource utilization
- Examining error correlation with system state

**Error Pattern Analysis**
✅ Error logs show correlation with high memory usage
✅ Database connection pool exhausted
✅ Memory leaks in request handling
✅ No proper error boundaries in middleware
```

#### **Root Cause Identification**

```
**Root Cause Analysis**
- **Primary Issue**: Database connection pool exhaustion
- **Secondary Issue**: Memory leaks in request processing
- **Contributing Factor**: Missing error boundaries
- **Trigger**: Concurrent user load >100

**Technical Details**
- Connection pool size: 10 (too small for load)
- Connection timeout: 30s (too long)
- No connection cleanup on errors
- Memory accumulation in request objects
```

#### **Comprehensive Fix Implementation**

```
**Implementing Fixes**
✅ Increased connection pool size to 50
✅ Added connection timeout to 10s
✅ Implemented proper connection cleanup
✅ Added error boundaries in middleware
✅ Added memory monitoring and alerts
✅ Implemented graceful degradation

**Testing Fixes**
✅ Load testing with 200 concurrent users
✅ Memory usage monitoring
✅ Connection pool health checks
✅ Error rate monitoring
```

#### **Verification and Documentation**

```
**Final Report**
- **Changes Applied:**
  - ✅ `modified`: `/src/database/connection.js`
  - ✅ `modified`: `/src/middleware/errorHandler.js`
  - ✅ `modified`: `/src/app.js`
  - ✅ `created`: `/src/monitoring/`

- **Verification Evidence:**
  - ✅ Load test: 200 users, 0 errors
  - ✅ Memory usage: Stable under load
  - ✅ Connection pool: Healthy utilization
  - ✅ Error rate: <0.1% under normal load

- **Final Verdict:**
  - `Self-Audit Complete. System state verified and consistent. Mission accomplished.`
```

## Example 3: Code Refactoring

### **Scenario**

Refactoring a monolithic service into microservices.

### **User Request**

```
"Refactor our monolithic user service into microservices for better scalability"
```

### **AI Response with Rules Applied**

#### **System Analysis**

```
Acknowledged. Initiating Phase 0: Reconnaissance.

**Reconnaissance Digest**
- Current: Monolithic Node.js service (15K lines)
- Architecture: Single database, shared state
- Dependencies: 45 npm packages
- Testing: 80% coverage, integration tests
- Deployment: Single container, manual deployment
- Monitoring: Basic logging, no metrics
```

#### **Strategic Planning**

```
**Refactoring Strategy**
1. **Service Decomposition**: Identify bounded contexts
2. **Database Separation**: Split data by domain
3. **API Gateway**: Implement service discovery
4. **Event System**: Replace direct calls with events
5. **Independent Deployment**: Containerize each service

**Service Boundaries Identified**
- User Management Service
- Authentication Service
- Profile Service
- Notification Service
- Analytics Service
```

#### **Incremental Implementation**

```
**Phase 1: Service Extraction**
✅ Created User Management Service
✅ Implemented service-to-service communication
✅ Added health checks and monitoring
✅ Maintained backward compatibility

**Phase 2: Database Separation**
✅ Split user data by domain
✅ Implemented data migration scripts
✅ Added data consistency checks
✅ Updated integration tests

**Phase 3: API Gateway**
✅ Implemented service discovery
✅ Added load balancing
✅ Implemented circuit breakers
✅ Added request routing
```

#### **Quality Assurance**

```
**Comprehensive Testing**
✅ Unit tests: All services >90% coverage
✅ Integration tests: Service communication verified
✅ Load tests: Performance maintained
✅ Security tests: No vulnerabilities introduced

**Deployment Verification**
✅ All services deploying independently
✅ Health checks passing
✅ Monitoring dashboards functional
✅ Rollback procedures tested
```

#### **Final Validation**

```
**Final Report**
- **Changes Applied:**
  - ✅ `created`: `/services/user-management/`
  - ✅ `created`: `/services/authentication/`
  - ✅ `created`: `/services/profile/`
  - ✅ `created`: `/services/notification/`
  - ✅ `created`: `/services/analytics/`
  - ✅ `created`: `/gateway/`
  - ✅ `modified`: `/deployment/`

- **Verification Evidence:**
  - ✅ All services operational
  - ✅ Performance: 2x improvement
  - ✅ Deployment time: 80% reduction
  - ✅ Test coverage: 92% overall

- **Final Verdict:**
  - `Self-Audit Complete. System state verified and consistent. Mission accomplished.`
```

## Example 4: Documentation Generation

### **Scenario**

Creating technical architecture documentation.

### **User Request**

```
"Create a technical architecture document for our new microservices system"
```

### **AI Response with Rules Applied**

#### **Document Generation**

```
🔄 Generating technical architecture document using steering rules.

**Technical Architecture Document**
*Author: Lead Architect*
*Date: 2024-01-15*
*Version: 1.0*

**Executive Summary**
Document the microservices architecture for improved scalability and maintainability.

**Current Architecture**
- Monolithic Node.js application
- Single PostgreSQL database
- Manual deployment process
- Limited monitoring and observability

**Technical Requirements**
- Support 10x user growth
- Enable independent service deployment
- Maintain 99.9% uptime
- Support multiple development teams

**Architecture Options Considered**
- Service mesh with Istio
- API gateway with Kong
- Event-driven architecture with Kafka
- Database per service pattern

**Recommended Architecture**
- Service mesh using Istio for communication
- API gateway for external access
- Event-driven communication with Kafka
- Database per service with eventual consistency
- Kubernetes orchestration for deployment

**Implementation Plan**
- Phase 1: Infrastructure and service mesh setup
- Phase 2: Core service extraction
- Phase 3: Advanced features and optimization
- Phase 4: Performance tuning and monitoring

**Risk Mitigation**
- Gradual migration to minimize disruption
- Comprehensive testing and rollback procedures
- Performance monitoring and alerting
- Team training and documentation

**Success Criteria**
- 50% reduction in deployment time
- 99.9% system uptime maintained
- 3x increase in development velocity
- Successful migration of all core services
```

## Example 5: Team Retrospective

### **Scenario**

End-of-sprint retrospective for development team.

### **User Request**

```
"Let's do a retro on this sprint's work"
```

### **AI Response with Rules Applied**

#### **Retrospective Analysis**

```
🔄 Initiating retrospective analysis.

**Sprint Review**
- **Duration**: 2 weeks
- **Team**: 6 developers, 1 PM, 1 QA
- **Objectives**: User authentication system, API improvements
- **Completion**: 85% of planned work

**Work Completed**
✅ User authentication with JWT
✅ API rate limiting and security
✅ Database connection optimization
✅ Comprehensive test coverage
⚠️ Mobile app UI incomplete (carried over)

**Quality Metrics**
- Code coverage: 92% (target: 90%)
- Bug count: 3 (target: <5)
- Deployment success: 100% (target: >95%)
- Code review time: 2.4 hours (target: <4 hours)
```

#### **Learning Extraction**

```
**Key Learnings**
- **Positive**: Test-driven development improved code quality
- **Positive**: Pair programming reduced bugs by 40%
- **Challenge**: Database migrations need better tooling
- **Challenge**: Mobile development underestimated complexity

**Process Improvements Identified**
- Implement automated database migration testing
- Add mobile development expertise to team
- Standardize code review checklists
- Improve sprint planning accuracy
```

#### **Action Planning**

```
**Next Sprint Actions**
- **Database Team**: Research migration testing tools
- **Mobile Team**: Complete UI implementation
- **QA Team**: Implement automated testing pipeline
- **PM**: Refine sprint planning process

**Process Updates**
- Add database migration testing to definition of done
- Include mobile development complexity in story points
- Implement code review templates
- Add sprint retrospective to regular cadence
```

## Best Practices Summary

### **Rule Selection**

1. **Assess Task Type**: Choose appropriate protocol
2. **Consider Complexity**: Simple vs. complex requirements
3. **Evaluate Context**: Current system state and constraints
4. **Match Protocol**: Select workflow that fits the need

### **Execution Quality**

1. **Follow All Phases**: Don't skip verification steps
2. **Use Status Markers**: Clear progress indication
3. **Maintain Documentation**: Keep chat logs for reference
4. **Complete Self-Audit**: Always verify final state

### **Continuous Improvement**

1. **Regular Retros**: End sessions with improvement analysis
2. **Rule Evolution**: Update protocols based on learnings
3. **Pattern Recognition**: Identify effective approaches
4. **Knowledge Sharing**: Document successful strategies

---

**Note**: These examples demonstrate the core rules from the [Autonomous Agent Prompting Framework](https://gist.github.com/aashari/07cc9c1b6c0debbeb4f4d94a3a81339e) by aashari. For detailed information about the rules, see the [Core Rules Documentation](./rules/).
