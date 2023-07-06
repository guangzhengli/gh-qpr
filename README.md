# How to use gh qpr to create a pull request with labels quickly

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


