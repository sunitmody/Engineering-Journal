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
 

## Terminal (Unix) Commands

*   Basic UNIX Commands
    *   https://mally.stanford.edu/~sr/computing/basic-unix.html
*   To move a file from your Downloads folder to a Work folder in your Documents folder
    *   % mv ~/Downloads/MyFile.txt ~/Documents/Work/MyFile.txt

## VS Code

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
