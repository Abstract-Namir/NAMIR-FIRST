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
    4 TPYES OF STATUS- 
    | Status    | Meaning                 | Command to Move to Next Step |
    | --------- | ----------------------- | ---------------------------- |
    | Untracked | New file, not yet added |  git add <-filename->        | 
    | Modified  | Tracked file, changed   |  git add <-filename->        |
    | Staged    | Ready to be committed   |  git commit -m "message"     |
    | Committed | Changes saved in repo   | (No action needed)           |
    to add all files at once CMD- git add .

    CHANGED FILES -----> ADD IN WORKING DIRECTORY -----> COMMITED
 
5)  INIT CMD- used to initialize new repo 
    git init 
    git remote add origin <-link->           
    git remote -v         (to verify remote)  
    git branch            (to check branch)
    git branch -M name    (to rename branch)       
    git push origin main LOCAL->REMOTE