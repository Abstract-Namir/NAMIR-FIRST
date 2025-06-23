# NAMIR-FIRST
<br>
this is my first GIT REPOSITORY 
Author- Namir Khan

COMMANDS in GITHUB
1)  CLONE- cloning a repo from remote(GITHUB) in our local machine(laptop/PC)
    CMD- git clone <-repo link-> REMOTE->LOCAL

2)  LS(LIST FILES)- lists all the files 
    ls in the TERMINAL to access hidden files (ls -a) OR gci -Force
  
3)    CD(CHANGE DIRECTORY)- going from one folder to another folder CMD-cd <-file name-> in the TERMINAL
      to get out of existing directory CMD- cd ..
      to create a new directory CMD- mkdir new <-folder name->  

4)  STATUS- display the state of the code
    CMD- git status
    4 TYPES OF STATUS- 
    | Status    | Meaning                 | Command to Move to Next Step |
    | --------- | ----------------------- | ---------------------------- |
    | Untracked | New file, not yet added |  git add <-filename->        | 
    | Modified  | Tracked file, changed   |  git add <-filename->        |
    | Staged    | Ready to be committed   |  git commit -m "message"     |
    | Committed | Changes saved in repo   | (No action needed)           |
    to add all files at once CMD- git add .

    CHANGED FILES -----> ADD IN WORKING DIRECTORY -----> COMMITED


5) To Initialize a Folder in Terminal:-

->GET OUT OF THE CURRENT FOLDER CMD- cd ..
->CREATE A NEW FOLDER CMD- mkdir <-NEW FOLDER NAME->
->GET INTO THE NEW FOLDER CMD- cd <--FOLDER NAME>
->INITIALIZE THE NEW FOLDER CMD- git init
->CREATE A NEW REPO IN GITHUB
->ADD IT TO YOUR REMOTE REPO CMD- git remote add origin <-link->
->VERIFY YOUR REMOTE CMD- git remote -v
->VERIFY BRANCH (IT SHOULD BE MAIN BY DEFAULT IF NOT )CMD- git branch -M name 
->PUSH IT TO FROM LOCAL->REMOTE CMD- git push origin main
 
6) BRANCH COMMANDS
->View Branches
git branch                                      # List local branches        
git branch -a                                   # List all (local + remote)
git branch -r                                   # List remote branches

->Create Branch
git branch <branch-name>                        # Create new branch
git checkout -b/-c <branch-name>                # Create + switch to new branch

->Switch Branch
git checkout <branch-name>                      # Switch to branch
git switch <branch-name>                        # Preferred way

->Delete Branch (TO DEL A BRANCH YOU FIRST NEED TO SWITCH FROM EXISTING BRANCH)
git branch -d <branch-name>                     # Delete local branch (safe)
git branch -D <branch-name>                     # Force delete (unsafe)
git push origin --delete <branch>               # Delete remote branch

->Rename Branch
git branch -m <new-name>                        # Rename current branch

->Merge Branch (TERMINAL)
git merge <branch-name>                         # Merge into current branch

->Merge Branch (GITHUB)
PR(Pull Request)- LETS YOU TELL OTHERS ABOUT YOU'VE PUSHED TO A BRANCH IN A REPO IN GITHUB 

->Push Branch
git push origin <branch-name>                   # Push branch to GitHub
git push --set-upstream origin <branch-name>    # Push + track remote

->Pull Branch 
git pull orign main                             # From remote repo -> local repo

6) Resolving Merge Conflicts
Happens when both branches edit the same line in a file. Git can't decide what to keep → you have to manually fix it.
Steps to Resolve:
->Run git merge <branch> → conflict shows up.
->Open conflicted file → Git marks the conflict like:

<<<<<<< HEAD
code from current branch
=======
code from merging branch
>>>>>>> branch-name

->Edit the file: remove conflict markers and fix the content.
->Stage it: git add <file>
->Commit it: git commit

TO CANCEL MERGE CMD- git merge --abort

7) UNDOING CHANGES (Changes that were not meant to be added/commited)
CASE 1:STAGED changes
CMD- git reset <-file name->                    # For single file
CMD- git reset                                  #for all files  

CASE 2:COMMITED changes (for single commit)
CMD- git reset HEAD~1

CASE 3:COMMITED changes (for many commits)
TO CHECK ALL THE COMMITS CMD- git log
when you want to jump from one commit to several commits back you use that specefic commit's UID such as: e5f6a9d3a93f45a9c087c81f54fbd2a6f0a3e0b1

CMD- git reset <-commit UID->
CMD- git reset <-commit UID-> 

CASE 4:RETURN TO SQUARE 1 changes
when you want to reset all the commits 
CMD- git reset --hard
CMD- git reset --hard<-UID->                    #Any changes you made after that commit are GONE.

TO RECOVER IF MESSED UP
CMD- git reflog

8) FORK
A fork is a copy of someone else’s GitHub repository under your own GitHub account.




