# Claude Flow Best Practices Guide
## Intention-Based Command Reference
*Your complete "If you want to..." guide*

---

## 🎯 Quick Decision Tree

**Starting a new project?** → Use `hive-mind wizard`  
**Building something complex?** → Use `swarm` with strategy  
**Need specific expertise?** → Use `sparc run <mode>`  
**Working with GitHub?** → Use `github` modes  
**Debugging issues?** → Use `sparc run debug`  
**Optimizing performance?** → Use `analysis` and `optimization`  

---

## 📚 Intention-Based Command Guide

### 🚀 "I want to START a new project"

#### From Scratch
```bash
# Best practice: Use the interactive wizard for guided setup
claude-flow hive-mind wizard

# Alternative: Manual initialization with specific features
claude-flow init --sparc --hive-mind --monitoring
claude-flow config set project.name "MyProject"
claude-flow memory store "project-context" "E-commerce platform with microservices"
```

#### With Existing Code
```bash
# Analyze existing codebase first
claude-flow swarm "Analyze existing codebase structure" --strategy research
claude-flow sparc run architect "Review current architecture"
claude-flow github repo-architect "Optimize repository structure"
```

#### Quick Prototype
```bash
# Rapid prototyping with minimal setup
claude-flow init --minimal
claude-flow sparc run code "Create MVP prototype"
claude-flow swarm "Build proof of concept" --strategy development --max-agents 3
```

---

### 💻 "I want to DEVELOP features"

#### New Feature Development
```bash
# Best practice: Use TDD workflow for robust development
claude-flow sparc tdd "User authentication system"

# Alternative: Multi-agent development
claude-flow swarm "Build user authentication" \
  --strategy development \
  --mode hierarchical \
  --max-agents 6 \
  --parallel

# For complex features: Use pipeline
claude-flow sparc pipeline "Complete payment integration"
```

#### API Development
```bash
# RESTful API
claude-flow swarm "Build REST API for products" --strategy development
claude-flow sparc run code "Implement CRUD endpoints"
claude-flow sparc run api-docs "Generate OpenAPI documentation"

# GraphQL API
claude-flow sparc run architect "Design GraphQL schema"
claude-flow swarm "Implement GraphQL resolvers" --parallel
```

#### Frontend Development
```bash
# React/Vue/Angular components
claude-flow sparc run code "Create responsive dashboard"
claude-flow agent spawn coder --name "frontend-specialist"

# Mobile development
claude-flow sparc run mobile-dev "Build React Native app"
```

#### Backend Services
```bash
# Microservices
claude-flow sparc run architect "Design microservices architecture"
claude-flow swarm "Build authentication microservice" --mode distributed

# Database operations
claude-flow sparc run supabase-admin "Setup database schema"
claude-flow sparc run code "Implement data access layer"
```

---

### 🧪 "I want to TEST my code"

#### Unit Testing
```bash
# Generate comprehensive test suite
claude-flow sparc run tdd "Create unit tests for UserService"

# Multi-agent testing approach
claude-flow swarm "Write comprehensive test coverage" --strategy testing
```

#### Integration Testing
```bash
# Test component integration
claude-flow sparc run integration "Test API endpoints"
claude-flow automation smart-spawn "Integration test suite"
```

#### Performance Testing
```bash
# Benchmark and load testing
claude-flow benchmark run --suite performance
claude-flow analysis bottleneck-detect
claude-flow sparc run code "Create load testing scripts"
```

#### Security Testing
```bash
# Security audit
claude-flow sparc run security-review "Audit authentication system"
claude-flow swarm "Perform security analysis" --strategy analysis
```

---

### 🏗️ "I want to DESIGN architecture"

#### System Architecture
```bash
# Best practice: Use architect mode with visual documentation
claude-flow sparc run architect "Design scalable microservices"
claude-flow sparc run docs-writer "Create architecture diagrams"

# For complex systems: Multi-agent approach
claude-flow hive-mind spawn "Design distributed system" \
  --queen-type strategic \
  --consensus byzantine
```

