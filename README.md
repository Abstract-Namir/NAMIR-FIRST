NAMIR-FIRST
This is my first Git repository
Author – Namir Khan

COMMANDS IN GITHUB

1) CLONE
----------------------------
Purpose: Cloning a repo from remote (GitHub) to your local machine.
Command:  git clone <repo-link>     # REMOTE → LOCAL

2) LS (List Files)
----------------------------
Purpose: Lists all the files in the terminal.
Commands: ls        # Shows visible files  
          ls -a     # Shows hidden files (Linux/macOS)  
          gci -Force  # Shows hidden files (Windows PowerShell)

5) CD (Change Directory)
----------------------------
Purpose: Navigate between folders.
Commands: cd <folder-name>        # Go into a folder  
          cd ..                   # Move out of current folder  
          mkdir <folder-name>     # Create a new folder

7) STATUS
----------------------------
Purpose: Display the current state of your working directory.
Command: git status
### 🟡 4 Types of Git Status
---------------------------------------------------------------------------------------
| **Status**   | **Meaning**                 | **Command to Move to Next Step**       |
|--------------|-----------------------------|----------------------------------------|
| Untracked    | New file, not yet added     | `git add <filename>`                   |
| Modified     | Tracked file, changed       | `git add <filename>`                   |
| Staged       | Ready to be committed       | `git commit -m "your message"`         |
| Committed    | Changes saved in repo       | *(No action needed)*                   |
---------------------------------------------------------------------------------------

To add all files at once Command: git add .
Flow: CHANGED FILES → STAGED (added) → COMMITTED

5) INITIALIZING A NEW FOLDER FOR GIT
----------------------------
Steps: cd ..                                 # Exit current directory (if needed)  
       mkdir <new-folder>                    # Create a new folder  
       cd <new-folder>                       # Enter the folder  
       git init                              # Initialize Git  
Then on GitHub:
       Create a new repository.
       Connect remote:
       git remote add origin <repo-link>  
       git remote -v                         # Verify remote  
       git branch -M main                    # Rename current branch to main  
       git push origin main                 # Push from LOCAL → REMOTE

7) BRANCH COMMANDS
----------------------------
➤ View Branches
       git branch               # Local branches  
       git branch -a            # All branches (local + remote)  
       git branch -r            # Remote branches
➤ Create Branch
       git branch <branch-name>  
       git checkout -b <branch-name>    # Create + switch  
       git switch -c <branch-name>      # Equivalent modern command
➤ Switch Branch
       git checkout <branch-name>  
       git switch <branch-name>         # Preferred modern command
➤ Delete Branch
       git branch -d <branch-name>              # Safe delete  
       git branch -D <branch-name>              # Force delete  
       git push origin --delete <branch-name>   # Delete from remote
➤ Rename Branch
       git branch -m <new-name>
➤ Merge Branch (TERMINAL)
       git merge <branch-name> 
➤ Merge Branch (GITHUB)
Pull Request (PR):
Used to propose and collaborate on changes before merging.
➤ Push Branch
       git push origin <branch-name>  
       git push --set-upstream origin <branch-name>  # Push + track
➤ Pull Branch
       git pull origin main    # REMOTE → LOCAL

9) RESOLVING MERGE CONFLICTS
----------------------------
Occurs when two branches modify the same line. Git needs your help.
Steps to Resolve:       
➤Run:
       git merge <branch-name>
➤Open the conflicted file. You'll see:
<<<<<<< HEAD
code from current branch
=======
code from merging branch
>>>>>>> branch-name
➤Fix the file → Remove the markers.
➤Stage it:
git add <file>
➤Commit:
       git commit
➤To cancel the merge:
       git merge --abort

8) UNDOING CHANGES
----------------------------
➤CASE 1: Undo STAGED changes
       git reset <file>      # Unstage single file  
       git reset             # Unstage all
➤CASE 2: Undo a COMMIT (Single commit)
       git reset HEAD~1
➤CASE 3: Undo MULTIPLE commits
--View history:
       git log
--Use a specific commit hash (UID):
       git reset <commit-UID>
CASE 4: HARD RESET to previous state
       git reset --hard  
       git reset --hard <commit-UID>    # Everything after that is lost
If you mess up:
       git reflog       

10) FORK
----------------------------
A fork is a copy of someone else’s GitHub repository under your own account. You can:
Work independently
Contribute back via pull requests

 

 
