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
| git add -p <_file_> | Add some changes in <_file_> to the next commit |
| git commit -a | Commit all changes in currently tracked files |
| git commit | Commit staged changes |
| git commit --amend | Amend the last commit |
| **COMMIT HISTORY** |  |
| git log | Show all commits, newest first |
| git log -p <_file_> | Show tracked history of a file |
| git blame <_file_> | See change history in <_file_> by user |
| **BRANCHES AND TAGS** |  |
| git branch -av | List all existing branches |
| git checkotu <_branch_> | Switch HEAD to <_branch_>|
| git branch <_branch_name_> | Create branch <_branch_name_> based on current HEAD |
| git checkout --track <_remote/branch_> | Create a new tracking branch based on a remote branch |
| git branch -d <_branch_> | Delete local <_branch_> |
| git tag <_tag_name_> | Make the current commit with a tag |
| **UPDATE AND PUBLISH** |  |
| git remote -v | List all currently configured remotes |
| git remote show <_remote_> | Show information about a remote |
| git remote add <_shortname_> <_url_> | Add new <_remote_> repository |
| git fetch <_remote_> | Download all changes from <_remote_> but don't integrate into HEAD |
| git pull <_remote_> <_branch_> | Download changes and merge <_remote_> into HEAD |
| git push <_remote_> <_branch_> | Push local changes to <remote> |
| git branch -dr <_remote/branch_> | Delete a branch on the remote |
| git push --tags | Publish your tags |
| **MERGE AND REBASE** ||
| git merge <_branch_> | Merge branch into your current HEAD |
| git rebase <_branch_> | Rebase your current HEAD onto <_branch_> |
| git rebase --abort | Abort a rebase |
| git rebase --continue | Continue a rebase after resolving conflicts |
| git mergetool | Use your confgured merge tool to resolve conflicts |
| **UNDO**||
| git reset --hard HEAD | Discard all local changes in your working directory |
| git checkout HEAD <_file_> | Discard changes in a specific <_file_> |
| git revert <_commit_> | Revert a commit by producing a new commit with contrary changes |
| git reset <_commit_> | Reset HEAD pointer to <_commit_> and preserve changes as unstaged changes |
| git reset --hard <_commit_> | Reset HEAD pointer to <_commit_> and discard all following changes |
| git reset --keep <_commit_> | Reset HEAD pointer to <_commit_> and preserve uncommitted local changes |

  