#### Database Design
```bash
# Schema design
claude-flow sparc run architect "Design database schema"
claude-flow sparc run supabase-admin "Implement database structure"
```

#### API Design
```bash
# API architecture
claude-flow sparc run spec-pseudocode "Define API specifications"
claude-flow sparc run architect "Design RESTful API structure"
claude-flow github workflow-auto "Setup API CI/CD pipeline"
```

---

### 🐛 "I want to DEBUG issues"

#### Bug Investigation
```bash
# Best practice: Systematic debugging
claude-flow sparc run debug "Investigate memory leak"
claude-flow analysis bottleneck-detect
claude-flow monitoring start --focus memory

# Multi-agent debugging
claude-flow swarm "Debug production issue" --strategy analysis --parallel
```

#### Performance Issues
```bash
# Performance debugging
claude-flow optimization analyze
claude-flow analysis performance-report --detailed
claude-flow sparc run refinement-optimization-mode "Optimize slow queries"
```

#### Error Analysis
```bash
# Error pattern analysis
claude-flow hooks post-task --task-id "error-analysis"
claude-flow memory query "error" --namespace logs
claude-flow sparc run debug "Analyze error patterns"
```

---

### 📝 "I want to DOCUMENT my project"

#### Code Documentation
```bash
# Best practice: Automated documentation generation
claude-flow sparc run docs-writer "Generate API documentation"
claude-flow sparc run tutorial "Create developer guide"

# Comprehensive documentation
claude-flow swarm "Create complete documentation" \
  --strategy development \
  --namespace docs
```

#### README and Guides
```bash
# Project documentation
claude-flow sparc run docs-writer "Create comprehensive README"
claude-flow sparc run tutorial "Write getting started guide"
```

#### API Documentation
```bash
# OpenAPI/Swagger
claude-flow sparc run api-docs "Generate OpenAPI spec"
claude-flow github workflow-auto "Setup documentation pipeline"
```

---

### 🚢 "I want to DEPLOY my application"

#### Initial Deployment
```bash
# Best practice: Full deployment pipeline
claude-flow sparc run devops "Setup deployment infrastructure"
claude-flow sparc run integration "Prepare for deployment"
claude-flow github release-manager "Create release v1.0.0"
```

#### CI/CD Setup
```bash
# GitHub Actions
claude-flow github workflow-auto "Setup CI/CD pipeline"
claude-flow sparc run cicd-engineer "Create GitHub Actions workflows"
```

#### Monitoring Setup
```bash
# Post-deployment monitoring
claude-flow sparc run post-deployment-monitoring-mode "Setup monitoring"
claude-flow monitoring start --alerts
claude-flow optimization analyze --export metrics.json
```

---

### 👥 "I want to COLLABORATE with my team"

#### Code Review
```bash
# Automated code review
claude-flow github code-review "Review pull request #123"
claude-flow github pr-manager "Manage pull requests"

# Multi-agent review
claude-flow swarm "Review codebase" --strategy analysis
```

#### Issue Management
```bash
# Issue tracking
claude-flow github issue-tracker "Triage open issues"
claude-flow task create research "Investigate issue #456"
```

#### Team Coordination
```bash
# Project coordination
claude-flow github project-board-sync "Sync project board"
claude-flow hive-mind spawn "Coordinate team tasks" --queen-type tactical
```

---

### 🔄 "I want to REFACTOR code"

#### Code Refactoring
```bash
# Best practice: Systematic refactoring
claude-flow sparc run refinement-optimization-mode "Refactor UserService"
claude-flow sparc run code "Apply SOLID principles"

# Large-scale refactoring
claude-flow swarm "Refactor legacy codebase" \
  --strategy optimization \
  --max-agents 8
```

#### Performance Optimization
```bash
# Optimize performance
claude-flow optimization optimize
claude-flow analysis bottleneck-detect
claude-flow sparc run refinement-optimization-mode "Optimize database queries"
```

