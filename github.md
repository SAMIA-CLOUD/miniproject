# Saleena John
# Github

1. **Repository**:
	
	Generically refers to a central place where data is stored and maintained. A repository can be a place where multiple databases or files are located for distribution over a network, or a repository can be a location that is directly accessible to the user without having to travel across a network. Sometimes GitHub users shorten this to “repo.” It can be local to a folder on your computer, or it can be a storage space on GitHub or another online host. You can keep code files, text files, image files, you name it, inside a repository.

 ![Repository](/images/repo.png)

2. **Clone**:
	
	This command is used to obtain a repository from an existing URL.

	Usage: git clone [url]

![Clone](/images/clone.PNG)

3. **Fork**:
	
	A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project. Mac Windows Linux All. Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea.

4. **Branch**:
	
	The "branch" command helps you create, delete, and list branches. It's the go-to command when it comes to managing any aspect of your branches - no matter if in your local repository or on your remotes. 

	![Branch](/images/branch.png)

	**Important Options**
	
	* -v -a
	
	Provides more information about all your branches. Listing your branches, by default, will only show your local branches' names.

	Adding the "-a" flag will make sure remote branches are also included in the list.
	
	Adding the "-v" flag will make the command more "verbose" and include SHA-1 hashes as well as commit subjects of the latest commits on your branches.

	* --no-merged

	Returns all branches that have not been merged into your current HEAD branch. This helps you understand which changes haven't been integrated into your current working context, yet. Note that you can also request all branches that already have been merged in your current HEAD by using the "--merged" option instead.

	* -d [branch]
	
	Deletes a specified branch.

	If the specified branch hasn't been fully merged yet, you'll have to use the capital "-D" flag. Be careful with this, though: deleting branches that contain unmerged data shouldn't be done lightly.

	If you want to delete a remote branch, add the "-r" flag in addition to "-d".

	* [new-branch]
	
	Create a new local branch based on your currently checked out branch. If you also provide a SHA-1 hash of a specific revision, your new branch will use that commit as its starting point.

5. **Commit**:
	
	The git commit command captures a snapshot of the project's currently staged changes.
	The "commit" command is used to save your changes to the local repository.
	
	A commit is not automatically transferred to the remote server. Using the "git commit" command only saves a new commit object in the local Git repository. Exchanging commits has to be performed manually and explicitly (with the "git fetch", "git pull", and "git push" commands).

	![Commit](/images/commit.png)

	**Important Options**
	
	* -m [message]
	
	Sets the commit's message. Make sure to provide a concise description that helps your teammates (and yourself) understand what happened.

	* -a
	
	Includes all currently changed files in this commit. Keep in mind, however, that untracked (new) files are not included.

	* --amend
	
	Rewrites the very last commit with any currently staged changes and/or a new commit message. Git will rewrite the last commit and effectively replace it with the amended one. Note that such a rewriting of commits should only be performed on commits that have not been pushed to a remote repository, yet.

	![Committypes](/images/committypes.PNG)


6. **Merge**:
	
	Merging is Git's way of putting a forked history back together again. The git merge command lets you take the independent lines of development created by git branch and integrate them into a single branch.
	The "merge" command is used to integrate changes from another branch.

	![Merge](/images/merge.png)
	
	The target of this integration (i.e. the branch that receives changes) is always the currently checked out HEAD branch.


	![Mergeexample](/images/mergeex.png)


7. **Checkout**:
	
	The git checkout command lets you navigate between the branches created by git branch . Checking out a branch updates the files in the working directory to match the version stored in that branch, and it tells Git to record all new commits on that branch.
	
	The "checkout" command can switch the currently active branch - but it can also be used to restore files.
	The most common use case for "checkout" is when you want to switch to a different branch, making it the new HEAD branch.

	Another use case for "checkout" is when you want to restore a historic version of a specific file. Thereby, you can reset single files to earlier revisions - while keeping the rest of the project untouched.

	![Checkout](/images/checkout.png)

	**Important Options**
	
	* [branch-name]
	
	The name of a local branch that you want to switch to. By specifying the name of a local branch, you will switch to this branch and make it the current "HEAD" branch.

	* -b [new-branch]
	
	Creates a new local branch and directly switches to it. This can be used as a shortcut instead of the following two commands:
	
	git branch [new-branch-name]
	
	git checkout [new-branch-name]

	* -b [new-branch] --track [remote-branch]
	
	Creates a new local branch - and sets up an "upstream" configuration. This way, the new local branch has a tracking relationship with its remote counterpart. This allows you to more easily see when the two aren't in sync (i.e. when unpushed commits in the local branch or unpulled commits in the remote exist).

	* [file-path] [commit-hash]
	
	Restores a historic revision of a given file. By providing HEAD as the revision, you can restore the last committed version of a file - effectively undoing any local changes that happened since then. If you want to restore a specific earlier revision you can provide that revision's SHA-1 hash.

8. **Push**:
	
	The git push command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo. It's the counterpart to git fetch , but whereas fetching imports commits to local branches, pushing exports commits to remote branches.

	The "push" command is used to publish new local commits on a remote server.

	The source (i.e. which branch the data should be uploaded from) is always the currently checked out HEAD branch.

	The target (i.e. which branch the data should be uploaded to) can be specified in the command's options. These options can be omitted, however, if a tracking relationship with a remote branch is set up.

	![Push](/images/push.png)

	**Important Options**

	* --all
	
	Pushes all local branches.

	* --tags
	
	Pushes all local tags.

	* --delete
	
	Deletes the specified remote branch.

	* -u
	
	Creates an upstream tracking connection and is especially useful when publishing a local branch on a remote for the first time.

9. **Pull**:
	
	git pull is a Git command used to update the local version of a repository from a remote. It is one of the four commands that prompts network interaction by Git. By default, git pull does two things. Updates the current local working branch (currently checked out branch)

	The "pull" command is used to download and integrate remote changes.

	The target (which branch the data should be integrated into) is always the currently checked out HEAD branch. By default, pull uses a merge operation, but it can also be configured to use rebase instead.

	**Important Options**
	
	* --no-ff

	Creates a merge commit even when a fast-forward would be possible.

	* --rebase

	Integrates changes using rebase instead of merge.

10. **Status**:

	The git status command displays the state of the working directory and the staging area. It lets you see which changes have been staged, which haven't, and which files aren't being tracked by Git. Status output does not show you any information regarding the committed project history.
