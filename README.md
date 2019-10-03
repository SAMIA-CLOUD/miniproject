# miniproject

1. **Repository**:
	Generically refers to a central place where data is stored and maintained. A repository can be a place where multiple databases or files are located for distribution over a network, or a repository can be a location that is directly accessible to the user without having to travel across a network. Sometimes GitHub users shorten this to “repo.” It can be local to a folder on your computer, or it can be a storage space on GitHub or another online host. You can keep code files, text files, image files, you name it, inside a repository.


2. **Clone**:
	This command is used to obtain a repository from an existing URL.

	Usage: git clone [url]

3. **Fork**:
	A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project. Mac Windows Linux All. Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea.

4. **Branch**:
	The "branch" command helps you create, delete, and list branches. It's the go-to command when it comes to managing any aspect of your branches - no matter if in your local repository or on your remotes.

	Important Options
	-v -a
	Provides more information about all your branches. Listing your branches, by default, will only show your local branches' names.

	Adding the "-a" flag will make sure remote branches are also included in the list.
	Adding the "-v" flag will make the command more "verbose" and include SHA-1 hashes as well as commit subjects of the latest commits on your branches.

	--no-merged
	Returns all branches that have not been merged into your current HEAD branch. This helps you understand which changes haven't been integrated into your current working context, yet. Note that you can also request all branches that already have been merged in your current HEAD by using the "--merged" option instead.

	-d <branch>
	Deletes a specified branch.

	If the specified branch hasn't been fully merged yet, you'll have to use the capital "-D" flag. Be careful with this, though: deleting branches that contain unmerged data shouldn't be done lightly.
	If you want to delete a remote branch, add the "-r" flag in addition to "-d".

	<new-branch>
	Create a new local branch based on your currently checked out branch. If you also provide a SHA-1 hash of a specific revision, your new branch will use that commit as its starting point.