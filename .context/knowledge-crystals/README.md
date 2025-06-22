# 💎 Knowledge Crystals Directory

Knowledge Crystals are compressed summaries of your learning progress, created when context windows approach their limit.

## 🔮 What Are Knowledge Crystals?

When a chat session gets too long, the AI creates a "crystal" - a highly compressed summary that captures:
- Your essential progress state
- Key concepts you've learned
- Current challenges and context
- Everything needed to continue seamlessly

## 📝 Crystal File Format

Files are named: `KC-YYYY-MM-DD-HHMM-[CODENAME].yaml`

Example: `KC-2024-01-20-1630-DragonCoder.yaml`

## 💡 When Crystals Are Created

- Automatically when context usage reaches 80%
- When starting a new chat from a full session
- On request with `/create-crystal`

## 🔄 Using Knowledge Crystals

### To Continue from a Crystal:
```
Start new chat with:
/load-crystal KC-2024-01-20-1630-DragonCoder
```

### Crystal Structure Example:
```yaml
KNOWLEDGE_CRYSTAL_001:
  student_state:
    codename: DragonCoder
    level: 5
    xp: 450/500
    skills: [80, 60, 40, 20]
  
  concepts_mastered:
    - Boolean logic
    - Basic conditionals
    - Simple loops
    - Function basics
    
  active_context:
    working_on: "Function Forest Quest"
    last_code: "def calculate_average(numbers)..."
    stuck_on: "Understanding recursion"
    next_step: "Explain recursion with visual metaphor"
    
  learning_profile:
    style: "Visual learner"
    strengths: ["debugging", "pattern recognition"]
    needs_work: ["abstract thinking", "algorithm design"]
```

## 🚀 Crystal Commands

- `/create-crystal` - Generate crystal from current state
- `/load-crystal [ID]` - Load and continue from crystal
- `/merge-crystals` - Combine multiple crystals (advanced)

## 📊 Crystal vs Checkpoint

| Feature | Checkpoint | Knowledge Crystal |
|---------|------------|-------------------|
| Size | Large (full state) | Small (compressed) |
| Detail | Everything | Essential only |
| Use Case | Normal continuation | Context limit recovery |
| Format | Markdown | YAML |

## ⚡ Best Practices

1. **Don't Delete Crystals** - They're your recovery lifeline
2. **Reference in New Chats** - Always mention crystal ID when continuing
3. **One Crystal Per Session** - Avoid confusion with multiple crystals

---
*Knowledge Crystals ensure you never lose progress, even across multiple chat sessions!*