#### Code Quality
```bash
# Improve code quality
claude-flow sparc run security-review "Security audit"
claude-flow analysis performance-report
claude-flow hooks post-edit --file "src/main.js" --memory-key "refactor/main"
```

---

### 📊 "I want to ANALYZE my project"

#### Codebase Analysis
```bash
# Best practice: Comprehensive analysis
claude-flow swarm "Analyze codebase quality" --strategy analysis
claude-flow analysis performance-report --detailed
claude-flow github repo-architect "Analyze repository structure"
```

#### Performance Analysis
```bash
# Performance metrics
claude-flow benchmark run --suite performance
claude-flow metrics collect --components all
claude-flow analysis token-usage
```

#### Security Analysis
```bash
# Security audit
claude-flow sparc run security-review "Full security audit"
claude-flow automation workflow-select "security-scanning"
```

---

### 🤖 "I want to AUTOMATE workflows"

#### Task Automation
```bash
# Best practice: Smart automation
claude-flow automation auto-agent "Daily maintenance tasks"
claude-flow automation workflow-select "continuous-integration"
claude-flow hooks pre-task --description "Automated setup"
```

#### Batch Operations
```bash
# Batch processing
claude-flow batch create-config batch-tasks.json
claude-flow batch estimate batch-tasks.json
claude-flow sparc batch "test,deploy,monitor" "Release process"
```

#### Scheduled Tasks
```bash
# Recurring tasks
claude-flow task workflow daily-tasks.json
claude-flow automation smart-spawn "Scheduled maintenance"
```

---

### 🧠 "I want to LEARN and improve"

#### Learning from Operations
```bash
# Best practice: Continuous learning
claude-flow training neural-train
claude-flow training pattern-learn
claude-flow training model-update

# Analyze patterns
claude-flow memory query "success" --namespace patterns
claude-flow analysis performance-report --export learnings.json
```

#### Knowledge Sharing
```bash
# Share knowledge across agents
claude-flow hive-mind memory
claude-flow memory export knowledge-base.json
claude-flow coordination agent-spawn --name "knowledge-coordinator"
```

---

### 🔍 "I want to SEARCH and explore"

#### Code Search
```bash
# Search codebase
claude-flow agent spawn researcher --name "code-explorer"
claude-flow swarm "Find all API endpoints" --strategy research
claude-flow memory query "function" --namespace code
```

#### Documentation Search
```bash
# Search documentation
claude-flow sparc run ask "How does authentication work?"
claude-flow memory query "docs" --recent
```

---

### 💾 "I want to MANAGE state and memory"

#### Session Management
```bash
# Best practice: Regular session saves
claude-flow session save "before-major-change"
claude-flow session list
claude-flow session restore "stable-version"
```

#### Memory Management
```bash
# Store important context
claude-flow memory store "architecture-decisions" "Chose microservices for scalability"
claude-flow memory query "decisions" --namespace project
claude-flow memory export project-memory.json
```

#### Backup and Recovery
```bash
# Backup strategy
claude-flow backup
claude-flow session export full-backup.json
claude-flow memory export memory-backup.json
```

---

## 🎯 Command Combinations for Complex Tasks

### Building a Complete Application
```bash
# 1. Initialize and plan
claude-flow hive-mind wizard
claude-flow sparc run architect "Design application architecture"

# 2. Develop features
claude-flow sparc pipeline "Build core features"
claude-flow swarm "Implement authentication" --strategy development --parallel

# 3. Test thoroughly
claude-flow sparc run tdd "Test all components"
claude-flow sparc run security-review "Security audit"

# 4. Document
claude-flow sparc run docs-writer "Complete documentation"

# 5. Deploy
claude-flow sparc run devops "Setup infrastructure"
claude-flow github release-manager "Deploy v1.0.0"

# 6. Monitor
claude-flow sparc run post-deployment-monitoring-mode "Monitor production"
```

