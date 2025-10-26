# 🧭 Git Installation Guide (macOS & Windows)

## 📘 Introduction

**Git** is a distributed version control system that helps developers manage, track, and collaborate on code efficiently.
This guide explains how to install Git on **macOS** and **Windows** using the most reliable methods.

---

## 🍎 macOS Installation (via Homebrew)

### Step 1: Install Homebrew

[Homebrew](https://brew.sh) is a package manager for macOS that makes software installation simple.

Open **Terminal** and run the following command to install Homebrew:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Once the installation completes, configure your shell environment (if prompted):

```bash
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

Verify that Homebrew is installed:

```bash
brew --version
```

---

### Step 2: Install Git using Homebrew

Use Homebrew to install Git:

```bash
brew install git
```

---

### Step 3: Verify Git Installation

After installation, confirm Git is working:

```bash
git --version
```

Expected output:

```
git version 2.xx.x
```

---

### Step 4: Configure Git (Recommended)

Set up your Git username and email (used in commits):

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Verify configuration:

```bash
git config --list
```

---

## 🪟 Windows Installation (via Git for Windows)

### Step 1: Download the Installer

Go to the official Git website:
👉 [https://git-scm.com/download/win](https://git-scm.com/download/win)

The installer will automatically download.

---

### Step 2: Run the Installer

1. Open the downloaded `.exe` file.
2. Follow the setup wizard and **keep the default settings** unless you have specific preferences.
3. Click **Finish** when the installation completes.

---

### Step 3: Open Git Bash

After installation, open **Git Bash** (not Command Prompt).
You can find it by searching for **“Git Bash”** in the Start Menu.

---

### Step 4: Verify Git Installation

In **Git Bash**, run:

```bash
git --version
```

Expected output:

```
git version 2.xx.x.windows.x
```

---

### Step 5: Configure Git

In **Git Bash**, set up your Git identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Check configuration:

```bash
git config --list
```

---

## 🧪 Quick Verification (Both macOS & Windows)

To ensure Git works correctly, create and initialize a test repository:

```bash
mkdir test-repo
cd test-repo
git init
```

If you see:

```
Initialized empty Git repository in ...
```

🎉 Git is successfully installed and ready to use!
