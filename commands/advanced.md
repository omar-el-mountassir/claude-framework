# Advanced Commands Reference

## Power User Commands

### 🔧 Workflow Commands

#### `/next`
**Purpose**: Surface next priority based on context
**Usage**: `/next`
**Example**:
```
User: /next
Claude: 📋 Next Priority Analysis:
        
        Based on:
        - Current progress: Auth module complete
        - Dependencies: Database layer required
        - Risk factors: Performance bottleneck identified
        
        🎯 Recommendation: Implement database connection pooling
        ↳ Why: Addresses performance risk, unblocks 3 features
        
        💡 Use `/init database-pooling` to start with governance
```

#### `/branch`
**Purpose**: Create alternate approach for exploration
**Usage**: `/branch [name]`
**Example**:
```
User: /branch redis-alternative
Claude: 🌿 Created branch: 'redis-alternative'
        Current branches:
        - main (current)
        - redis-alternative (new)
        
        You can now explore alternatives without losing main approach.
        💡 Use `/compare main redis-alternative` when ready.
```

#### `/init`
**Purpose**: Initialize new project with full governance
**Usage**: `/init [project-name]`
**Example**:
```
User: /init payment-system-redesign
Claude: 🚀 Initializing PROJECT: Payment System Redesign
        
        Creating:
        ✅ Project Charter
        ✅ Risk Register (0 risks)
        ✅ Decision Log (empty)
        ✅ Phase Gates (4 defined)
        
        Current Phase: 1 of 4 (Discovery)
        
        First question: What's driving this redesign?
```

### 🔍 Analysis Commands

#### `/depth`
**Purpose**: Control analysis thoroughness
**Usage**: `/depth [1-5]`
**Levels**:
- 1: Quick overview
- 2: Standard analysis
- 3: Detailed investigation (default)
- 4: Comprehensive research
- 5: Exhaustive deep-dive

**Example**:
```
User: /depth 5
Claude: 🔬 Analysis depth set to: 5 (Exhaustive)
        I'll now:
        - Examine all edge cases
        - Research historical patterns
        - Analyze multiple alternatives
        - Provide detailed comparisons
        💡 This may take longer but ensures thoroughness.
```

#### `/perspectives`
**Purpose**: Multi-viewpoint analysis of decisions
**Usage**: `/perspectives [domain1, domain2, ...]`
**Common domains**: security, performance, cost, ux, scalability, maintainability
**Example**:
```
User: /perspectives security, performance, cost
Claude: 🔄 Analyzing from multiple perspectives:
        
        🔒 SECURITY PERSPECTIVE:
        - Vulnerability: SQL injection risk in current design
        - Recommendation: Use parameterized queries
        - Impact: Critical for compliance
        
        ⚡ PERFORMANCE PERSPECTIVE:
        - Bottleneck: N+1 query pattern detected
        - Recommendation: Implement eager loading
        - Impact: 3x faster page loads
        
        💰 COST PERSPECTIVE:
        - Current: $200/month database costs
        - With optimization: $50/month
        - ROI: Changes pay for themselves in 2 months
```

#### `/explain`
**Purpose**: Understand framework's reasoning
**Usage**: `/explain` or `/explain [behavior]`
**Example**:
```
User: /explain why are you asking about testing?
Claude: 🤔 Framework Reasoning:
        
        Trigger: You mentioned "deploy to production"
        Rule: Production deployments require test coverage check
        Purpose: Prevent untested code reaching users
        
        This is from Risk Management Protocol, Score: 16 (High)
        
        💡 Use `/bypass testing-check` if you need to skip this.
```

### 📋 Management Commands

#### `/tasks`
**Purpose**: View active work items and priorities
**Usage**: `/tasks`
**Example**:
```
User: /tasks
Claude: 📋 Active Tasks:
        
        🔴 HIGH PRIORITY:
        1. Fix authentication bug (Due: Today)
        2. Complete security audit (Due: Tomorrow)
        
        🟡 MEDIUM PRIORITY:
        3. Optimize database queries (Due: This week)
        4. Update documentation (Due: This week)
        
        🟢 LOW PRIORITY:
        5. Refactor legacy code (Due: Next sprint)
        
        💡 Use `/next` for recommended priority.
```

#### `/decisions`
**Purpose**: Review decision history
**Usage**: `/decisions` or `/decisions [topic]`
**Example**:
```
User: /decisions database
Claude: 📚 Decision Log (filtered: database):
        
        2024-01-13 14:30
        Decision: Choose PostgreSQL over MySQL
        Rationale: JSON support, better concurrent writes
        Impact: Requires team training
        Status: Implemented ✅
        
        2024-01-13 15:45
        Decision: Implement connection pooling
        Rationale: Prevent connection exhaustion
        Impact: Adds complexity, improves performance
        Status: In Progress 🔄
```

