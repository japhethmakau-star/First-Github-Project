# **Installing Git on Windows (with Command Prompt & PowerShell Access)**

## **Step 1 — Download Git**

1. Open your browser and go to:
   🔗 [https://git-scm.com/download/win](https://git-scm.com/download/win)
2. The **64-bit Git for Windows** installer should download automatically.
3. Save the file to your Downloads folder.

---

## **Step 2 — Run the Installer**

1. **Double-click** the `.exe` file you downloaded.
2. In the setup wizard:

   * **"Select Components"** → Leave everything checked (optional: enable “Windows Explorer integration” for right-click Git options).
   * **"Adjusting your PATH environment"** → Select:
     ✅ **Git from the command line and also from 3rd-party software**
     *(This is important so Git works in Command Prompt and PowerShell.)*
3. Click **Next** through the other options (leave defaults if unsure).
4. Click **Finish** when done.

---

## **Step 3 — Verify Installation**

Open **Command Prompt** or **PowerShell** and type:

```powershell
git --version
```

Expected output:

```
git version 2.xx.x.windows.x
```

If you see the version number, Git is installed and ready.

---

## **Step 4 — Configure Git (First Time Only)**

Run the following commands in **Command Prompt** or **PowerShell**, replacing with your own name and email:

```powershell
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Check that it saved:

```powershell
git config --list
```

---

## **Step 5 — Create a New Repository**

1. Create a folder for your project:

```powershell
mkdir myproject
cd myproject
```

2. Initialize Git in this folder:

```powershell
git init
```

3. Create a `.gitignore` file (optional but recommended):

```powershell
echo # Ignore files > .gitignore
```

4. Add and commit files:

```powershell
git add .
git commit -m "Initial commit"
```

---

## **Step 6 — (Optional) Connect to GitHub**

If you have a GitHub account:

1. Create a new empty repository on GitHub.
2. In your terminal:

```powershell
git remote add origin https://github.com/username/repo-name.git
git branch -M main
git push -u origin main
```

---

✅ **Now Git is ready on Windows** — and you can run `git` commands in **Command Prompt**, **PowerShell**, or **Git Bash** without issues.


