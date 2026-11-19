# Experiment 2: Cloning a GitHub Repository and Editing Files Locally

## Aim

To clone an existing GitHub repository to a local computer, edit a file, save the changes using Git, and push the updated file back to GitHub.

## Requirements

- Git installed on the computer
- A GitHub account with access to the repository
- Terminal or command prompt
- Internet connection

## Repository

```text
https://github.com/Rohith-192007/-exp-25
```

## Procedure

### 1. Open the terminal

Open Terminal on macOS, or Git Bash / Command Prompt on Windows.

### 2. Clone the repository

Move to the folder where you want to keep your project, then run:

```bash
git clone https://github.com/Rohith-192007/-exp-25.git
```

This downloads the repository and its commit history to your computer.

### 3. Enter the cloned folder

```bash
cd -exp-25
```

### 4. Check the repository status

```bash
git status
```

This displays the current branch and whether any files have been changed.

### 5. Edit a file locally

Open `README.md` in a text editor such as VS Code:

```bash
code README.md
```

Add the following section at the end of the file, then save it:

```markdown
## Local Editing Test

This section was added after cloning the repository.
The changes were made locally and are ready to be committed.
```

If the `code` command is not available, open the cloned folder manually in VS Code and edit `README.md`.

### 6. Review the changes

```bash
git status
git diff
```

- `git status` shows which files have changed.
- `git diff` displays the exact lines added, modified, or removed.

### 7. Stage the edited file

```bash
git add README.md
```

### 8. Commit the changes

```bash
git commit -m "Update README after local cloning"
```

A commit records the changes in the local Git repository.

### 9. Push the changes to GitHub

```bash
git push origin main
```

If GitHub requests authentication, complete its sign-in flow. Do not share your password or access token.

### 10. Verify the update

Refresh the GitHub repository page and confirm that the new **Local Editing Test** section appears in `README.md`.

## Important Git Commands

| Command | Description |
|---|---|
| `git clone URL` | Downloads a remote repository |
| `cd -exp-25` | Opens the cloned project folder |
| `git status` | Checks the working-tree status |
| `git diff` | Shows local file changes |
| `git add README.md` | Stages the edited file |
| `git commit -m "message"` | Records the staged changes |
| `git push origin main` | Uploads commits to GitHub |
| `git pull origin main` | Downloads and integrates remote changes |

## Result

The GitHub repository can be cloned to a local computer. After editing and saving a file, Git tracks the changes, stages them, and records them in a commit. The commit can then be pushed to GitHub and verified on the repository page.
