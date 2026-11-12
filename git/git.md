# Git Documentation

## 1. Introduction

Git is a free and open-source distributed version control system. It is used to track changes in source code and other files during software development.

Git allows multiple developers to work on the same project while maintaining a history of changes.

## 2. Features of Git

- Tracks changes made to files.
- Maintains the history of a project.
- Supports collaboration among developers.
- Allows users to create and manage branches.
- Supports merging changes from different branches.
- Works locally without requiring an internet connection for most operations.
- Helps recover previous versions of files.

## 3. Important Git Terminology

| Term | Meaning |
|---|---|
| Repository | A location where project files and their history are stored. |
| Commit | A saved snapshot of project changes. |
| Branch | An independent line of development. |
| Working Directory | The folder containing the project files. |
| Staging Area | The area where changes are prepared before committing. |
| Clone | A local copy of an existing repository. |
| Merge | Combining changes from different branches. |
| Remote | A repository hosted on another computer or service. |

## 4. Installing and Configuring Git

After installing Git, configure the username and email address:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Check the configuration:

```bash
git config --list
```

## 5. Creating a Repository

### Initialize a new repository

```bash
git init
```

This initializes a new Git repository in the current directory.

### Clone an existing repository

```bash
git clone <repository-url>
```

This downloads an existing repository to the local computer.

## 6. Basic Git Commands

### Check repository status

```bash
git status
```

Displays the current state of the working directory and staging area.

### Add files to the staging area

```bash
git add filename
```

Adds a particular file to the staging area.

```bash
git add .
```

Adds all changes in the current directory to the staging area.

### Commit changes

```bash
git commit -m "Commit message"
```

Saves the staged changes with a descriptive message.

### View commit history

```bash
git log
```

Displays the history of commits.

```bash
git log --oneline
```

Displays a compact commit history.

### View changes

```bash
git diff
```

Shows changes that have not yet been staged.

```bash
git diff --staged
```

Shows changes that are staged but not yet committed.

## 7. Working with Branches

Branches allow developers to work on different features independently.

### List branches

```bash
git branch
```

### Create a branch

```bash
git branch branch-name
```

### Switch branches

```bash
git switch branch-name
```

### Create and switch to a new branch

```bash
git switch -c branch-name
```

### Delete a merged branch

```bash
git branch -d branch-name
```

## 8. Merging Branches

To combine changes from another branch into the current branch:

```bash
git merge branch-name
```

Git attempts to combine the changes. Sometimes a merge conflict occurs when changes cannot be combined automatically.

## 9. Working with Remote Repositories

Remote repositories are versions of a project hosted on services such as GitHub.

### View remote repositories

```bash
git remote -v
```

### Add a remote repository

```bash
git remote add origin <repository-url>
```

### Upload commits

```bash
git push origin main
```

Uploads local commits to the remote repository.

### Download and integrate changes

```bash
git pull origin main
```

Fetches and integrates changes from the remote branch.

### Fetch changes

```bash
git fetch origin
```

Downloads remote changes without merging them into the current branch.

## 10. Undoing and Managing Changes

### Restore an unstaged file

```bash
git restore filename
```

Discards unstaged changes in the specified file. Use carefully because those changes may be lost.

### Unstage a file

```bash
git restore --staged filename
```

Removes a file from the staging area without deleting its working-directory changes.

### Revert a commit

```bash
git revert commit-id
```

Creates a new commit that reverses the changes introduced by an earlier commit.

### Remove a tracked file

```bash
git rm filename
```

Removes a file and stages its deletion.

### Rename or move a tracked file

```bash
git mv old-name new-name
```

Moves or renames a tracked file and stages the change.

## 11. Stashing Changes

Stashing temporarily stores changes that have not been committed.

```bash
git stash
```

Saves the current changes temporarily.

```bash
git stash list
```

Displays saved stashes.

```bash
git stash apply
```

Applies the most recent stash without removing it from the stash list.

```bash
git stash pop
```

Applies the most recent stash and removes it from the stash list.

## 12. Tags

Tags are used to mark important points in the repository's history, such as software releases.

```bash
git tag
```

Lists existing tags.

```bash
git tag v1.0
```

Creates a tag named v1.0.

```bash
git show v1.0
```

Displays information about the specified tag.

## 13. Other Useful Commands

| Command | Purpose |
|---|---|
| `git show` | Displays information about a commit or Git object. |
| `git help` | Displays help information. |
| `git status -s` | Shows a short status summary. |
| `git branch -a` | Lists local and remote branches. |
| `git remote show origin` | Displays information about a remote repository. |
| `git config --global --list` | Displays global Git configuration. |

## 14. The Basic Git Workflow

A typical Git workflow follows these steps:

1. Create or clone a repository.
2. Make changes to project files.
3. Check the status using `git status`.
4. Add changes using `git add`.
5. Commit changes using `git commit`.
6. Upload commits using `git push`.

### Workflow Commands

```bash
git status
git add .
git commit -m "Describe your changes"
git push
```

## 15. Advantages of Git

- Maintains a complete history of project changes.
- Supports teamwork and collaboration.
- Allows parallel development through branches.
- Helps recover previous versions.
- Supports distributed development.
- Is free and open-source.

## 16. Applications of Git

Git is commonly used in:

- Software development.
- Academic programming projects.
- Open-source projects.
- Collaborative development.
- Website development.
- Technical documentation.

## 17. Conclusion

Git is an important version control system that helps developers manage changes, maintain project history, and collaborate effectively. Understanding Git commands and workflows is useful for software development and technical documentation.