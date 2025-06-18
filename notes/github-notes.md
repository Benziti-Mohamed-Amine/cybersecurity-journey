# 1. Clone your GitHub repo to your computer (only once)
git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git

# 2. Move into your project folder
cd YOUR-REPO

# 3. Make changes (add notes, create .md files, etc.)

# 4. Stage ALL your changes
git add .

# 5. Save the snapshot with a message
git commit -m "Your message here"

# 6. Push it to GitHub (the origin)
git push origin main


📁 Your Computer (Local)               🌐 GitHub (Remote)

       ┌────────────┐                        ┌──────────────┐
       │ Your files │                        │ Online repo  │
       └────┬───────┘                        └────┬─────────┘
            │                                     │
       git add .                            git clone
            ↓                                     ↑
    git commit -m "msg"                     git pull
            ↓                                     ↑
       git push origin main  ───────────────────►


# Check current branch
git branch

# Create a new branch
git checkout -b new-feature

# Switch back to main
git checkout main

# Merge your branch into main (after testing)
git merge new-feature

######################################################################################################

# Git & Github explained with GTA(game)

Git is Like Saving Game Progress
Imagine you're playing GTA (or any game with saves).

Git Term	GTA Equivalent	Why It Exists
Repository	Your game install folder	Where all files live
Working Directory	Your current unsaved game	Changes aren’t safe yet
git add	Selecting which missions to save	You don’t want to save everything (e.g., ignore failed missions)
git commit -m	Pressing "Save Game" + naming the save (e.g., "After Heist")	So you know what this snapshot contains
git push	Uploading saves to Rockstar Cloud	Backup in case your PC explodes
git pull	Downloading saves from a friend	Get their progress
Branch	A separate save file for "Evil Playthrough"	Lets you experiment without overwriting your main game

# Real-Life Git Walkthrough (GTA Edition)

You start playing → Git doesn’t track anything yet.

Run git init to start tracking.

You complete a mission → You git add mission1 (stage it).

You save → git commit -m "Completed heist".

You mess up → git checkout -- savefile (reload last save).

You want a "Dark Side" playthrough → git checkout -b evil-path.

# Start tracking your game
git init

# Save mission progress (but don't commit yet)
git add mission2

# Permanently save with a note
git commit -m "Stole a tank"

# Upload saves to cloud (GitHub)
git push

# Try a "no cops" playthrough
git checkout -b no-cops-mode

# Example:

Open a txt file (call it gta_saves.txt).

Pretend it’s a game:

echo "Mission 1: Done" > gta_saves.txt
git add gta_saves.txt
git commit -m "First mission completed"
Now "fail" a mission:

echo "Mission 2: Failed" >> gta_saves.txt
git checkout -- gta_saves.txt  # Undo!

#######################################################################################################

# Configure Git with Github:

💡 git config --global user.name → This is the name that will appear next to your commits.
✅ So yes:
Use your GitHub display name — or any professional name you want shown publicly on GitHub.

Example:

git config --global user.name "YourName"   # or your real name if you prefer
💡 git config --global user.email → This must be the same email as your GitHub account, or GitHub won’t link your commits to your profile.

Example:

git config --global user.email "yourgithubemail@example.com"
✅ You can check your GitHub email here:
Go to github.com → Settings → Emails

If you want to hide your real email, GitHub gives you a noreply email like:

12345678+yourusername@users.noreply.github.com
You can use that too — GitHub will still link it to your account.

Final Step (to check it's correct):

git config --global --list

It should output:

user.name=YourName
user.email=yourgithubemail@example.com

