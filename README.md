# git-guide
*A comprehensive reference to commonly used git commands*

## Repository Setup

### Initialize a new repository
```bash
git init
```
### Clone an existing repository
```bash
git clone <repository-url>
```
### Add remote repository
```bash
git remote add origin <repository-url>
```
## Basic Commands

### Check repository status
```bash
git status
```
### Add files to staging
```bash
git add <filename>      # Add specific file
git add .              # Add all files
```
### Commit changes
```bash
git commit -m "commit message"
git commit -am "commit message"  # Add and commit in one step    
```
### Push changes
```bash
git push origin <branch-name>
git push -u origin <branch-name>   # Set upstream branch
```
## Branch Operations

### List branches
```bash
git branch      # Local branches
git branch -r   # Remote branches
git branch -a   # All branches
```
### Create branches
```bash
git branch <branch-name>
git checkout -b <branch-name> # Create and switch to a new branch
```
### Switch branches
```bash
git checkout <branch-name>
git switch <branch-name>
```
### Delete branch
```bash
git delete -d <branch-name>
git branch -D <branch-name>
```

## Working with Changes

### View changes
```bash
git diff                # Unstaged changes
git diff --staged       # Staged changes
```
### Discard changes
```bash
git checkout -- <filename>    # Discard file changes
git restore <filename>        # Modern alternative
git reset --hard    
```
### Temporary store changes
```bash
git stash
git stash pop              # Apply and remove stashed changes
git stash apply            # Apply but keep stashed changes
```
### History and Logs
```bash
git log
git log --oneline
git log --graph
```
## Check specific commit
```bash
git show <commit-hash>
```
## Compare branches
```bash
git diff <branch1> <branch2>
```
### Merging and Rebasing
## Merge branches
```bash
git merge <branch-name>
```
## Rebase branch
```bash
git rebase <branch-name>
```
## Handle merge conflicts
```bash
git merge --abort        # Cancel merge
git rebase --abort       # Cancel rebase
```

### Remote Operations

## Update local repository
```bash
git fetch
git pull
```
## Show remote info
```bash
git remote -v
```

### Configuration
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
git config --list
```
### Advanced Operations
## Revert commit
```bash
git revert <commit-hash>

# Reset to specific commit
git reset --soft <commit-hash>    # Keep changes staged
git reset --mixed <commit-hash>   # Keep changes unstaged
git reset --hard <commit-hash>    # Discard changes

```
## Clean untracked files
```git
git clean -n            # Dry run
git clean -f            # Force clean
```
