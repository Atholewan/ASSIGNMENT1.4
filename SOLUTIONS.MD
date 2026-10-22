

The assignment requires a real Git repository and screenshots of its folder and commit history. I can prepare the project content for you, but the Git commands must be run in a Git environment to produce genuine commit history.

## Run this script to create the complete assignment

If you're using Windows, this PowerShell script will create the project folder, initialize Git, add the HTML and README files, and make all three commits automatically.

### 1. Install Git first

git --version
```
# Assignment 1.4 - Git Essentials I

# Ask for your Git identity
$gitName = Read-Host "Enter your name"
$gitEmail = Read-Host "Enter your email"




# Configure Git for this project only
git init


git config user.name $gitName
git config user.email $gitEmail

# Commit 1: Create the HTML page
@'

'@ | Set-Content -Encoding utf8 index.html

git add index.html
git commit -m "Initial commit: add HTML page"


# Commit 2: Update the HTML page
   '

git add index.html
git commit -m "Update page with learning goals"


# Commit 3: Add project documentation
@'
# My First Git Project

This project demonstrates basic Git operations.

## Technologies
- HTML
- Git

## Learning Goals
- Initialize a repository
- Track file changes
- Create commits
'@ | Set-Content -Encoding utf8 README.md

git add README.md
git commit -m "Add project README documentation"
if ($LASTEXITCODE -ne 0) { throw "Third commit failed." }

# Display final results
Write-Host "`n--- COMMIT HISTORY ---" -ForegroundColor Cyan
git log --oneline

Write-Host "`n--- REPOSITORY STATUS ---" -ForegroundColor Cyan
git status

Write-Host "`n--- PROJECT LOCATION ---" -ForegroundColor Green
Get-Location

Write-Host "`nAssignment project created. Capture your screenshots now."
```

### 3. Capture your submission screenshots

After the script finishes, take these two screenshots:

Cloning an Azure Repo into GitHub Desktop with Single Click 🖱 | by Upendra Venkata Muralidhar Thunuguntla | Medium

Screenshot 1: Project folder

Open `Assignment-1.4` in File Explorer. Show `index.html`, `README.md`, and the `.git` folder if hidden files are enabled.

Pretty PowerShell with Windows Terminal, posh-git, and oh-my-posh | HynekS

Screenshot 2: Git commit history

Show the terminal with all three commits and the output of `git status`.

Your commit history should contain:

- `Initial commit: add HTML page`
- `Update page with learning goals`
- `Add project README documentation`

Your final repository should report `nothing to commit, working tree clean`.

One important note: I haven't run this script on your computer, so the repository and screenshots still need to be generated on your machine. Once you run it, the project files and the three real commits will be created automatically.