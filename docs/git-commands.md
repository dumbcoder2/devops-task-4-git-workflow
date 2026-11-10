# Git Commands Reference Guide

## 1. Git Configuration
- git --version : Check Git version.
- git config --global user.name "Name" : Set username.
- git config --global user.email "email" : Set email.
- git config --list : View Git configuration.

## 2. Repository Management
- git init : Initialize a repository.
- git clone <url> : Clone a remote repository.
- git status : Check working tree status.
- git remote -v : Display remote repositories.
- git remote add origin <url> : Add remote repository.

## 3. File Management
- git add . : Stage all changes.
- git add filename : Stage a specific file.
- git commit -m "message" : Commit changes.
- git commit --amend : Modify the latest commit.
- git restore filename : Discard unstaged changes.
- git restore --staged filename : Unstage a file.
- git rm filename : Remove a tracked file.

## 4. Branch Management
- git branch : List local branches.
- git branch -a : List all branches.
- git branch dev : Create a branch.
- git switch dev : Switch branches.
- git switch -c feature/login : Create and switch branch.
- git branch -d branch-name : Delete a merged branch.
- git merge branch-name : Merge a branch.
- git rebase main : Rebase current branch onto main.

## 5. Remote Operations
- git fetch : Download remote updates.
- git pull : Fetch and integrate remote changes.
- git push : Upload commits.
- git push -u origin branch-name : Push and set upstream.
- git push origin --delete branch-name : Delete remote branch.

## 6. Commit History and Comparison
- git log : View commit history.
- git log --oneline : Compact commit history.
- git log --graph --oneline --all : Visualize branch history.
- git show : View latest commit details.
- git diff : View unstaged changes.
- git diff --staged : View staged changes.
- git blame filename : See who changed each line.

## 7. Stash Commands
- git stash : Temporarily save changes.
- git stash list : List saved stashes.
- git stash apply : Restore latest stash.
- git stash pop : Restore and remove latest stash.
- git stash drop : Delete a stash.

## 8. Tags and Releases
- git tag : List tags.
- git tag v1.0 : Create a lightweight tag.
- git tag -a v1.0 -m "Release" : Create annotated tag.
- git show v1.0 : View tag details.
- git push origin v1.0 : Push a tag.
- git push origin --tags : Push all tags.

## 9. Undo and Recovery
- git revert <commit-id> : Create a commit that reverses changes.
- git reset --soft HEAD~1 : Undo last commit but keep staged changes.
- git reset --mixed HEAD~1 : Undo last commit and unstage changes.
- git reflog : View recent HEAD movements.
- git cherry-pick <commit-id> : Apply a specific commit.

## 10. Useful Maintenance Commands
- git clean -n : Preview untracked files to delete.
- git clean -f : Delete untracked files.
- git gc : Optimize repository storage.
- git fsck : Check repository integrity.

## Note
Be careful with destructive commands such as git reset --hard,
git clean -f and force push. They can permanently discard work.
