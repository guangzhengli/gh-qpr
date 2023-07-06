# How to use gh qpr to create a pull request with labels quickly

## Why create this extension

Recently, I had a requirement to use Git to submit a PR to the remote branch with the same name on GitHub, and also add some labels to the PR.

I needed to manually create a new branch, create a PR, add tags, merge the PR, delete temporary branches, return to the original branch and pull code. It was too cumbersome. So I created this extension to simplify the process.

## Use

```bash
gh qpr
```

First, it will create a new branch with rondom uuid name and push it to remote. 

Then create a PR with labels and auto merge. 

Finally, it will delete the local and origin temporary branch, go back to the original branch and pull the latest code.

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


