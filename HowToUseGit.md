# **Git:**

**Git is a distributed version control system (DVCS)** used to **track changes** in **source code** during **software development**.

It allows multiple developers to work on a project simultaneously, manage versions of files, and collaborate efficiently without overwriting each other’s work.





**1) git init:** is the command used to initialize a new Git repository.

**2) git status:** it shows you the current state of your working directory and staging area.

  It helps you see:

\- Which files have been modified

\- Which files are staged for the next commit

\- Which files are untracked (not yet added to Git)

\- Which branch you’re currently on



**3-a) git status** → verbose, beginner-friendly explanation

* Full, detailed view
* Explains everything in plain English
* Helpful for beginners
* Shows branch info, hints, and instructions

**3-b) git status -s / git status --short** → concise, quick overview for advanced users

* Short, compact summary
* Ideal for experienced users or quick checks

Uses symbols to show the file state instead of sentences

| **Symbol**       | **Meaning**                           |

| ------------ | --------------------------------- |

| ??           | Untracked file (not added yet)    |

| A            | File added to staging area        |

| M            | File modified                     |

| D            | File deleted                      |

| Left column  | Status in \*\*staging area\*\*        |

| Right column | Status in \*\*working directory\*\*   |



**4-a) git add filename =>** Use to add a **single** **file** into **Staging Area**

>>>>>>> Stashed changes

**4-b) git add . =>** used to add **all files** into **Staging Area**

| Command          | Adds New Files | Adds Modified Files  | Adds Deleted Files | Notes                  |

| ---------------- | -------------- | -------------------- | ------------------ | ---------------------- |

| `git add .`      | ✔ Yes          | ✔ Yes               | ❌ No              | Most commonly used     |

| `git add -A`     | ✔ Yes          | ✔ Yes               | ✔ Yes              | Add EVERYTHING         |

| `git add -u`     | ❌ No          | ✔ Yes               | ✔ Yes              | No new files           |

| `git add <file>` | ✔ Yes (single) | ✔ Yes (single)      | ✔ Yes (single)     | Target a specific file |





**5) git commit -m "comments"=>** used to add **comments**

>>>>>>> Stashed changes



**6) git remote add origin <repo-url> =>** Adds a connection between your local project and GitHub

* **"remote"** = online repository
* **"origin"** = a nickname for the GitHub repository
* **<repo-url>** = the GitHub link



So this **command** is basically saying: “Hey Git, connect my local folder with this GitHub repository.”



**7) git remote -v => check** if you are **connected** to the **online repository**

   If you see the GitHub link → ✔ Your project is connected to GitHub.

It will show something like:



 	origin  https://github.com/YourUserName/YourRepoName.git (fetch)

 	origin  https://github.com/YourUserName/YourRepoName.git (push)



   If you see the GitHub link → ✔ Your project is connected to GitHub.

   If nothing shows → ❌ Not connected.



**8) git push origin main =>** Upload your code to GitHub (send changes)/Upload my local commits to the main branch on GitHub.

* git push → push changes
* origin → remote repository
* main → branch name



**9) git pull origin main =>** Download code from GitHub (get changes)

* git pull → pull changes
* origin → remote repository
* main → branch name



**10) git log => displays** **all the commits** that have been made in your **repository**/ **history of your project**.

Each commit in Git has:

* Who created it
* When it was created
* A unique commit ID (hash)
* The commit message

git log shows ALL of these.



**Why is it useful?**

Check what changes were made | See who made changes (in team projects) | Jump to old versions |

Undo mistakes | Track your progress



**10-a) git log** = full history

**10-b) git log --oneline** = short history

**10-c) git log --graph** => visual branch history



**11-a) git config --global user.name "Your Name"** =>

**11-b) git config --global user.email "your\_email@example.com"** =>



**--global means:**

This setting applies to all Git projects on your computer.



| **Scope**      | **Command Example**                            | **Applies to**           |

| ---------- | ------------------------------------------ | -------------------- |

| \*\***Global**\*\* | git config --global user.email "email"`    | All projects         |

| \*\***Local**\*\*  | git config user.email "email"`             | Only current project |





**12) git diff =>** This shows:

* Files you edited
* What exactly changed
* What is not staged yet



**12-a) git diff --staged / git diff --cached**

Both commands show the differences between:

👉 your staged files (files added with git add)

👉 your last commit (HEAD)



**| Command                    | Purpose                |**

**| -------------------------- | ---------------------- |**

**| `git diff`                 | Unstaged changes       |**

**| `git diff --staged`        | Staged changes         |**

**| `git diff COMMIT1 COMMIT2` | Compare two commits    |**

**| `git diff main test`       | Compare branches       |**

**| `git diff filename.txt`    | Diff for a file        |**

**| `git diff --name-only`     | Show changed filenames |**

**| `git diff --stat`          | Summary of changes     |**



**13) git reset**



**| Command                    | What It Does                 | Safe?       |**

**| -------------------------- | ---------------------------- | ----------- |**

**| `git reset <file>`         | Unstage file                 | ✅ Safe      |**

**| `git reset --soft HEAD~1`  | Undo commit, keep staged     | ✅ Safe      |**

**| `git reset --mixed HEAD~1` | Undo commit, keep changes    | ✅ Safe      |**

**| `git reset --hard HEAD~1`  | Undo commit \& delete changes | ❌ Dangerous |**



**14) git clone**

**14-a) git clone repository-link =>** Creates a new folder and clones repository inside it.

**14-b) git clone repository-link . =>**  Applying **Dot** . Clone the repository into the Current/Same folder.





**15) Touch : touch is NOT a Git command.**

    \*\*It is a Linux / Git Bash command used to create an empty file.\*\*



**16) touch .gitignore =>** it create the empty gitignore file in the directory.

 			Inside .gitignore, you list folders or files Git should skip.

**16-a) notepad .gitignore** => it open gitignore file with notepad application.



**16-b) git rm --cached filename =>** To **stop tracking** an **already tracked file**.

 	because **.gitignore only ignores untracked files**. If a file is already tracked by Git,

 	.gitignore will NOT hide it.



**17) Creating New Branch and their related commands.**

| **Command**                             | **Meaning**                          |

| ----------------------------------- | -------------------------------- |

| git branch                          | List branches                    |

| git branch newBranch                | Create branch                    |

| git checkout branchName             | Switch branch                    |

| git checkout -b newBranch           | Create + switch                  |

| git merge branchName                | Merge branch into current branch |

| git branch -d branchName            | Delete local branch              |

| git push origin --delete branchName | Delete remote branch             |

| git push -u origin branchName       | Publish branch to GitHub         |



 

