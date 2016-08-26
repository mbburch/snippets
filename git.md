# Git Snippets

* git fetch -p: git fetch prune removes remote tracking references that no longer exist on remote
* git branch -a: shows both local and remote branches
* git branch -r: shows remote branches

## From Penney's Gist

Haught git flow with interactive rebasing and squashing:<br>
- switch to master, pull down, then check out your branch
- <code>git rebase master</code>
- fix any conflicts, then <code> git add .</code> and <code>git rebase --continue</code>
- <code>git rebase -i <sha just before your 1st commit></code>
- do the squashing!
- <code>git push origin [branch name] -f</code>
- don't switch to master and merge --> merge on Github via the PR
- viola!

Merge in master from your branch:<br>
- <code>git stash</code>
- <code>git rebase master</code>
- <code>git push -f</code>
- <code>git stash pop</code>

Example of how to set/change the upstream:<br>
<code>git remote set-url origin https://github.com/HaughtCodeworks/cfp-app.git</code>

Some helpful git commands from Marty:<br>
<code>git config --global apply.whitespace nowarn</code> ignore whitespace differences<br>
<code>git config --global core.excludesfile ~/.gitignore</code><br>
<code>git config --global push.default tracking</code><br>
<code>git config --global branch.autosetuprebase always</code> default to rebase instead of merge on a <code>git pull</code>

Set a remote:<br>
<code>git remote add remote-name remote-url</code><br><br>
Example: <code>git remote add staging https://git.heroku.com/cfp-next-staging.git</code><br>
Do a <code>git fetch</code> after

git blame - to see who did what in the terminal:<br>
<code>git blame [file path]</code>

<code>git fetch</code> vs. <code>git pull</code><br>
<code>fetch</code> is safe and simply makes the local aware of changes<br>
<code>pull</code> will try to merge or rebase (depending on what you have your local set to do)

Reset a file to its state before changes / the same state as if you just pulled from master (great for schema issues on master)
<code>git checkout db/schema.rb</code>