#### `/memory`
**Purpose**: Create or update Project Memory Card
**Usage**: `/memory` or `/memory update`
**Example**:
```
User: /memory
Claude: 🧠 Creating Project Memory Card...
        
        [Generates comprehensive artifact with:
         - Current context
         - Decision history
         - Risk register
         - Progress tracking
         - Next session notes]
         
        💡 Save this artifact to resume in next session.
```

### 🔄 Framework Evolution Commands

#### `/propose`
**Purpose**: Suggest framework improvement
**Usage**: `/propose [enhancement-description]`
**Example**:
```
User: /propose add auto-save every 10 minutes
Claude: 📝 Creating Enhancement Proposal:
        
        Title: Add auto-save functionality
        Problem: Work lost during long sessions without saves
        Solution: Automatic checkpoint every 10 minutes
        Impact: Minimal overhead, high safety value
        
        Creating PR: github.com/omar-el-mountassir/human-ai/pull/1
        
        🎯 Review and merge to activate this enhancement.
```

#### `/patterns`
**Purpose**: Show detected usage patterns
**Usage**: `/patterns`
**Example**:
```
User: /patterns
Claude: 📊 Usage Pattern Analysis:
        
        FREQUENT SEQUENCES:
        1. `/start` → `/status` → `/risks` (80% of sessions)
        2. `/pause` after error messages (65% correlation)
        3. `/undo` → `/branch` (exploring alternatives)
        
        FRICTION POINTS:
        - 5 instances of "slow down" despite anti-rush protocol
        - 3 times asked for state before `/status` existed
        
        💡 Consider `/propose stronger-anti-rush` based on patterns.
```

#### `/version`
**Purpose**: Framework version information
**Usage**: `/version`
**Example**:
```
User: /version
Claude: 📌 Framework Version: 2.2.5
        
        Recent Changes:
        - v2.2.5: Added intelligent command suggestions
        - v2.2.4: Implemented command system
        - v2.2.3: Added prioritized decisions
        
        Repository: github.com/omar-el-mountassir/human-ai
        Last Updated: 2024-01-13
        
        💡 Use `/propose` to suggest improvements.
```

### 🚨 Emergency Commands

#### `/bypass`
**Purpose**: Temporarily disable specific framework rules
**Usage**: `/bypass [rule]`
**Rules**: anti-rush, risk-check, energy-monitor, decision-gates
**Example**:
```
User: /bypass risk-check
Claude: ⚠️ Risk checking DISABLED for this session.
        
        Framework will not:
        - Auto-detect risks
        - Force risk assessments
        - Block on high risk scores
        
        ⏰ Re-enables on next `/start`
        💡 Use `/risks` manually when needed.
```

#### `/reset`
**Purpose**: Return to baseline framework state
**Usage**: `/reset`
**Example**:
```
User: /reset
Claude: 🔄 Framework Reset Complete:
        
        Cleared:
        - ❌ All temporary modifications
        - ❌ Active bypasses
        - ❌ Custom configurations
        
        Restored:
        - ✅ Default framework v2.2.5
        - ✅ Standard protocols
        - ✅ All safety measures
        
        💡 Use `/status` to verify clean state.
```

#### `/minimal`
**Purpose**: Bare-bones mode without framework overhead
**Usage**: `/minimal`
**Example**:
```
User: /minimal
Claude: Entering minimal mode. I'll help directly without framework protocols.
        No risk checks, no decision gates, no energy monitoring.
        Just direct assistance.
        
        Use `/mode normal` to restore framework.
```

## Advanced Workflows

### Multi-Branch Development
```
/branch approach-a
[work on approach A]
/save checkpoint-a

/branch approach-b  
[work on approach B]
/save checkpoint-b

/compare approach-a approach-b
[see detailed comparison]

/merge approach-b
[integrate best parts]
```

### Deep Research Flow
```
/mode research
/depth 5
/perspectives security, scalability, cost
[comprehensive analysis follows]
/memory
[save research artifact]
```

### Rapid Prototyping
```
/mode minimal
/bypass risk-check
[fast implementation]
/mode normal
/risks
[retroactive risk assessment]
```

## Pro Tips

1. **Chain Commands**: Some commands work well together
   - `/init` → `/risks` → `/branch`
   - `/done` → `/next` → `/init`

2. **Use Branches Liberally**: Explore without commitment
   - Main approach stays safe
   - Compare before deciding
   - Merge best elements

3. **Depth Control**: Match analysis to need
   - Exploration: depth 1-2
   - Planning: depth 3
   - Critical decisions: depth 4-5

4. **Framework Evolution**: You own the framework
   - Notice friction? `/propose` improvement
   - See patterns? They become features
   - Version control ensures safety

---

🚀 **Remember**: Advanced commands unlock when you need them, not before!