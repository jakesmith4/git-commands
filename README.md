# **GIT BASH COMMANDS**

## **_CREATING & DELETING FILES & FOLDERS_**

---

### Going Into A Folder

```bash
cd {folder name}

cd /c/Projects
```

### Going Out Of A Folder

```bash
cd ..
```

### Creating A Folder Or Directory

```bash
mkdir {folder name}
```

### Deleting A Folder Or Directory

```bash
rm -r {folder name}
```

### Create File

```bash
touch {file name}
```

### Delete File

```bash
rm {file name}
```

### Delete File & Stage Changes All In One Go

```bash
git rm {file name}
```

### Open Up VS Code In A File

```bash
code {file name}
```

## **_RENAMING FILES_**

---

### Renaming A File

```bash
mv {file name} {file name to rename to}
```

### Rename & Stage A File All In One Go

```bash
git mv {file name} {file name to rename to}
```

## **_INITALIZING AS A GIT REPOSITORY_**

---

### Initalize A Folder As A Git Repo

```bash
git init
```

### Add Files or File To Staging Area

```bash
git add .

git add {file name}
```

### Committing Files To Repo

```bash
git commit -m "Inital Commit"
```

> THEN GO TO GITHUB AND CREATE A _**NEW REPO.**_ THEN COPY THE _**GIT REMOTE COMMAND.**_ THEN DO THE _**FOLLOWING COMMAND**_

```bash
git push -u origin master
```

### Push Changes Github After Inital Push

```bash
git push
```

### Stage & Commit Files At The Same Time

```bash
git commit -am "{message goes here}"
```

## **_CLONING A GITHUB REPOSITORY_**

---

### Cloning A Repo

> GO TO THE REPO YOU WANT TO CLONE ON _**GITHUB**_ THEN CLICK THE _**GREEN CODE BUTTON.**_ COPY THE _**LINK**_ FROM THE REPO YOU WANT TO CLONE, IT WILL BE THE _**LINK**_ UNDER THE _**HTTPS**_ TAB, NOT THE SSH TAB. THEN RUN THE _**FOLLOWING COMMAND**_ IN THE FOLDER OR DIRECTORY YOU WANT THE FILES TO BE CLONED IN

```bash
git clone {copyed repo link from github (THE REPO YOU WANT TO COPY)}
```

## **_REMOVING FILES OR RESTORING/REVERTING_**

---

### Remove A File Or All Files From Staging Area

```bash
git restore --staged {file name}
```

### Remove Files Or Changes From Working Directory Or _**REVERT BACK**_

```bash
git restore .

git restore {file name}
```

## **_Remove Untracked Files_**

```bash
git clean -fd
```

### Restore The Last File Already Commited

```bash
git restore --source=HEAD~1 {name of file}
```

### Append Text To A File

```bash
echo {text goes here} >> {file name here}
```

### Replace The Text In A File

```bash
echo {text goes here} > {file name here}
```

## **_Checking The Status Of Your Repo_**

---

### Check The Status

```bash
git status

git status -s
```

### See All Files In The Current Directory

```bash
git ls-files
```

### Check What Changes Were Made To ALL Files In The Staging Area

```bash
git diff --staged
```

### Check What Changes Were Made In The Working Directory

```bash
git diff
```

### Check To See If A Repo Has Has An Origin Or Is Already In Github

```bash
git remote
```

### See A Log Of All Commits

```bash
git log --oneline
```

## **_BRANCHES_**

---

### See Branches

```bash
git branch
```

### Add Branch

```bash
git branch {branch name}
```

### Switch Branches

```bash
git checkout {branch name}
```

### Merge Branches (From Master)

```bash
git merge {branch name}
```

> _**IF THE BASH WANTS INPUT:**_ THEN PRESS _**I**_ FOR INSERT, THEN TYPE _**Added {Your Text Here}**_ THEN PRESS _**ESC.**_ THEN PRES _**:wq**_

### Deleting A Branch

```bash
git branch --delete {branch name}
```

## **_GIT IGNORE_**

---

### Git Ignore

> ADD PATHS INTO A **.gitignore** FILE FOR GIT TO ALWAYS IGNORE THESE FILES OR DIRECTORYS, AND NEVER THEM ADD TO THE STAGING AREA

### Create a Gitignore File

```bash
touch .gitignore
```

## **CONFIGURATION SETTINGS\_**

---

### See Config Settings In VS CODE

```bash
git config --global -e
```
