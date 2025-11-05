# testtt


## 1. Configure Git Identity

Set your username and email — this links your commits to your GitHub account.

```bash
git config --global user.name "Your Name"
git config --global user.email yourname@example.com
```

>
> ```bash
> git config --global user.email 123456789+username@users.noreply.github.com
> ```

---

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

---

## 3. Create an SSH Key (for GitHub Authentication)

### 3.1 Check for Existing Key

```bash
ls ~/.ssh/id_ed25519.pub
```

If you see “No such file or directory”, continue to create one.

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

## 5. Test SSH Connection

Run:

```bash
ssh -T git@github.com
```

Expected output:

```
Hi username! You’ve successfully authenticated, but GitHub does not provide shell access.
```



```bash
git init
```

---
