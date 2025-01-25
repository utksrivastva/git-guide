# git-guide
*A comprehensive reference to commonly used git commands*

## Repository Setup

### Initialize a new repository
git init

### Clone an existing repository
git clone <repository-url>

### Add remote repository
git remote add origin <repository-url>

## Basic Commands

### Check repository status
git status

### Add files to staging
git add <filename>      # Add specific file
git add .              # Add all files

### Commit changes
git commit -m "commit message"
git commit -am "commit message"    # Add and commit in one step

### Push changes
git push origin <branch-name>
git push -u origin <branch-name>   # Set upstream branch
