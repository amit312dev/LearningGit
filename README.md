# 🚀 Learning Git Like a Pro  

![Git](https://img.shields.io/badge/Git-Mastering-orange?logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-Learning-black?logo=github)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Made with ❤️](https://img.shields.io/badge/Made%20with-%E2%9D%A4-red)

---

## 📚 About This Repo
Welcome to my **Git & GitHub learning journey**!  
Here, I explore:
- 🛠 **Basic Git commands**
- 🔄 Branching, committing & pushing
- 🌐 Syncing with GitHub like a pro

---

## 🛠 Git Commands I’ve Learned
```bash
git init                   # Initialize a new repo
git add .                  # Stage changes
git commit -m "message"    # Commit changes
git branch -M main         # Rename branch to main
git remote add origin <url> # Connect to GitHub
git push -u origin main    # Push code
git pull                   # Get latest changes

Project Structure-
hello-git/
│
├── README.md       # This epic guide 😎
├── hello.txt      # Test file first
└── a.txt       # Test file second

## 📚 Some extra features
🔄 Git Sync Aliases
To save time on adding, committing, pulling, and pushing changes, you can set up custom Git aliases. These shortcuts let you sync changes with one simple command.

1️⃣ Auto-Timestamp Sync
This version automatically creates a commit message with the current date and time.

Setup
Run this once in your terminal:
git config --global alias.sync '!b=$(git rev-parse --abbrev-ref HEAD) && git add . && git diff-index --quiet HEAD || git commit -m "Sync on $(date +"%Y-%m-%d %H:%M:%S")" && git pull --rebase origin $b && git push origin $b'

## Usage
From any Git repo: Just provide following command in git bash terminal
git sync

What it does:

1. Detects the current branch (main, master, or others)

2. Adds all changes

3. Commits with a timestamp (only if there are changes)

4. Pulls the latest changes from GitHub with --rebase

5. Pushes your commits to the remote branch

2️⃣ Manual Message Sync
This version lets you enter your own commit message instead of using a timestamp.

Setup
Run this once:
git config --global alias.syncm '!f() { b=$(git rev-parse --abbrev-ref HEAD); git add .; git commit -m "$1"; git pull --rebase origin $b; git push origin $b; }; f'

## Usage
From any Git repo: Run following command in git bash terminal
git syncm "Your custom commit message here"

💡 Tips
You can use both versions — git sync for quick saves, git syncm when you need a meaningful commit message.

These aliases work in any repository on your system after setup.

If you ever want to see your saved aliases, run: git config --global --get-regexp alias

💡 Fun Git Tip
“Commit often, push regularly, and never fear the merge!” 💪

👨‍💻 Author
Amit Singh
📧 Email: amit1scriet312@gmail.com
🔗 GitHub: amit312dev

⭐ If you found this while browsing, drop a star to make my day! ⭐


