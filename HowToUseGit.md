# **Git:**

**Git is a distributed version control system (DVCS)** used to **track changes** in **source code** during **software development**.

It allows multiple developers to work on a project simultaneously, manage versions of files, and collaborate efficiently without overwriting each other’s work.





**1) git init:** is the command used to initialize a new Git repository.

**2) git status:** it shows you the current state of your working directory and staging area.

&nbsp; It helps you see:

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

**4-b) git add . =>** used to add **all files** into **Staging Area**



**5) git commit -m "comments"=>** used to add **comments** 



**6) git remote add origin <repo-url> =>** Adds a connection between your local project and GitHub

* **"remote"** = online repository
* **"origin"** = a nickname for the GitHub repository
* **<repo-url>** = the GitHub link



So this **command** is basically saying: “Hey Git, connect my local folder with this GitHub repository.”



**7) git remote -v => check** if you are **connected** to the **online repository**

	It will show something like: 

&nbsp;	origin  https://github.com/YourUserName/YourRepoName.git (fetch)

&nbsp;	origin  https://github.com/YourUserName/YourRepoName.git (push)



&nbsp;  If you see the GitHub link → ✔ Your project is connected to GitHub.

&nbsp;  If nothing shows → ❌ Not connected.



**8) git push origin main =>** Upload your code to GitHub (send changes)/Upload my local commits to the main branch on GitHub.

* git push → push changes
* origin → remote repository
* main → branch name



**9) git pull origin main =>** Download code from GitHub (get changes)

* git push → push changes
* origin → remote repository
* main → branch name







