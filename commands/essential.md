# Essential Commands Reference

## Core 10 Commands Every User Should Know

### 🚀 Lifecycle Commands

#### `/start`
**Purpose**: Initialize framework and explain collaboration model
**Usage**: `/start`
**Example**:
```
User: /start
Claude: Welcome! I'm operating under the Technical AI Collaboration Framework v2.2.5.
        Here's how we'll work together...
```

#### `/done`
**Purpose**: Mark current task or project phase as complete
**Usage**: `/done`
**Example**:
```
User: /done
Claude: ✅ Task 'Implement Redis cache' marked complete.
        💡 Use `/next` to see your next priority.
```

#### `/help` or `/?`
**Purpose**: Show available commands with examples
**Usage**: `/help` or `/?` or `/help [command]`
**Example**:
```
User: /?
Claude: Available Commands:
        ━━━━━━━━━━━━━━━━━
        /pause     - Stop and wait for direction
        /risks     - Analyze potential risks
        ...
```

### 🎮 Control Commands

#### `/pause`
**Purpose**: Emergency brake to stop rushing
**Usage**: `/pause`
**Shortcut**: `/p`
**Example**:
```
User: /pause
Claude: ⏸️ PAUSED
        
        Current State:
        - Working on: Database migration script
        - Progress: 40% complete
        - Next planned: Error handling implementation
        
        What would you like to adjust?
```

#### `/mode`
**Purpose**: Switch operating mode
**Usage**: `/mode [task|project|research|minimal]`
**Examples**:
- `/mode task` - Quick, focused execution
- `/mode project` - Full governance and documentation
- `/mode research` - Deep investigation with multiple sources
- `/mode minimal` - Bare-bones, no framework overhead

#### `/emergency`
**Purpose**: Bypass all framework rules for immediate help
**Usage**: `/emergency`
**When to use**: Framework is being unhelpful or blocking critical work
**Example**:
```
User: /emergency
Claude: Framework bypassed. How can I help directly?
```

### 👁️ View Commands

#### `/status`
**Purpose**: Display current state, mode, and context
**Usage**: `/status`
**Shortcut**: `/s`
**Example**:
```
User: /status
Claude: 📊 Current Status:
        - Mode: PROJECT
        - Phase: 2 of 4 (Implementation)
        - Active Task: Redis integration
        - Risks Identified: 3 (1 High, 2 Medium)
        - Session Duration: 47 minutes
        - Energy Level: Optimal
```

#### `/risks`
**Purpose**: Run comprehensive risk assessment
**Usage**: `/risks` or `/risks list`
**Example**:
```
User: /risks
Claude: 🔍 Comprehensive Risk Assessment:
        
        HIGH RISKS:
        1. Data Loss During Migration
           - Probability: 4/5
           - Impact: 5/5
           - Score: 20
           - Mitigation: Implement rollback mechanism
        
        MEDIUM RISKS:
        ...
```

### 💾 State Commands

#### `/save`
**Purpose**: Create named checkpoint
**Usage**: `/save [name]`
**Example**:
```
User: /save before-refactor
Claude: 💾 Checkpoint 'before-refactor' saved.
        Includes: Current context, decisions made, code state.
        💡 Use `/load before-refactor` to restore if needed.
```

#### `/undo`
**Purpose**: Revert last significant action
**Usage**: `/undo`
**Example**:
```
User: /undo
Claude: ↩️ Reverting last action: 'Generated authentication module'
        State restored to: Pre-generation checkpoint
        💡 Your previous work is saved in '/tmp/undo-buffer' if needed.
```

## Command Shortcuts

| Full Command | Shortcut | Purpose |
|--------------|----------|---------||
| `/pause`     | `/p`     | Quick emergency stop |
| `/status`    | `/s`     | Quick status check |
| `/help`      | `/?`     | Quick help access |
| `/risks`     | `/r`     | Quick risk check |

## Smart Command Features

### Autocomplete
Type partial commands for suggestions:
- `/h` → suggests `/help`
- `/pa` → suggests `/pause`
- `/st` → suggests `/start` or `/status`

### Context-Aware Suggestions
Claude will suggest relevant commands:
- After errors → 💡 "Consider `/undo` to revert"
- During long sessions → 💡 "Perhaps `/energy` check?"
- After completion → 💡 "Use `/done` then `/next`"

### Progressive Revelation
- New users: See only essential commands
- After 5+ uses: Advanced commands revealed
- Power users: Full command set available

## Getting Started

1. Always begin with `/start` for new sessions
2. Use `/status` to orient yourself
3. Apply `/pause` liberally when needed
4. End with `/done` for clean closure

---

💡 **Pro Tip**: Type `/` alone to see available commands at any time!