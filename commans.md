In DevOps, Git is the foundation for Version Control and CI/CD pipelines, managing code as the "single source of truth" for infrastructure and applications. 

1. Core Repository Management
git init: Initializes a new local repository in the current directory.
git clone [url]: Creates a local copy of an existing remote repository, including its entire history.
git remote add origin [url]: Connects your local repository to a remote server.
git status: Shows the state of the working directory and staging area, highlighting modified or untracked files. 

2. Development Workflow (Stage & Commit)
git add [file]: Adds a specific file to the staging area; use git add . for all changes.
git commit -m "[message]": Records your staged changes with a descriptive message to the local history.
git commit --amend: Modifies the most recent commit, useful for fixing a typo in the message or adding a forgotten file.
git log --oneline --graph: Displays a visual representation of the commit history, essential for tracking deployment versions in pipelines. 
   
3. Branching & Merging (Collaboration)
git branch [name]: Creates a new branch for a feature or fix.
git checkout -b [name]: Creates and immediately switches to a new branch.
git switch [name]: The modern alternative to checkout for switching branches.
git merge [branch]: Integrates changes from a specified branch into the current one.
git rebase [branch]: Reapplies commits on top of another base tip to maintain a linear history. 
   
4. Syncing with Remote Repositories
git fetch: Downloads objects and refs from another repository without merging them into your current work.
git pull: Fetches and immediately merges remote changes into your local branch.
git push: Uploads local commits to the remote repository, which often triggers CI/CD build pipelines. 
DEV Community
DEV Community
 +4
5. DevOps Special Operations
git tag [tagname]: Marks specific points in history, such as release versions (e.g., v1.0.0), often used to trigger production deployments.
git push --tags: Pushes all local tags to the remote server.
git stash: Temporarily saves uncommitted changes so you can switch branches for urgent hotfixes without losing work.
git cherry-pick [commit_id]: Applies a single specific commit from one branch to another, useful for porting critical bug fixes.
git bisect: A debugging tool that uses binary search to find which commit introduced a bug. 
DEV Community
DEV Community
 +6
6. Reverting & Recovery
git revert [commit_id]: Creates a new commit that undoes the changes of a previous commit; this is safer for public branches than resetting.
git reset --hard [commit_id]: Resets the current branch to a specific commit and permanently deletes all local changes.
git clean -fd: Removes all untracked files and directories, helpful for cleaning build artifacts before a fresh run.
git reflog: Shows a history of all Git actions, allowing you to recover deleted branches or commits. 
LinkedIn
LinkedIn
 +5
