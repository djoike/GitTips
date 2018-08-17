# GIT commands

## Pulling

**Pulling**
`pull upstream master`
`pull {remote} {branch}`

## Changes

**List of changes**
`status`

**Stage all changes**
`add .`

**Stage all changes - dry run**
`add . -n`

**Stage specific things**
`add *.js`
`add {file name pattern}`

**Unstage all**
`git reset`

**Unstage file**
`git reset <file>`

## Committing

**Committing**
`commit -m "Commit message"`
`commit -m "{commit message}"`

## Pushing

**Pushing**
`push origin SUP-12345`
`push origin {branch name}`

## Branches

**List local branches**
`branch`

**List remote branches**
`branch -r`

**Delete local branch**
`branch -D SUP-12345`
`branch -D {branch name}`

**Create a new branch**
`checkout master -b SUP-12345`
`checkout {existing branch name} -b {new branch name}`

**Create a new branch from remote**
_Remember it might be necessary to fetch before, if the remote branch is new_
`git checkout -b SUP-12345 djoike/SUP-12345`
`git checkout -b {new branch name} {name of remote}/{existing branch name}`

**Rename branch, if you are already on the branch**
`git branch -m {new-name}`
`git branch -m SUP-12345`

**Rename branch, if you are on a different branch**
`git branch -m {old-name} {new-name}`
`git branch -m SUP-75890 SUP-12345`

## Fetching

**Fetch from specific remote**
`git fetch upstream`
`git fetch {name of remote}`

## Remotes
**Add new remote**
`git remote add {remote-name} {remote-url}`
`git remote add mov git@github.com:djoike/Masterpiece.git`

## Housekeeping

### Discarding untracked changes
**Removing untracked and unstaged files — dry run**
`clean -n`

**Removing untracked and unstaged files**
`clean -f`

**Removing untracked and unstaged files & folders - dry run**
`clean -d -n`

**Removing untracked and unstaged files & folders**
`clean -d -f`

### Removing unstaged
**Discard versioned, but unstaged**
For a specific file use:
`git checkout path/to/file/to/revert`

For all unstaged files use:
`git checkout -- .`

## Cloning

**Clone repository**
`git clone {repository-url}`
*(Will create a folder for the repository, so do it in the parent folder)*
