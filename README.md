# jordan
jordaninfo


delete all dev branches locally
git branch -D `git branch --list 'DEV*'`

Quickly delete all local branches that have been merged into master or develop already by adding this to your git config: 
alias cu = !git branch --merged | egrep -v \"(^\\*|master|develop)\" | xargs git branch -d
Then type "git cu" (Git Clean Up) and presto, all clean.
