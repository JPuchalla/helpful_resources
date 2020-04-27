# GitHub Flow

<p align="center">
<img width=100% height=100% src="https://guides.github.com/activities/hello-world/branching.png">
</p>

## Configure tooling

#### Enables helpful colorization of command line output:

```javascript 
git config --global color.ui auto
```

#### Sets the email you want attached to your commit transactions:

```javascript
git config --global user.email "[email address]"
```

#### Sets the name you want attached to your commit transactions:

```javascript 
git config --global user.name "[name]"
```

## Create repositories

#### Turn an existing directory into a git repository:

```javascript 
git init
```

#### Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits:

```javascript 
git clone [url]
```

## Synchronize changes

#### Uploads all local branch commits to GitHub:

```javascript 
git push
```

#### Combines remote tracking branch into current local branch:

```javascript 
git merge
```

#### Downloads all history from the remote tracking branches:

```javascript 
git fetch
```

#### Updates your current local working branch with all new commits from the corresponding remote branch on GitHub:

```javascript 
git pull
```

 * `git pull` is a combination of `git fetch` and `git merge`

## Branches

#### Checks current branch:

```javascript
git status
```

#### Deletes the specified branch:

```javascript 
git branch -d [branch-name]
```

#### Combines the specified branch’s history into the current branch:

```javascript 
git merge [branch]
```

#### Switches to the specified branch and updates the working directory:

```javascript 
git checkout [branch-name]
```

#### Creates a new branch:

```javascript 
git branch [branch-name]
```

## Make changes

#### Lists version history for the current branch:

```javascript 
git log
```

#### Lists version history for a file, including renames:

```javascript 
git log --follow [file]
```

#### Shows content differences between two branches:

```javascript 
git diff [first-branch]...[second-branch]
```

#### Outputs metadata and content changes of the specified commit:

```javascript 
git show [commit]
```

#### Snapshots the file in preparation for versioning:

```javascript 
git add [file]
```

#### Records file snapshots permanently in version history:

```javascript 
git commit -m "[descriptive message]"
```

## Redo commits

#### Undoes all commits after [commit], preserving changes locally:

```javascript 
git reset [commit]
```

#### Discards all history and changes back to the specified commit:

```javascript 
git reset --hard [commit]
```

* CAUTION! Changing history can have nasty side effects. If you
  need to change commits that exist on GitHub (the remote),
  proceed with caution.
