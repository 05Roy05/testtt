# testtt


## 1. Configure Git Identity

Set your username and email — this links your commits to your GitHub account.

```bash
git config --global user.name "Your Name"
git config --global user.email yourname@example.com

>
> ```bash
> git config --global user.email 123456789+username@users.noreply.github.com


## 2. Set Default Branch & Pull Behavior

Change default branch name from `master` → `main`:

```bash
git config --global init.defaultBranch main
```

Set default pull behavior (recommended):

```bash
git config --global pull.rebase false
```

Verify settings:

```bash
git config --get user.name
git config --get user.email
```




```bash
ls ~/.ssh/id_ed25519.pub


### 3.2 Generate a New SSH Key

```bash
ssh-keygen -t ed25519
```


### 3.3 Copy Your Public Key

```bash
cat ~/.ssh/id_ed25519.pub
```

Copy the full output — it starts with `ssh-ed25519` and ends with your username.

---

## 4. Add SSH Key to GitHub

1. Go to **GitHub → Settings → SSH and GPG Keys**
2. Click **New SSH Key**
3. Enter a title (e.g., `ubuntu-laptop` or `macbook`)
4. Paste your key
5. Click **Add SSH Key**

---


ssh -T git@github.com
```




```bash
git init
```

---
