# Claude Flow Complete Command Reference
## Version: 2.0.0-alpha.88
*Last Updated: 2025-08-09*

---

## 🚀 Quick Reference

### Installation & Setup
```bash
# Install latest alpha version
npm install -g claude-flow@alpha

# First-time setup
npx claude-flow@alpha init                  # Standard initialization
npx claude-flow@alpha hive-mind wizard      # Interactive wizard (RECOMMENDED)

# After installation
claude-flow --version                        # Check version
claude-flow --help                          # Show main help
```

---

## 📚 Complete Command Catalog

### 🎯 Core Commands

#### `init` - Initialize Claude Flow
```bash
claude-flow init [options]

Options:
  --force, -f              # Overwrite existing configuration
  --minimal, -m            # Minimal setup
  --sparc                  # Enable SPARC modes
  --project-name NAME      # Set project name
  --hive-mind             # Enable hive-mind features
  --monitoring            # Enable token usage tracking
  --neural-enhanced       # Enhanced AI features
```

#### `start` - Start Orchestration System
```bash
claude-flow start [options]

Options:
  --ui                    # Enable interactive UI
  --swarm                 # Enable swarm intelligence
  --daemon, -d            # Run as background daemon
  --port PORT             # MCP server port (default: 3000)
  --auto-start           # Auto-start processes
  --health-check         # Enable health monitoring
  --timeout SECONDS      # Startup timeout
  --verbose              # Detailed logging
```

#### `swarm` - Multi-Agent Coordination
```bash
claude-flow swarm "objective" [options]

Options:
  --strategy TYPE         # research, development, analysis, testing, optimization
  --mode TYPE            # centralized, distributed, hierarchical, mesh, hybrid
  --max-agents N         # Maximum agents (default: 8)
  --parallel             # Enable parallel execution
  --monitor              # Real-time monitoring
  --claude               # Use Claude integration
  --namespace NS         # Organization namespace
  --temp                 # Temporary deployment
```

#### `agent` - Agent Management
```bash
claude-flow agent <action> [options]

Actions:
  spawn <type>           # Create new agent
  list                   # List active agents
  info <id>              # Show agent details
  terminate <id>         # Stop agent
  hierarchy              # View agent hierarchy
  network                # View agent network
  ecosystem              # Agent ecosystem view
  provision              # Provision new agents

Agent Types:
  researcher, coder, analyst, optimizer, coordinator
```

#### `status` - System Status
```bash
claude-flow status [options]

Options:
  --json                 # JSON output format
  --detailed             # Detailed information
  --verbose              # Extra verbose output
  --watch                # Live updates
  --interval MS          # Update interval
  --history              # Show history
  --health-check         # Include health metrics
```

---

### 🧠 SPARC Development Modes

#### `sparc` - SPARC Command Suite
```bash
# List all modes
claude-flow sparc modes [--verbose]

# Get mode information
claude-flow sparc info <mode>

# Execute specific mode
claude-flow sparc run <mode> "task description"

# Run TDD workflow
claude-flow sparc tdd "feature description"

# Batch execution
claude-flow sparc batch "mode1,mode2,mode3" "task"

# Full pipeline
claude-flow sparc pipeline "task description"

# Concurrent processing
claude-flow sparc concurrent <mode> "tasks-file.txt"
```

#### Available SPARC Modes (17 total)
```bash
# Architecture & Design
claude-flow sparc run architect "design system architecture"
claude-flow sparc run spec-pseudocode "analyze requirements"

# Development
claude-flow sparc run code "implement feature"
claude-flow sparc run tdd "test-driven development"
claude-flow sparc run debug "troubleshoot issues"

# Quality & Security
claude-flow sparc run security-review "audit code"
claude-flow sparc run refinement-optimization-mode "optimize performance"

# Documentation
claude-flow sparc run docs-writer "generate documentation"
claude-flow sparc run tutorial "create learning materials"

# Integration & Deployment
claude-flow sparc run integration "integrate components"
claude-flow sparc run post-deployment-monitoring-mode "monitor deployment"
claude-flow sparc run devops "infrastructure setup"

# Specialized
claude-flow sparc run supabase-admin "database management"
claude-flow sparc run mcp "tool integration"
claude-flow sparc run ask "expert consultation"
claude-flow sparc run sparc "orchestrate SPARC workflow"
```

---

### 🐝 Hive Mind System

#### `hive-mind` - Collective Intelligence
```bash
# Main commands
claude-flow hive-mind init                    # Initialize system
claude-flow hive-mind wizard                  # Interactive setup (RECOMMENDED)
claude-flow hive-mind spawn "objective"       # Create swarm
claude-flow hive-mind status                  # View status
claude-flow hive-mind metrics                 # Performance metrics

# Session management
claude-flow hive-mind sessions                # List all sessions
claude-flow hive-mind resume <session-id>     # Resume session
claude-flow hive-mind stop <session-id>       # Stop session

# Advanced features
claude-flow hive-mind consensus               # View consensus decisions
claude-flow hive-mind memory                  # Manage collective memory

Options:
  --queen-type TYPE      # strategic, tactical, adaptive
  --max-workers N        # Maximum workers (default: 8)
  --consensus TYPE       # majority, weighted, byzantine
  --memory-size MB       # Collective memory (default: 100)
  --auto-scale          # Enable auto-scaling
  --encryption          # Encrypted communication
  --monitor             # Real-time dashboard
  --claude              # Claude Code integration
  --auto-spawn          # Auto-spawn instances
  --execute             # Execute immediately
  --verbose             # Detailed logging
```

