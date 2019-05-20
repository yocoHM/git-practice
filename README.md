# Practice repository for Git demonstration

## Information about the first lesson (commit and add)

Commands used
- git init : initializes a git repository
- git status : compares the working directory, the current branch, and the staging area
	- Red files mean that they are being untracked 
	- Green files mean they are being tracked and are added to a “staging area”
- git add <file> : adds files to tracking 
	- When git add is used on a directory, it also 	adds all the files in it 
- git commit : It’s like a snapshot from your work at a point in time
	This command opens vim to add a message to a commit
	After a commit, the terminal shows branch, commit id, and a summary of the change
- git commit -m "comment" : specifies the comment about the commit in the same command
- git log : gives information about the repository's history
	The most recent commit is at the top

Information
.git directory : is where Git stores all the information about the repository

## Information about the second lesson
- git branch <branchName> : creates a new branch
- git branch : lists branches created and marks the one that you are currently working on

## Information about the third lesson
- git log <branchName> : shows the commit history from the specified branch
- git log <commitID> : shows the history from a commit and prior to it
- git log --all : shows all commits (all branches)
- git log --author "authorName" : search commits from a specific person
- git log --since "date/months/days/hours/minutes ago" : commits made since the specified time
- git log --until "date/months/days/hours/minutes ago" : commits made prior to the specified time
- git log --oneline : shows one commit per line
- git log --graph : shows the commits with a graph view
	Any combination of the previous log commands can be made.
- git show <commitID> : shows detailed information and differences of a commit
	A blank in the first column means that a line is just context
	A plus means that a line was added
	A minus means that a line was removed
- git diff : shows the difference between the working directory and HEAD
- git diff <commitID> : shows the difference between the working directory and the specified commit
- git diff --cached : shows the difference between staging area and HEAD
- git diff --cached <commitID> : shows the difference between staging area and the specified commit
- git diff --cached <branchName> : shows the difference between staging area and the specified branch
- git diff <commitID>..<commitID> : shows the difference between two commits
- git diff <branchName>..<branchName> : shows the difference between two branches

## Information about the third lesson (merging)
- git merge <branchName> : brings the changes from the specified branch, to the current branch
	Fast forward merge happens when the target branch was branched from the current one, and there are no new changes to the current branch since then 
	An automatic merge happens when the two histories have diverged, but Git is able to reconcile them into one set of changes. It creates a new commit on the current branch
- git branch -d <branchName> : deletes the specified branch