# Git Cheat Sheet
Git commands cheat sheet



| Command | Effect|
| --- | --- |
| **CREATE COMMANDS** | |
|git init| Create a new local git repository |
|git clone https://github.com/rohit-patel/Git-Cheat-Sheet | Clone a remote repository locally|
| **LOCAL CHANGES** |  |
|git status | Get update on locally changed files|
|git diff | Get changes in tracked files|
| git add . | Add all existing changes to the next commit |
| git add -p <file> | Add some changes in <file> to the next commit |
| git commit -a | Commit all changes in currently tracked files |
| git commit | Commit staged changes |
| git commit --amend | Amend the last commit |
| **COMMIT HISTORY** |  |
| git log | Show all commits, newest first |
| git log -p <file> | Show tracked history of a file |
| git blame <file> | See change history in <file> by user |
| **BRANCHES AND TAGS** |  |
| git branch -av | List all existing branches |
| git checkotu <branch> | Switch HEAD to <branch>|
| git branch <branch_name> | Create branch <branch_name> based on current HEAD |
| git checkout --track <remote/branch> | Create a new tracking branch based on a remote branch |
| git branch -d <branch> | Delete local <branch> |
| git tag <tag_name> | Make the current commit with a tag |
| **UPDATE AND PUBLISH** |  |
| git remote -v | List all currently configured remotes |
| git remote show <remote> | Show information about a remote |
| git remote add <shortname> <url> | Add new <remote> repository |
| git fetch <remote> | Download all changes from <remote> but don't integrate into HEAD |
| git pull <remote> <branch> | Download changes and merge <remote> into HEAD |
| git push <remote> <branch> | Push local changes to <remote> |
| git branch -dr <remote/branch> | Delete a branch on the remote |
| git push --tags | Publish your tags |
| **MERGE AND REBASE** ||
| git merge <branch> | Merge branch into your current HEAD |
| git rebase <branch> | Rebase your current HEAD onto <branch> |
| git rebase --abort | Abort a rebase |
| git rebase --continue | Continue a rebase after resolving conflicts |
| git mergetool | Use your confgured merge tool to resolve conflicts |
| **UNDO**||
| git reset --hard HEAD | Discard all local changes in your working directory |
| git checkout HEAD <file> | Discard changes in a specific <file> |
| git revert <commit> | Revert a commit by producing a new commit with contrary changes |
| git reset <commit> | Reset HEAD pointer to <commit> and preserve changes as unstaged changes |
| git reset --hard <commit> | Reset HEAD pointer to <commit> and discard all following changes |
| git reset --keep <commit> | Reset HEAD pointer to <commit> and preserve uncommitted local changes |

  
