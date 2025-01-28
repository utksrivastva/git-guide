# git-guide
*A comprehensive reference to commonly used git commands*

## Repository Setup

### Initialize a new repository
```git
git init
```
### Clone an existing repository
```git
git clone <repository-url>
```
### Add remote repository
```git
git remote add origin <repository-url>
```
## Basic Commands

### Check repository status
```git
git status
```
### Add files to staging
```git
git add <filename>      # Add specific file
git add .              # Add all files
```
### Commit changes
```git
git commit -m "commit message"
git commit -am "commit message"  # Add and commit in one step    
```
### Push changes
```git
git push origin <branch-name>
git push -u origin <branch-name>   # Set upstream branch
```
## Branch Operations

### List branches
```git
git branch      # Local branches
git branch -r   # Remote branches
git branch -a   # All branches
```
### Create branches
```git
git branch <branch-name>
git checkout -b <branch-name> # Create and switch to a new branch
```
### Switch branches
```git
git checkout <branch-name>
git switch <branch-name>
```
### Delete branch
```git
git delete -d <branch-name>
git branch -D <branch-name>
```

## Working with Changes
