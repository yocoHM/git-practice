# Practice repository for Git demonstration

## Information about the first lesson

Commands used
- git init : initializes a git repository
- git status : compares the working directory, the current branch, and the staging area.
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