---

### 🐙 GitHub Integration

#### `github` - GitHub Workflow Automation
```bash
claude-flow github <mode> "objective" [options]

Modes:
  init                   # Initialize GitHub-enhanced checkpoints
  gh-coordinator         # Workflow orchestration
  pr-manager            # Pull request management
  issue-tracker         # Issue management
  release-manager       # Release coordination
  repo-architect        # Repository optimization
  sync-coordinator      # Multi-repo synchronization
  workflow-auto         # Automation setup
  code-review           # Automated reviews
```

---

### 💾 Memory Management

#### `memory` - Persistent Memory Operations
```bash
claude-flow memory <action> [args] [options]

Actions:
  store "key" "value"    # Store data
  query "pattern"        # Search memory
  list                   # List namespaces
  export <file>          # Export to file
  import <file>          # Import from file
  clear [namespace]      # Clear namespace
  stats                  # Memory statistics
  cleanup                # Clean old data

Options:
  --namespace NS         # Memory namespace
  --recent              # Recent entries only
  --ttl SECONDS         # Time to live
```

---

### 🤖 Intelligence Commands

#### `training` - Neural Pattern Learning
```bash
claude-flow training <command> [options]

Commands:
  neural-train           # Train neural patterns
  pattern-learn          # Learn from outcomes
  model-update          # Update agent models
```

#### `coordination` - Swarm Orchestration
```bash
claude-flow coordination <command> [options]

Commands:
  swarm-init            # Initialize swarm infrastructure
  agent-spawn           # Spawn coordinated agents
  task-orchestrate      # Orchestrate task execution
```

#### `analysis` - Performance Analytics
```bash
claude-flow analysis <command> [options]

Commands:
  bottleneck-detect     # Detect bottlenecks
  performance-report    # Generate reports
  token-usage           # Analyze token consumption
```

#### `automation` - Workflow Management
```bash
claude-flow automation <command> [options]

Commands:
  auto-agent            # Auto-spawn optimal agents
  smart-spawn           # Intelligent agent spawning
  workflow-select       # Select optimal workflows
```

#### `hooks` - Lifecycle Events
```bash
claude-flow hooks <command> [options]

Commands:
  pre-task              # Before task execution
  post-task             # After task completion
  pre-edit              # Before file modification
  post-edit             # After file modification
  session-start         # Session initialization
  session-end           # Session cleanup
  session-restore       # Restore session state
  notify                # Send notifications

Options:
  --description DESC    # Task description
  --task-id ID         # Task identifier
  --file PATH          # File path
  --memory-key KEY     # Memory storage key
  --session-id ID      # Session identifier
  --export-metrics     # Export metrics
  --message MSG        # Notification message
```

---

### 📊 Monitoring & Optimization

#### `monitoring` - Real-Time Monitoring
```bash
claude-flow monitoring <command> [options]

Commands:
  start                 # Start monitoring
  status                # Monitor status
  metrics               # View metrics
```

#### `optimization` - Performance Optimization
```bash
claude-flow optimization <command> [options]

Commands:
  analyze               # Analyze performance
  optimize              # Apply optimizations
  report                # Generate report
```

---

### 🔧 Configuration & Utilities

#### `config` - System Configuration
```bash
claude-flow config <action> [key] [value]

Actions:
  get <key>             # Get configuration value
  set <key> <value>     # Set configuration value
  list                  # List all settings
  reset [key]           # Reset to defaults
  validate              # Validate configuration
  init                  # Initialize config
```

#### `task` - Task Management
```bash
claude-flow task <action> [options]

Actions:
  create <type> "desc"  # Create task
  list                  # List tasks
  status [id]           # Task status
  cancel <id>           # Cancel task
  workflow <file>       # Run workflow
```

#### `mcp` - MCP Server Management
```bash
claude-flow mcp <action> [options]

Actions:
  start                 # Start MCP server
  status                # Server status
  tools                 # List available tools
  stop                  # Stop server
  auth setup            # Setup authentication

Options:
  --port PORT           # Server port
  --transport TYPE      # Transport type
  --verbose             # Detailed output
```

#### `batch` - Batch Operations
```bash
claude-flow batch <action> [options]

Actions:
  create-config <file>  # Create batch config
  validate-config <file># Validate config
  estimate <file>       # Estimate resources
  list-templates        # List templates
  list-environments     # List environments

Options:
  --interactive         # Interactive mode
```

#### `stream-chain` - Stream Processing
```bash
claude-flow stream-chain <workflow> [options]

# Multi-agent pipeline processing with stream-JSON
```

---

### 🛠️ Utility Commands

