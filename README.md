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


5) To Initialize a Folder in Terminal:-

->GET OUT OF THE CURRENT FOLDER CMD- cd ..

->CREATE A NEW FOLDER CMD- mkdir <-NEW FOLDER NAME->

->GET INTO THE NEW FOLDER CMD- cd <--FOLDER NAME>

->INITIALIZE THE NEW FOLDER CMD- git init

->CREATE A NEW REPO IN GITHUB

->ADD IT TO YOUR REMOTE REPO CMD- git remote add origin <-link->

->VERIFY YOUR REMOTE CMD- git remote -v

->VERIFY BRANCH (IT SHOULD BE MAIN BY DEFAULT IF NOT )CMD- git branch -M name 

->PUSH IT TO FROM LOCAL->REMOTE CMD- git push prigin main
