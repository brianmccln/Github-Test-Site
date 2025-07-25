# 🛠️ chmod +x and Running Shell Scripts Cheat Sheet

## ✅ What is `chmod`?

`chmod` means **"change mode"** — it's used to change the **permissions** on a file.

### 🔒 Problem:
When you create a `.sh` file (like `update.sh`), it **might not be executable** by default.

### ⚡ Solution:
Use `chmod` to add **execute permission**.

---

## 🚀 Make a Script Executable

```bash
chmod +x update.sh
---

## 🚀 Make a Script Executable and Run It

### 1. Create a shell script

Save the following in a file called `update.sh`:

```bash
#!/bin/bash
git add .
git commit -m "update stuff"
git push

# So, Mac vs. Windows:
# Mac:
chmod +x update.sh
./update.sh

# Windows
update.bat
# that failing, try:
call update.bat
```