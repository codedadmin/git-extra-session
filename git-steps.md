# Git Steps

1. Clone a repository, or create a folder and do `git init`
2. Make a branch `git switch -c <feature-name>` or `git checkout -b <feature-name>`
3. Make some changes to your codebase
4. Stage your files to be committed `git add <file>...`
5. Commit your changes `git commit -m "Your nice message please"`
6. Push your changes to origin (i.e., remote repo) `git push`
   1. It will fail and tell you, your branch is unlinked, so do `git push -u origin <feature-name>`
7. Open a Pull Request on GitHub

## Merge conflicts

1. Run `git fetch`
2. Make sure you are in the branch that has an open PR and run `git merge origin/main`
3. Fix conflicts in VSCode like a pro (do not manually remove stuff, use Accept ...)
4. Stage the files that are resolved (using `git add <file>...`)
5. Commit your merge by running `git commit --no-edit`
6. Push your merge conflict resolution to GitHub (`git push`)

## Merge PR

1. Click on Merge PR and confirm
2. Delete remote branch
3. Switch to main branch locally and delete local branch by running `git branch -d <feature-name>`
4. Pull latest changes from remote main