#### Session Management
```bash
claude-flow session list                      # List sessions
claude-flow session save "name"               # Save session
claude-flow session restore "name"            # Restore session
claude-flow session delete "name"             # Delete session
claude-flow session export <file>             # Export session
claude-flow session import <file>             # Import session
claude-flow session info [name]               # Session info
claude-flow session clean                     # Clean old sessions
```

#### System Utilities
```bash
claude-flow diagnostics                       # System diagnostics
claude-flow health-check                      # Health check
claude-flow benchmark run [suite]             # Run benchmarks
claude-flow metrics collect                   # Collect metrics
claude-flow cleanup                          # Clean temporary files
claude-flow backup                           # Create backup
claude-flow restore <backup>                 # Restore from backup
```

#### Development Tools
```bash
claude-flow repl                             # Interactive REPL
claude-flow completion                       # Shell completion
claude-flow node-repl                        # Node.js REPL
```

---

### 🎛️ Environment Variables

#### Core Configuration
```bash
CLAUDE_FLOW_DISABLE_PRE_TASK=true           # Disable pre-task hooks
CLAUDE_FLOW_DISABLE_POST_EDIT=true          # Disable post-edit hooks
CLAUDE_FLOW_HOOK_TIMEOUT=30000              # Hook timeout (ms)
CLAUDE_FLOW_MEMORY_PATH=./custom-memory     # Custom memory path
CLAUDE_FLOW_METRIC_FORMAT=json              # Metric format
```

#### Runtime Environment
```bash
CLAUDE_WORKING_DIR=/workspace               # Working directory
CLAUDE_FLOW_PATH=/custom/path               # Executable path
MCP_ENABLED=true                           # Enable MCP
NODE_ENV=production                        # Environment mode
```

#### Feature Toggles
```bash
CLAUDE_FLOW_EXPERIMENTAL=true              # Experimental features
CLAUDE_FLOW_DEBUG=true                     # Debug mode
CLAUDE_FLOW_PERFORMANCE_TRACKING=true      # Performance tracking
```

---

### 🔗 Command Aliases & Shortcuts

#### Built-in Aliases
```bash
cf = claude-flow                           # Main alias
hive = claude-flow hive-mind              # Hive-mind shortcut
sw = claude-flow swarm                    # Swarm shortcut
```

#### NPM Scripts
```bash
npm run dev                                # Development mode
npm run build                              # Build project
npm run test                               # Run tests
npm run diagnostics                        # System diagnostics
npm run health-check                       # Health check
```

---

### 🚨 Hidden/Advanced Commands

#### Background Operations
```bash
claude-flow-swarm-background "task"        # Background swarm
claude-flow-swarm-bg "task"               # Background alias
claude-flow-swarm-monitor                 # Direct monitoring
```

#### Internal Commands
```bash
claude-flow orchestrate "task"            # Internal orchestrator
claude-flow coordinate "multi-step"       # Task coordination
claude-flow automation setup              # Workflow automation
claude-flow automation execute            # Execute automation
```

#### Alternative Entry Points
```bash
./bin/claude-flow                         # Direct binary
./bin/claude-flow-dev                     # Development mode
./bin/claude-flow-swarm                   # Swarm-specific
./bin/claude-flow-swarm-ui                # UI-enabled swarm
./claude-flow                             # Universal wrapper
```

---

### 📝 Command Patterns & Examples

#### Complex Task Orchestration
```bash
# Multi-agent development pipeline
claude-flow swarm "Build microservices API" \
  --strategy development \
  --mode hierarchical \
  --max-agents 10 \
  --parallel \
  --monitor

# SPARC batch processing
claude-flow sparc batch "architect,code,tdd,integration" \
  "Create authentication system"

# Hive-mind with Claude integration
claude-flow hive-mind spawn "Research AI trends" \
  --claude \
  --auto-spawn \
  --queen-type strategic \
  --consensus byzantine
```

#### Background Processing
```bash
# Start background swarm
claude-flow swarm "Long analysis task" --daemon &

# Monitor progress
claude-flow monitor --focus swarm --alerts

# Export metrics
claude-flow metrics collect --export metrics.json
```

#### Session Workflows
```bash
# Save current state
claude-flow session save "project-v1"

# Run complex workflow
claude-flow sparc pipeline "Complete feature implementation"

# Restore if needed
claude-flow session restore "project-v1"
```

---

### 🎯 Best Practices

1. **Always use `hive-mind wizard` for first-time setup**
2. **Enable monitoring for production workflows**
3. **Use parallel execution for multi-agent tasks**
4. **Leverage session management for complex projects**
5. **Configure hooks for automated workflows**
6. **Use namespaces for organized memory storage**
7. **Enable health checks for long-running processes**
8. **Export metrics regularly for analysis**

---

### 📚 Additional Resources

- **Documentation**: https://github.com/ruvnet/claude-flow
- **Hive Mind Guide**: https://github.com/ruvnet/claude-flow/tree/main/docs/hive-mind
- **ruv-swarm**: https://github.com/ruvnet/ruv-FANN/tree/main/ruv-swarm
- **Discord Community**: https://discord.agentics.org

---

*This document represents the complete command reference for Claude Flow v2.0.0-alpha.88. All commands have been verified against the actual codebase and tested for accuracy.*