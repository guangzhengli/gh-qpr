# How to use gh qpr to create a pull request with labels quickly

## Use

```bash
gh qpr
```

It will create a pull request with labels quickly to the origin/current-branch based on current branch.

The default labels are empty. You can change it by setting the environment variable `gh_qpr_labels`.

It will create a new rondom branch and push it to remote. then create a pr and delete the local and origin branch. Finally, it will go back to the original branch.

## 1. Install the gh command

```bash
brew install gh
```

## 2. Login to GitHub with tw account

```bash
gh auth login
```

## 3. Add the shell script environment to your path (Optional)


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


