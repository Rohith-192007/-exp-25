# Experiment: Creating a GitHub Repository and Pushing a README File

## Aim

To create a GitHub repository and push a `README.md` file from a local Git repository using Git commands.

## Software Requirements

- Git
- A GitHub account
- Terminal or command prompt
- Internet connection

## Introduction

Git is a distributed version control system used to track changes in source code. GitHub is a web-based platform that hosts Git repositories and supports collaboration, version control, and project management.

A `README.md` file describes a project and is displayed on the repository's main page.

## Procedure

### 1. Create a repository on GitHub

1. Sign in to [GitHub](https://github.com).
2. Select **New repository**.
3. Enter a repository name.
4. Choose Public or Private visibility.
5. Create the repository.

For this experiment, the repository is:

```text
https://github.com/Rohith-192007/-exp-25
```

### 2. Configure Git

Set your Git username and email address:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Use the name and email associated with your GitHub account where appropriate.

### 3. Create a local project folder

```bash
mkdir github-readme-experiment
cd github-readme-experiment
```

### 4. Initialize Git

```bash
git init
```

### 5. Create the README file

Create a file named `README.md` and add project information:

```markdown
# My First GitHub Repository

This repository demonstrates how to create a GitHub repository
and push a README file using Git.

## Tools Used
- Git
- GitHub
- Terminal
```

### 6. Stage and commit the file

```bash
git add README.md
git commit -m "Add README file"
```

### 7. Connect the local repository to GitHub

```bash
git branch -M main
git remote add origin https://github.com/Rohith-192007/-exp-25.git
```

### 8. Push the file to GitHub

```bash
git push -u origin main
```

If Git requests authentication, complete the sign-in flow using Git Credential Manager or a GitHub-supported authentication method. Do not put passwords or access tokens directly in commands or files.

## Common Git Commands

| Command | Purpose |
|---|---|
| `git init` | Initializes a local Git repository |
| `git status` | Displays the working-tree status |
| `git add README.md` | Stages the README file |
| `git commit -m "message"` | Saves staged changes as a commit |
| `git remote -v` | Displays configured remote repositories |
| `git push -u origin main` | Pushes the main branch to GitHub |
| `git log --oneline` | Displays recent commits |

## Result

A GitHub repository was created and a README file was prepared for version control. The local Git workflow stages and commits the README, connects the local repository to GitHub, and pushes the commit to the remote `main` branch.

**Verification:** After pushing, open the repository on GitHub and confirm that `README.md` appears on the repository page.

## Repository

[View the GitHub repository](https://github.com/Rohith-192007/-exp-25)
