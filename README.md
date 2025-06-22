# 🎮 CodeQuest: AI-Powered Programming Learning System

Welcome to your personalized programming education system! This project uses Cursor's AI with persistent context management to create a gamified learning experience.

## 🚀 Quick Start

### First Time Setup
1. Open this project in Cursor
2. Start a new chat and say:
   ```
   Initialize me as a new CodeQuest student
   ```

### Continuing Your Journey
Start any new chat with:
```
Continue my CodeQuest session from the latest checkpoint
```

## 📁 Project Structure

```
relearn-programming-as-you-should/
├── .cursor/
│   └── rules/                    # AI behavior rules (auto-loaded)
│       ├── codequest-system.mdc  # Main system rules
│       ├── session-state.mdc     # Progress tracking rules
│       └── context-persistence.mdc # Save/load rules
│
├── .context/                     # Your progress data
│   ├── current-session.md        # Active session state
│   ├── checkpoints/              # Full progress saves
│   └── knowledge-crystals/       # Compressed summaries
│
├── quests/                       # Learning challenges
│   ├── logic_foundations/        # Beginner concepts
│   ├── programming_basics/       # Core programming
│   └── real_projects/            # Advanced projects
│
└── achievements/                 # Your earned badges
```

## 🎯 How It Works

1. **Gamified Learning**: Earn XP, level up, unlock achievements
2. **Persistent Progress**: Never lose your place between chats
3. **Guided Discovery**: Learn by understanding, not copying
4. **Smart Context**: AI remembers everything about your journey

## 💡 Essential Commands

### During Learning
- `/checkpoint` - Save your progress now
- `/status` - See your current level and XP
- `/hint` - Use a hint token (if available)
- `/achievements` - View all achievements

### Session Management
- `/load-checkpoint [ID]` - Load specific save
- `/create-crystal` - Create compressed backup
- `/session-info` - Current session details

## 🎮 Understanding the System

### XP System
- **Logic Understanding**: 10-20 XP
- **Problem Solving**: 15-30 XP
- **Bug Fixing**: 20-40 XP
- **Code Refactoring**: 30-60 XP

### Levels
- Every 100 XP initially (scales up later)
- New abilities unlock with each level
- Special rewards at milestone levels (5, 10, 15...)

### Power-ups
- **Hint Tokens**: Get subtle guidance
- **Debug Vision**: See potential issues
- **Mentor Wisdom**: Deep explanations
- **Pattern Radar**: Find similar solutions

## 🚨 When You Hit Context Limits

If the AI seems to forget things or mentions "context limits":

1. Immediately say:
   ```
   Create a knowledge crystal and checkpoint for continuation
   ```

2. Start a new chat with:
   ```
   Load my CodeQuest progress from crystal: [PROVIDED_ID]
   ```

## 📝 Best Practices

1. **Regular Saves**: Let the system auto-save every 5 challenges
2. **One Topic Per Session**: Start fresh chats for new topics
3. **Read the Feedback**: The AI explains WHY, not just HOW
4. **No Copy-Paste**: Type code yourself for better learning
5. **Ask Questions**: The AI is your pair programming partner

## 🎯 Your First Quest

Ready to begin? Start Cursor and say:
```
I'm ready to begin CodeQuest! Initialize my profile and let's start with the Logic Labyrinth quest line.
```

## 🆘 Troubleshooting

### "AI doesn't remember me"
- Check if `.context/current-session.md` exists
- Use `/load-checkpoint latest`

### "Context limit reached"
- Create a crystal immediately
- Start new chat with crystal ID

### "Lost my progress"
- Check `.context/checkpoints/` directory
- Load the most recent checkpoint file

## 🌟 Pro Tips

1. **Git Commit Progress**: Track your learning journey
2. **Review Checkpoints**: See how far you've come
3. **Challenge Yourself**: Try solving without hints first
4. **Take Notes**: Add comments to your code for later

---

## 🚀 Let's Start Learning!

Remember: The goal isn't to get AI to write code for you - it's to understand programming deeply enough that you won't need AI assistance. CodeQuest makes this journey fun and trackable!

**Happy Learning!** 🎮👨‍💻👩‍💻