
### 1. Install Git first and verification

git --version
```
c:\Users\HomePC\Pictures\Screenshots\GIT VERSION.png

# Open terminal in the project folder
Write-Host "`n--- PROJECT LOCATION ---" -ForegroundColor Green
Get-Location

c:\Users\HomePC\Pictures\Screenshots\project location.png

# Configure Git for this project only
git init
c:\Users\HomePC\Pictures\Screenshots\git init.png

#INITIALIZATION COMMANDS
git config user.name $gitName
git config user.email $gitEmail
c:\Users\HomePC\Pictures\Screenshots\git name,email init.png

###git status
Write-Host "`n--- REPOSITORY STATUS ---" -ForegroundColor Cyan
git status
c:\Users\HomePC\Pictures\Screenshots\git status.png

#git add and git commit
c:\Users\HomePC\Pictures\Screenshots\git add,commit.png

#GIT COMMIT HISTORY
Write-Host "`n--- COMMIT HISTORY ---" -ForegroundColor Cyan
git log --oneline
c:\Users\HomePC\Pictures\Screenshots\commit history.png

 #PICTURE OF PROJECT FOLDER
 c:\Users\HomePC\Pictures\Screenshots\PROJECT FOLDER.png



