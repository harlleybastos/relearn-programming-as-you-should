# 🧪 Test Your CodeQuest Setup

## Step 1: Open VS Code
Open the project folder in VS Code with GitHub Copilot installed.

## Step 2: Start a New Copilot Chat
Open GitHub Copilot Chat (Ctrl+Alt+I or Cmd+Alt+I), select **CodeMentor** from the agents dropdown, and paste this exact prompt:

```
I want to test the CodeQuest system. Please:
1. Confirm you can see the custom instructions from .github/copilot-instructions.md
2. Check the current session at .context/current-session.md
3. Initialize me as a new student named "TestCoder"
4. Award me 10 XP for successfully setting up the system
5. Create a checkpoint to save this progress
6. Show me my status dashboard
```

## Step 3: Verify Success
You should see:
- ✅ Confirmation of custom instructions loaded (check References in the response)
- ✅ Your new student profile created
- ✅ XP awarded (10/100 towards Level 2)
- ✅ A checkpoint created with ID like "CQ-2026-03-02-1500-L1"
- ✅ Your status dashboard displayed

## Step 4: Test Continuation
Start a SECOND Copilot Chat, select **CodeMentor** again, and paste:

```
Continue my CodeQuest session.
Load from .context/current-session.md
I should be TestCoder with 10 XP.
```

You should see:
- ✅ "Welcome back TestCoder!"
- ✅ Your 10 XP preserved
- ✅ System ready to continue

## ✅ If Both Tests Pass
Your system is working perfectly! You can now:
1. Start your real learning journey
2. Change your CodeName from TestCoder
3. Begin the Tutorial Island quest

## ❌ If Something Fails
Check:
1. Is GitHub Copilot Chat extension installed and active?
2. Does `.github/copilot-instructions.md` exist at the correct path?
3. Is "Use Instruction Files" enabled in VS Code settings? (Search for `github.copilot.chat.codeGeneration.useInstructionFiles`)
4. Is the `.context/` folder accessible?
5. Do you see `copilot-instructions.md` in the References section of Copilot Chat responses?

## 🎉 Success!
If everything works, delete this test file and start your real journey:
```
Initialize me as a new CodeQuest student.
My name is [YOUR_ACTUAL_NAME].
Let's begin the Tutorial Island!
```