Git Setup & Foundations Lab

Welcome to your first hands-on lab for Git Made Easy! 
In this lab, you’ll get familiar with Git, set up your environment, and connect to GitHub (or GitLab).

Lab Steps

Step 1 — Create a Repository on GitHub (or GitLab)
  - Log in to GitHub (or GitLab).
  - Create a new repository named hello-git.
    - Keep it empty (no README, no .gitignore).
  - Copy the HTTPS URL of your new repo — you’ll need it later.
    - Example: https://github.com/<your-username>/hello-git.git
  This lab uses HTTPS for authentication. The first time you push, Git will prompt for credentials. Use your username and a Personal Access Token (PAT) (not your password).
  - GitHub PAT setup guide: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token

Step 2 — Use the Git CLI to Explore Available Commands
  git help
  git help -a #Type q to exit help

Step 3 — Validate Git Installation on Your Machine
  git --version
  which git     # macOS/Linux
  # or
  where git     # Windows

Step 4 — Configure Global Git Settings for Your Identity and Defaults
  git config --global user.name "Your Name"
  git config --global user.email "you@example.com"
  git config --global init.defaultBranch main
  git config --global color.ui auto
  git config --global -l

Step 5 — Modify the Provided File, Initialize a Repo, and Make Your First Commit
  In the hello-git directory, open the provided file hello-git.txt in your editor.
  Add a new line of text (for example: This is my first Git change!).
  Save the file, then run the following commands:
    git init
    git status
    git add hello-git.txt
    git commit -m "Initial commit with hello-git.txt"
    git log --oneline
  Run a git status after the command to see how the state changes.

Step 6 — Connect Your Local Repo to GitHub (HTTPS) and Push
  Replace <your-username> with your GitHub username:
    git remote add origin https://github.com/<your-username>/hello-git.git
    git branch -M main
    git push -u origin main
  When prompted, authenticate with your username and Personal Access Token (PAT).

By the End

You’ll have:

  - A fully configured Git environment
  - A local repository with a committed file
  - Your code pushed and visible on GitHub (or GitLab)

This repo will be the foundation for later labs, where you’ll branch, merge, and collaborate.