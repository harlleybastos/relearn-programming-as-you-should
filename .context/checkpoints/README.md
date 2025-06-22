# 📁 CodeQuest Checkpoints Directory

This directory stores all your CodeQuest learning progress checkpoints.

## 🔧 How Checkpoints Work

Checkpoints are automatically created:
- Every 5 completed challenges
- Every 30 minutes of active learning
- When you request a manual save with `/checkpoint`
- Before the AI reaches context limits

## 📄 Checkpoint File Format

Each checkpoint follows this naming convention:
```
CQ-YYYY-MM-DD-HHMM-L[LEVEL].md
```

Example: `CQ-2024-01-20-1430-L5.md` means:
- Created on January 20, 2024 at 14:30
- Student was Level 5 at the time

## 🔄 Using Checkpoints

### To Load a Specific Checkpoint:
```
/load-checkpoint CQ-2024-01-20-1430-L5
```

### To Load the Latest Checkpoint:
```
/load-checkpoint latest
```

## 📊 Checkpoint Contents

Each checkpoint contains:
1. **Complete Student Profile** - Your exact progress state
2. **Achievement Status** - All unlocked achievements and progress
3. **Quest Progress** - Current and completed quests
4. **Code Context** - Your recent code attempts
5. **Learning Map** - Concepts you've mastered
6. **Session Bridge** - Instructions to continue

## 🛡️ Backup Strategy

- Keep at least the last 5 checkpoints
- Archive checkpoints when completing major quests
- The `latest.md` file always links to your most recent checkpoint

## ⚠️ Important Notes

- **Never edit checkpoint files manually** - They're used by the AI to restore your exact state
- **Git commit regularly** - Version control your learning journey
- **Large files** - Checkpoints may grow large; consider archiving old ones

## 🚀 Quick Commands

- `/checkpoint` - Create checkpoint now
- `/list-checkpoints` - Show all available checkpoints
- `/load-checkpoint [ID]` - Load specific checkpoint
- `/checkpoint-info` - Show current checkpoint status

---
*The CodeQuest system manages these files automatically. Just focus on learning!*