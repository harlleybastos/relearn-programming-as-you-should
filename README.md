# 🎮 CodeQuest: AI-Powered Programming Learning System

Welcome to your personalized programming education system! This project uses GitHub Copilot's custom instructions with persistent context management to create a gamified learning experience inside VS Code.

## 🚀 Quick Start

### First Time Setup
1. Open this project in **VS Code** with **GitHub Copilot** installed
2. Open Copilot Chat and say:
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
├── .github/
│   ├── copilot-instructions.md       # Repository-wide custom instructions (auto-loaded by Copilot)
│   └── instructions/                  # Path-specific custom instructions
│       └── code-files.instructions.md # Rules for code file interactions
│
├── .context/                          # Your progress data
│   ├── current-session.md             # Active session state
│   ├── checkpoints/                   # Full progress saves
│   └── knowledge-crystals/            # Compressed summaries
│
├── quests/                            # Learning challenges
│   ├── logic_foundations/             # Beginner concepts
│   ├── programming_basics/            # Core programming
│   └── real_projects/                 # Advanced projects
│
└── achievements/                      # Your earned badges
```

## 🎯 How It Works

1. **Gamified Learning**: Earn XP, level up, unlock achievements
2. **Persistent Progress**: Never lose your place between chats
3. **Guided Discovery**: Learn by understanding, not copying
4. **Smart Context**: AI remembers everything about your journey via `.context/` files

### How GitHub Copilot Custom Instructions Work

GitHub Copilot automatically reads the `.github/copilot-instructions.md` file whenever you chat in this repository. This file contains the full CodeQuest system rules — gamification, progress tracking, teaching methodology, and more. You don't need to configure anything; just open the project and start chatting!

Path-specific instructions in `.github/instructions/` are applied when Copilot works with matching files (e.g., `.py`, `.js`, `.ts` files trigger the code-files instructions).

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

Ready to begin? Open **GitHub Copilot Chat** in VS Code and say:
```
I'm ready to begin CodeQuest! Initialize my profile and let's start with the Logic Labyrinth quest line.
```

## ⚙️ Prerequisites

1. **VS Code** installed
2. **GitHub Copilot** extension installed and active
3. **GitHub Copilot Chat** extension installed
4. An active GitHub Copilot subscription (Individual, Business, or Enterprise)

> **Tip**: Make sure "Use Instruction Files" is enabled in your Copilot settings. In VS Code, go to Settings → search for `github.copilot.chat.codeGeneration.useInstructionFiles` and set it to `true`.

## 🆘 Troubleshooting

### "AI doesn't remember me"
- Check if `.context/current-session.md` exists and has your data
- Use `/load-checkpoint latest`
- Verify that `.github/copilot-instructions.md` is being picked up (check the references section in Copilot Chat responses)

### "Context limit reached"
- Create a crystal immediately
- Start new chat with crystal ID

### "Custom instructions not loading"
- Ensure `.github/copilot-instructions.md` is at the correct path
- Ensure "Use Instruction Files" is enabled in VS Code settings
- Check the References section at the top of Copilot Chat responses to confirm `copilot-instructions.md` is listed

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

Remember: The goal isn't to get AI to write code for you — it's to understand programming deeply enough that you won't need AI assistance. CodeQuest makes this journey fun and trackable!

**Happy Learning!** 🎮👨‍💻👩‍💻