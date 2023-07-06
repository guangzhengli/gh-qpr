# How to use gh qpr to create a pull request with labels quickly

## Use

```bash
gh qpr
```

It will create a pull request with labels quickly to the origin/current-branch based on current branch.

It will create a new branch with rondom uuid name and push it to remote. then create a PR and auto merge. Finally, it will delete the local and origin branch, go back to the original branch and pull the latest code.

The default labels are empty. You can change it by setting the environment variable `gh_qpr_labels`.


## 1. Install the gh command

```bash
brew install gh
```

## 2. Login to GitHub with account

```bash
gh auth login
```

## 3. Download the gh-qpr extension

```bash
gh extension install guangzhengli/gh-qpr
```

## 4. Add the shell script environment to your path (Optional)

replace the `migration,need review` with your labels.

```bash
vim ~/.zshrc
```

```bash
export gh_qpr_labels="migration,need review"
```

```bash
source ~/.zshrc
```

## 5. How to use

```bash
gh qpr
```


