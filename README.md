# Engineering Journal

### Description: Journal of engineering tips

## Node

*   Install latest node version
    *   nvm install node
*   Use latest node version
    *   nvm use node
*   List all node versions
    *   nvm list
*   Link to NVM doc
    *   [https://github.com/nvm-sh/nvm](https://github.com/nvm-sh/nvm)

## Git Commands

*   Rename branch
    *   git branch -m \<new branch name>
*   Delete local git repo
    *   rm -rf \<git repo name>.git
    *   rm -rf \<git repo name>
*   Cancel a git merge
    *   git-reset or git merge --abort
*   Reset to older commit in remote branch (dangerous if someone has pulled down changes in the commit you're deleting)
    *   git reset --hard \<commit-hash>
    *   git push -f origin \<branch-name>
*   Discard local uncommitted git changes
    *   git reset –hard
    *   git clean -fxd
*   Undo last local commit while leaving your working tree (the state of your files on disk) untouched
    *   git reset HEAD~
*   Delete all local branches besides "develop" or "master" etc.
    *   windows (powershell): git branch | %{ $_.Trim() } | ?{ $_ -ne 'master' } | ?{ $_ -ne 'main'} | ?{ $_ -ne 'develop'} | %{ git branch -D $_ }
    *   mac (terminal): git branch | grep -v "develop" | grep -v "master" | grep -v "main" | xargs git branch -D
*   Rollback to a previous commit and checkout into a branch
    *   git checkout < commithash > -b < branchname >
*   Commit and get past linting errors such as unused vars
    *   git commit -m "Commit Message" --no-verify
*   error: cannot lock ref
    *   git remote prune origin
    
## NPM

*   If you have npm install issues
    *   delete package-lock.json file and try npm i again
    *   try npm cache clean --force and then try npm i again
    *   delete node-modules folder and try npm i again
    *   try installing in a different terminal (e.g vscode terminal)
    *   restart terminal or restart compouter and try again

## Terminal (Unix) Commands

*   Basic UNIX Commands
    *   https://mally.stanford.edu/~sr/computing/basic-unix.html
*   To move a file from your Downloads folder to a Work folder in your Documents folder
    *   % mv ~/Downloads/MyFile.txt ~/Documents/Work/MyFile.txt
*   Something is already running on port 3000
    *   $ lsof -i tcp:3000
    *   $ kill -9 PID

## VS Code

*   Settings editor
    *   To open the Settings editor, navigate to Code > Settings > Settings. Alternately, open the Settings editor from the Command Palette (⇧⌘P) with Preferences: Open Settings or use the keyboard shortcut (⌘,).
*   Accept all incoming changes
    *   Press Ctrl+shift+p (command palette) or go to view and open command palette manually and type "merge" in your command palette, now you can see the Accept all incoming changes.
*   Open default settings
    *   Press F1, type in "open settings" go to Preferences: Open Default Settings (JSON)
*   Find and replace all occurrences of words in all files
    *   Press ctrl + shift + h
    *   Enter the word you want to replace on top input, and the word you want to replace to on the next input
    *   Click the button next to the second input to replace all of the occurrences
*   Find and replace all occurrences of words in one file
    *   Highlight some text and then press ctrl + shift + l
*   Format current file (e.g. with Prettier)
    *   alt + shift + f
*   Useful Keyboard Shortcuts
    *   https://semicolon.dev/tutorial/vscode/keyboard-shortcuts
*   Format code on save in VS Code
    *   Add the following to your settings.json file:
    *   "editor.formatOnSave": true

    
## Browser Debugger

*   Which DOM element has focus?
    *   In the console type in "document.activeElement"
    
## Variable Name Casing

*   Snake Case
    *   separates each word with an underscore character
    *   number_of_donuts = 34
*   Camel Case
    *   start by making the first word lowercase. Then, you capitalize the first letter of each word that follows
    *   numberOfDonuts = 34
*   Kebab Case
    *   separates each word with a dash character
    *   number-of-donuts = 34
*   Pascal Case
    *   like camel case but the first letter of the first word is also capitalized
    *   NumberOfDonuts = 34

