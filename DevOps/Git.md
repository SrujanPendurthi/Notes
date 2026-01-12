# Foundations
Three important locations:
	Working Repository
	Staging
	Remote Repository

Working Repository is the repository or directory that we are currently working on locally on our machines

Staging is basically prepping our working repository before sending it to the remote repository
	directories and repository must be staged before making it into a remote repository

Remote Repository is the repository that we see on services like Github

Working Repository Commands:
	mkdir: make a directory/folder
	touch: make a file
	git init: adds git and git tracking to a directory
	git status: tells us which files and directories were modified
	git rm: deletes file
	git restore: brings file back to how it looked in previous commit 
	git revert: brings file back to a certain commit, while making a new commit

Staging Commands:
	git add -all: staging every single change across the project
	git add -A: staging every single change across the project
	git add . : Staging the changes within the current directory
	git add * : staging the only the modified files
	git reset: undo changes by moving the current branch's pointer to a specified previous commit
		git reset HEAD~: rolls it back one version
	git commit -m: adding a message when commit to local repository
	git rm -f: forces deleting a file when the file is not staged
	git rm --cached: removes file from staging but keeps it in working directory

Remote Repository Commands:
	git clone: cloning a specified remote repository to a working repository locally
	git log: see full git commit history
	git diff: will show two commits using the commit ids
	git push: sending local changes to the remote
	git fetch: bringing remote changes into local repository, but not merging them yet
	git pull: fetching plus merging, so your working directory immediately reflects the remote changes

# Git Branching
Git branching is one of the most powerful tools with git

It enables good version control workflows as it basically enables new timelines for code

When developing a new feature, we can make a separate branch, so we can develop, test, and break anything we want before merging back to the main branch

Git Branch Commands:
	git branch: see all branches and can add new ones
		There is an asterisk showing which one you are currently in
	git checkout: enter new branch
	git merge: merging branches in order to combine modifications
		merging the current branch you are in with another branch
	git stash: lets you switch between branches without needing to save modifications
	git stash pop: restores unsaved modifications and removes it from stash
	git stash apply: does same thing as pop, but does not remove it from stash
	git stash list: shows everything in stash
	git rebase: does the same thing as merge, but its rewrites project commit history to keep it clean and linear

Merge Conflicts:
	Happens when there are multiple modifications to the same code, which require manual resolution

Git Pull Requests are requests to the main maintainer of the project to look at modifications in your branch and eventually merge them, done in github or using gh in CLI

# Resources:

https://education.github.com/git-cheat-sheet-education.pdf

https://git-scm.com/cheat-sheet

https://www.youtube.com/watch?v=mAFoROnOfHs&t=241s