### Debugging Production Issues
```bash
# 1. Gather information
claude-flow swarm "Analyze production logs" --strategy analysis
claude-flow monitoring start --focus errors --alerts

# 2. Reproduce issue
claude-flow sparc run debug "Reproduce production bug"
claude-flow analysis bottleneck-detect

# 3. Fix issue
claude-flow sparc run code "Implement bug fix"
claude-flow sparc run tdd "Add regression tests"

# 4. Deploy fix
claude-flow github pr-manager "Create hotfix PR"
claude-flow sparc run integration "Deploy hotfix"
```

### Optimizing Performance
```bash
# 1. Baseline measurement
claude-flow benchmark run --suite performance
claude-flow analysis performance-report --detailed

# 2. Identify bottlenecks
claude-flow analysis bottleneck-detect
claude-flow optimization analyze

# 3. Implement optimizations
claude-flow sparc run refinement-optimization-mode "Optimize bottlenecks"
claude-flow optimization optimize

# 4. Verify improvements
claude-flow benchmark run --suite performance
claude-flow metrics collect --export after-optimization.json
```

---

## 📋 Quick Reference: Intention → Command

| If you want to... | Use this command |
|------------------|------------------|
| Start a new project | `claude-flow hive-mind wizard` |
| Build a feature | `claude-flow sparc tdd "feature"` |
| Fix a bug | `claude-flow sparc run debug "issue"` |
| Optimize performance | `claude-flow optimization analyze` |
| Review code | `claude-flow github code-review` |
| Deploy application | `claude-flow sparc run devops` |
| Create documentation | `claude-flow sparc run docs-writer` |
| Analyze codebase | `claude-flow swarm "analyze" --strategy analysis` |
| Setup CI/CD | `claude-flow github workflow-auto` |
| Manage tasks | `claude-flow task create` |
| Save progress | `claude-flow session save "checkpoint"` |
| Get help | `claude-flow sparc run ask "question"` |

---

## 🚀 Pro Tips

1. **Always start with `hive-mind wizard`** for new projects - it guides you through optimal setup
2. **Use `--parallel` flag** when working with multiple agents for 2.8-4.4x speed improvement
3. **Save sessions regularly** before major changes using `session save`
4. **Enable monitoring** with `--monitoring` flag for production workflows
5. **Use namespaces** in memory operations to organize data
6. **Leverage SPARC pipeline** for complex multi-step processes
7. **Export metrics** regularly for performance tracking
8. **Use strategy flags** to optimize swarm behavior for specific tasks
9. **Enable auto-scaling** with `--auto-scale` for dynamic workloads
10. **Chain commands** with `&&` for sequential operations

---

## 🎨 Workflow Templates

### Standard Development Workflow
```bash
#!/bin/bash
# development-workflow.sh

# Initialize
claude-flow hive-mind wizard

# Architecture
claude-flow sparc run architect "Design system"

# Development
claude-flow sparc pipeline "Implement features"

# Testing
claude-flow sparc run tdd "Test implementation"

# Documentation
claude-flow sparc run docs-writer "Document code"

# Deployment
claude-flow sparc run integration "Deploy to staging"
```

### Continuous Integration Workflow
```bash
#!/bin/bash
# ci-workflow.sh

# Pre-commit hooks
claude-flow hooks pre-task --description "CI checks"

# Run tests
claude-flow sparc run tdd "Run test suite"

# Security scan
claude-flow sparc run security-review "Security scan"

# Build
claude-flow task create build "Build application"

# Post-build
claude-flow hooks post-task --task-id "build"
```

### Debug Workflow
```bash
#!/bin/bash
# debug-workflow.sh

# Analyze issue
claude-flow swarm "Analyze bug report" --strategy analysis

# Debug
claude-flow sparc run debug "Investigate issue"

# Fix
claude-flow sparc run code "Implement fix"

# Test
claude-flow sparc run tdd "Test fix"

# Deploy
claude-flow github pr-manager "Create fix PR"
```

---

*This guide covers all major use cases and intentions. For specific command details, refer to the Complete Command Reference.*