# git Commands Cheat Sheet &nbsp; <img src="https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png" width="30">
## 1. Creating Repositories

* Turns an current directory into a local git repository <br/>
`git init`

* Clones an existing repository from on the internet to your current directory <br/>
`git clone [url]`

* Matchs a remote URL with a specified name <br/>
`git remote add [remote-name] [url]`

## 2. Making Changes

* Lists version history for the current branch <br/>
`git log`

* Shows content differences between two branches <br/>
`git diff [first-branch]...[second-branch]`

* Snapshots the file in preparation for versioning (use * for [file] for adding everything) <br/>
`git add [file]`

* Records file snapshots permanently in version history <br/>
`git commit -m "[descriptive message]"`

## 3. Synchronizing Changes

* Downloads all history from the remote tracking branches <br/>
`git fetch [remote-name] [branch-name]`

* Combines remote tracking branch into current local branch <br/>
`git merge [remote-name] [branch-name]`

* Uploads all local branch commits to the remote repository branch <br/>
`git push [remote-name] [branch-name]`

* Updates your current local working branch with all new commits from the corresponding remote repository branch (combination of git fetch and git merge) <br/>
`git pull [remote-name] [branch-name]`

## 4. Branching

* Creates a new branch <br/>
`git branch [branch-name]`

* Deletes the specified branch <br/>
`git branch -d [branch-name]`

* Switches to the specified branch and updates the working directory <br/>
`git checkout [branch-name]`

* Combines the specified branch’s history into the current branch <br/>
`git merge [branch-name]`

## 5. Reverting Commits

* Undoes all commits after [commit], preserving changes locally <br/>
`git reset [commit]`

* Discards all history and changes back to the specified commit <br/>
`git reset --hard [commit]`

## 6. Starting Over

* Removes all version tracking from your current directory <br/>
`rm -rf .git`
