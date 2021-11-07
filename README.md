# Git Cheat Sheet
Git commands cheat sheet


| Command | Effect|
| --- | --- |
| **CREATE COMMANDS** | |
| git init | Create a new local git repository |
| git clone https://github.com/rohit-patel/Git-Cheat-Sheet | Clone a remote repository locally |
| **LOCAL CHANGES** |  |
| git status | Get update on locally changed files |
| git diff | shows difference between working directory and staging area |
| git diff --staged | difference between staging area and last commit |
| git add <_files_> | Add <_files_> to the next commit (stage) |
| git add . | Add all existing changes, including untracked files but excluding ignored files, to the next commit |
| git add -p <_file_> | Add some changes(hunks) in <_file_> to the next commit interactively |
| git restore --staged <_files_> | Unstage <_files_> |
| git restore --staged . | Unstage all files |
| git restore <_files_> | to discard changes of <_files_> in working directory. Revert to staged version if it is there other wise revert to last committed version |
| git restore . | to discard changes of <_file_> in working directory. Revert to staged version if it is there other wise revert to last committed version |
| git commit -a | Stage and Commit all changes of currently tracked files |
| git commit | Commit staged changes |
| git commit -m "message" | Commit staged file with commit message without invoking editor |
| git commit --amend | Amend the last commit |
| **COMMIT HISTORY** |  |
| git log  | Show all commits reachable from HEAD, newest first |
| git log <_commit1_> ^<_commit2_> | Show all commits reachable from <_commit1_> but isn't reachable by <_commit2_>. Branch name instead of commit hash can also be used |
| git log -p | Shows changes alongwith each commit reachable from HEAD |
| git log -p -- <_file_> | Show changes of each commit reachable from HEAD |
| git log -p <_commit_> -- | Show changes of each commit reachable from <_commit_> |
| git log --since="2 weeks ago" -- <_file_> | Show changes during last two weeks to file <_file_> |
| git log --stat --summary | Show overview of changes alongwith commits reachable from HEAD |
| git blame <_file_> | See change history in <_file_> by user |
| **BRANCHES AND TAGS** |  |
| git branch | List all existing local branches |
| git branch -r | List all existing remote branches |
| git branch -a | List all existing branches from both local and remote |
| git branch -av | List all existing branches |
| git switch <_branch_name_> | Switch HEAD to <_branch_> |
| git checkout <_branch_> -- | Switch HEAD to <_branch_> |
| git branch <_branch_name_> | Create branch <_branch_name_> based on current HEAD |
| git switch  -c  new-branch | To create and swtich to new branch in one go |
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
| git merge --abort | Abort merging |
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
