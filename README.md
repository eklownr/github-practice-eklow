# github-practice-eklow
## Set up new repo:

```bash
mkdir <your-repo-name>
cd <your-repo-name>
git intt
git remote add origin https://github.com/<your-github>/<your-repo-name>.git
echo > "your-repo-message" README.md
git add .
git commit -m "first commit"
git push --set-upstream origin main
```
## Fix header
```bash
git checkout -b fix-header
vim README.md # update/fix README
git checkout origin/main
git pull
```
## Clean up branches 
```bash
git checkout main
git branch -d fix-header # remove local
git push origin --delete fix-header # remove from github
```

