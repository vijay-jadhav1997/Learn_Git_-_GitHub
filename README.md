# 🛠 Learn Basics of Git and GitHub 🔄👩🏻‍💻

## Git basic commands 

1. **See all configuration setting**
The `git config -l` command lists all the configuration settings for Git in the current repository.

```sh
git config -l
```

2. **Set global configuration with `git config --global `**:

```sh
git config --global user.name "user name goes here"
#* Example
git config --global user.name "vijay-jadhav1997"

git config --global user.email "user email Id goes here"
#* Example
git config --global user.email "example24@gmail.com"

# These commands set our username & emailId to "User Name" & "Email Id" for all Git repositories on our system.

#* We can check this with following command
git config --global user.name  #* Reply wil be =>  vijay-jadhav1997

git config --global user.email  #* Reply wil be =>  example24@gmail.com


```

3. **Initialization of a new Git repository with `git init`**:
  - After running following command, the directory/folder becomes a git repository where we can track changes, commit snapshots, and collaborate with others using Git.
```sh
git init
```

4. **See Git Repo status with `git status` :**
- The following command displays the current status of the Git repository.
- modified files, tracked and untracked files i.e. overall status of Repo.

```sh
git status
```


5. **Stage the changes for next commit with `git commit` :**
- with this command we can basically add new files, stage modified files, and/or stage files for deletion in the very next commit.
- After adding changes with `git add`, usually then after we commit changes with `git commit` to create a snapshot of the staged changes. 

```sh
git add file_1 file_2 ....
git add diractory_name1/ diractory_name2/ ....

#* Example :
git add ./fronend/index.html ./fronend/style.css

git add ./frontend

#* To add all the directories/folders and files
git add .

#* 
git add filename_startswith_letters*
```


6. **Record the staged changes with `git commit` :**
- It creates a snapshot of changes.
- Each commit has a unique identifier (a long string of characters called a "hash") that allow us to refer to it later if we need.

```sh
git commit -m "Commit message goes here in double quotation marks"

#* Examples
git commit -m "feat: add dark mode feature to app"
git commit -m "styl: style home page"

#* directly commit modified tracked files with single command
git commit -a -m "commit message...."
```


7.  **See the history of commit with `git log` :**
- Git log shows us the history of the commits that we have made up until now.

```sh
#* it shows all commits with commit message and 'hash' value or commit id
git log

#* only list online commit 
git log --oneline

#* 
git log -p

#* 
git reflog

```

8.  **Push local Repo to remote origin with `git push` :**
```sh
git push -u origin xyz_branch_name

#* Examples 
git push -u origin main #* 
```



### Branching in Git:
1. **Shows all the branches - `git branch`:**
```sh
git branch #* Shows all the branches consists with current Repo
```

2. **create a new branch with `git branch`:**
```sh
#* creates new branch
git branch branch_name 

git branch dark_mode_feature #* creates new branch with 'dark_mode_feature' name
```

3. **Switch to a particular branch with `git checkout` :**
```sh
#* Switch 'HEAD' to particular branch (existing branch)
git checkout xyz_branch 

git checkout dark_mode_feature #* Switches 'HEAD' to 'dark_mode_feature' branch
```

4. **Create and Switch to a new branch :**
```sh
#* Create new branch and switches 'HEAD' to it:
git checkout -b new_branch_name

git checkout -b new_feature #* Create 'new_feature' branch an switches 'HEAD' to it.
```


5. **Delete a branch :**
```sh
#* Create new branch and switches 'HEAD' to it:
git branch -d xyz_branch_name
git branch -D xyz_branch_name

#* Examples:
git branch -d dark_mode_feature #* delete 'dark_mode_feature' branch
```


---

## Learning in progress....
7.  
```sh
git config -l
```
7.  
```sh
git config -l
```