#Useful Terminal Commands

### File location

- <b>ls</b>: lists contents in directory
- <b>ls -a</b>: contents + hidden files
- <b>pwd</b>: print working directory
- <b>application -v</b>: show version of the application installed


### Moving around
- <b>cd</b>: change directory
  - typing cd by itself will take you back to root
  - <b>..</b> : go up one folder
- <b>cp filename newFilename</b>
  - will copy filename in the directory to newFilename. You can also specify a different direction for newFilename ../Folder/newFilename
  - <b>cp -r directory newDirectory</b>: copy entire directories
- <b>mkdir folderName</b>: make directory
- <b>mv oldFile newFile</b>: like cp, but will delete oldFile. Works on files and directories
- <b>rm</b>: remove file
  - <b>rm -rf</b>: remove folder
- <b>touch fileName</b>: create file
- <b>vim fileName</b>: create and write file
  - <b>i</b>: insert mode
  - <b>esc, then :wq</b> to write and quit

### Useful Node commands
- <b>npm i -D libraryName</b>: -i = install, -D = Developer dependency
  - ex. eslint babel babel-preset-es2015 is a developer dependency; you use it during development but not during production
  - <b>npm i -S libraryName</b>: install as a regular dependency, used in both development and production
    - ex. lodash is used by the developer and user
    
### Git Basics
#### Creating a Repo
1. Create new project folder and add a file. CD into the folder.
  - <b>git init</b>
  - <b>git add file</b>
    - if a file is altered, add the file so that the status is updated. status will show that the file was updated
    - <b>git add .</b>: add all files in directory
  - <b>git commit -m "Commit comment"</b>: create first commit
    - m tag allows comment
2. Check status: <b>git status</b>
3. View log: <b>git log</b>
  - <b>git log --pretty=oneline</b> to view one line updates
  - <b>git log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short</b>: a good log format
