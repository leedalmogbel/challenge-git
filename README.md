# Git Challenge
There are two branches, `add-echo` and `add-reverse`. The goal of this challenge is to use `git rebase` to bring both commits onto master. When finished there should be no merge commits or branching. For example, `git log` on the `master` branch should look similar to this:
```
/challenge-git master
⚡ git log
61a2c67 feat: add reverse route (David Guttman, 7 minutes ago)
2c2c5d6 feat: add echo route (David Guttman, 10 minutes ago)
dcc4c0b docs: add more instructions (David Guttman, 11 minutes ago)
...
```
## Instructions
How to attempt this challenge:
1) Create a new repo in your account and note the git url
2) Clone this repo
3) Solve the challenge
4) Set your new repo as the origin: `git remote set-url origin ${your repo url}`
5) Push your solution to your repo
You must follow these steps for your solution to be accepted -- forks or other methods will not be considered.

## Solutions
git clone
cd repo
git pull
git checkout add-echo
git rebase master
git checkout master
git rebase add-echo
git checkout add-reverse
git rebase master
*conflicts will show
git mergetool
*fix all the conflicts)
git rebase --continue
git checkout master
git rebase add-reverse
git log
