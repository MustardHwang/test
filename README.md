# Three Stages:
  - Modified
  - Staged
  - Committed

# Command                                                             :drill:
```shell
git clone
```

# Command                                                             :drill:
```shell
git add
```

# Command                                                             :drill:
```shell
git status
```

# Command                                                             :drill:
```shell
git status -s
```

# Command                                                             :drill:
```shell
.gitignore
```

# Command                                                             :drill:
```shell
git diff
```

# Command                                                             :drill:
```shell
git diff --staged
```

# Command                                                             :drill:
```shell
git diff --cached
```

# Command                                                             :drill:
```shell
git commit
```

# Command                                                             :drill:
```shell
git commit -m <Message>
```

# Command                                                             :drill:
```shell
git -a commit
```

## What does it do?

# Command                                                             :drill:
```shell
git rm <filename>
```

## What does it do?
File is staged for removal. Next commit will remove it from the
filesystem and will no longer be tracked.

If you simply remove the file from the filesystem, Git will see that
it has been deleted but not staged to be committed.

# Command                                                             :drill:
```shell
git rm --cached <filename>
```

## What does it do?
Removes a file from the staging area, but not from your
filesystem/working tree

# Command                                                             :drill:
git mv <original file> <new file>
```

## What does it do?
Renames a file and then stages it for commit.

# Command
git log
```

## What does it do?
Shows commit history

# Command
```shell
git log -p -2
```

# Command
```shell
git log --stat
```

## What does it do?
Show statistics for each commit

# Command
```shell
git log --pretty
git log --pretty=oneline
git log --pretty --graph
git log --since=2008-01-15
git log --since=2.weeks
git log --since="2 years 1 day 3 minutes ago"
git log --author="specific author"
git log --grep="specific commit message"
```

```shell
git log --until
```

# Scenario                                                            :drill:
```shell
git commit --amend
```

## Details
When you need to correct the commit message of an already staged set

# Scenario                                                            :drill:
```shell
git reset HEAD <filename>
```

## Details
when you need to unstage a file

# Scenario
```shell
git checkout -- <filename>
```

## Details
When you need to discard the changes made on the file in your
filesystem

# Command                                                             :drill:
```shell
git branch <branch name>
```

## What does it do?
Creates a branch for you

# Command                                                             :drill:
```shell
git checkout <branch name>
```

## What does it do?
```shell
Switch branch to <branch name>
```

# Command                                                             :drill:
```shell
git checkout -b <branch name>
```

## What does it do?
Creates a branch and switches to it


# Command                                                             :drill:
```shell
git branch -d <branch name>
```

## What does it do?
Deletes branch <branch name>

# Command
```shell
git merge <branch name>
```

## What does it do?
It merges the branch to the current branch that you've switched to.

Behind the scenes, it moves the HEAD pointer to the merged branch.

# Scenario
```shell
git checkout master
git merge hotfix
```

## Details
Switch to master branch, then merge 'hotfix' branch into master
branch.
