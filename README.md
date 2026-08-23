# Getting Started: Calc-Demo

A complete guide for absolute beginners to download the repository and push your first changes to GitHub.

---

## Windows Instructions

### What you'll need:
- A Windows laptop
- An internet connection
- A GitHub account (free at github.com)

---

### Step 1: Open PowerShell (Windows Terminal)

**What is PowerShell?** It's a program where you type commands to tell your computer what to do.

1. Click the **Windows Start button** (bottom left corner, the Windows logo)
2. In the search box that appears, type: `PowerShell`
3. You'll see "Windows PowerShell" appear in the results
4. Click on it
5. A dark blue window will open with white text — this is PowerShell

---

### Step 2: Navigate to your Documents folder

In PowerShell, type this command and press Enter:
```powershell
cd Documents
```

**What does this do?** It moves you to your Documents folder. You should see the text change to show you're in Documents.

---

### Step 3: Create a new folder called Demo

Type this command and press Enter:
```powershell
mkdir Demo
```

**What does this do?** It creates a new folder named "Demo" in your Documents folder.

Now type this command and press Enter:
```powershell
cd Demo
```

**What does this do?** It moves you INTO the Demo folder.

---

### Step 4: Download and Install Git

**What is Git?** It's software that helps you save and manage your code changes.

#### 4a. Download Git

1. Open your web browser (Chrome, Edge, or Firefox)
2. In the address bar at the top, type: `git-scm.com/download/win`
3. Press Enter
4. A download will start automatically
5. Wait for it to finish (it will download to your Downloads folder)

#### 4b. Find and run the Git installer

1. Click the **Windows Start button** (bottom left)
2. In the search box, type: `Downloads`
3. Click "Downloads" to open your Downloads folder
4. Look for a file that looks like: `Git-2.x.x-64-bit.exe` (the numbers might be different)
5. **Right-click** on it (press the right button on your mouse, not the left)
6. Click **"Run as administrator"**
7. A popup might appear asking "Do you want to allow this app?" — Click **"Yes"**

#### 4c. Install Git (follow the wizard)

1. A new window will open with the Git installer
2. You'll see many screens with options
3. For every screen, just click the **"Next >"** button
4. **Important screen:** When you see a screen that says "Adjusting your PATH environment", make sure the option **"Git from the command line and also from 3rd-party software"** is selected (it should be by default, with a circle next to it)
5. Keep clicking **"Next >"** until you see an **"Install"** button
6. Click **"Install"**
7. Wait for the installation to finish (about 1-2 minutes)
8. When you see **"Completing the Git Setup Wizard"**, click **"Finish"**
9. Close the installer window

#### 4d. Verify Git was installed

1. **Close PowerShell completely** — Click the X button
2. Open PowerShell again (click Windows Start, type PowerShell, click it)
3. Type this command and press Enter:
```powershell
git --version
```

**What should you see?**
- ✅ If you see: `git version 2.40.0` (or any version number) — Git is installed! Move to Step 5.
- ❌ If you see: `'git' is not recognized as the name of a cmdlet` — Git didn't install correctly. Try restarting your computer and running this command again.

---

### Step 5: Clone the repository (download the project)

**What does "clone" mean?** It means downloading a copy of the project from GitHub to your computer.

Make sure PowerShell is still showing you're in the Demo folder. Type this command and press Enter:
```powershell
git clone https://github.com/Zrokool/Calc-Demo.git
```

**What will happen?** You'll see text scrolling in PowerShell. Wait for it to finish.

Now move into the Calc-Demo folder:
```powershell
cd Calc-Demo
```

---

### Step 6: Create your first file

**What is VSCode?** It's a program for editing text files. It will open when you run this command.

Type this and press Enter:
```powershell
code vision.md
```

**What will happen?**
1. VSCode will open (it might take a few seconds)
2. You'll see an empty file ready for you to type in

**Write something in the file:**

Copy and paste this text (or write your own):
```
# My Vision

I am learning to use Git and GitHub.

## My goals:
- Understand version control
- Complete this project
- Learn to collaborate
```

**Save the file:**
1. Press **Ctrl + S** (hold Ctrl, press S)
2. You'll see the filename at the top stop having a dot next to it — that means it's saved

**Close VSCode:**
1. Click the **X button** in the top right corner of VSCode
2. You're back in PowerShell

---

### Step 7: Save your work to GitHub

#### 7a. Set up your Git identity (first time only)

This tells Git who you are. Type these commands:

```powershell
git config --global user.name "Your Full Name"
```

Replace `Your Full Name` with your actual name (example: `John Smith`)

Press Enter, then type:

```powershell
git config --global user.email "your.email@gmail.com"
```

Replace `your.email@gmail.com` with your actual email address.

Press Enter.

#### 7b. Create a GitHub personal access token (first time only)

**What is a token?** It's a special password that lets Git access your GitHub account.

1. Open your browser
2. Go to: `https://github.com/settings/tokens`
3. Sign in if needed
4. Click the blue button **"Generate new token"**
5. Click **"Generate new token (classic)"**
6. In the box labeled "Note", type: `Calc-Demo`
7. Scroll down and look for a box labeled **"repo"** — check it (click the checkbox)
8. Scroll down and click the green button **"Generate token"**
9. **A long code will appear** — this is your token
10. **Copy it** (Ctrl + C) and paste it into a text file so you don't lose it
11. ⚠️ **Important:** You'll only see this token once. If you leave this page without copying it, you have to generate a new one.

#### 7c. Upload your file to GitHub

Go back to PowerShell and type these commands one at a time, pressing Enter after each:

```powershell
git add vision.md
```

```powershell
git commit -m "Add my vision file"
```

```powershell
git push
```

**What will happen next?**

PowerShell will ask for your username and password:

```
Username for 'https://github.com': 
```

1. Type your **GitHub username** (the name you use to log in)
2. Press Enter
3. It will then ask:

```
Password for 'https://username@github.com':
```

4. Paste your **personal access token** (that long code you saved earlier)
5. Press Enter
6. The password won't show as you type — this is normal

**Wait for success message:**

You should see:
```
Enumerating objects: 3, done.
To https://github.com/Zrokool/Calc-Demo.git
   abc1234..def5678  main -> main
```

**🎉 Success!** Your file is now on GitHub!

---

## macOS Instructions

### What you'll need:
- A Mac laptop
- An internet connection
- A GitHub account (free at github.com)

---

### Step 1: Open Terminal (Mac's command tool)

**What is Terminal?** It's a program where you type commands to tell your Mac what to do.

1. Press **Cmd + Space** (Command key and Space bar at the same time)
2. A search box will appear at the top of your screen
3. Type: `Terminal`
4. You'll see "Terminal" appear in the results
5. Press Enter or click on it
6. A white window will open with text — this is Terminal

---

### Step 2: Navigate to your Documents folder

In Terminal, type this command and press Enter:
```bash
cd ~/Documents
```

**What does this do?** It moves you to your Documents folder.

---

### Step 3: Create a new folder called Demo

Type this command and press Enter:
```bash
mkdir Demo
```

**What does this do?** It creates a new folder named "Demo" in your Documents folder.

Now type this command and press Enter:
```bash
cd Demo
```

**What does this do?** It moves you INTO the Demo folder.

---

### Step 4: Download and Install Git

**What is Git?** It's software that helps you save and manage your code changes.

#### 4a. Download Git

1. Open your web browser (Safari, Chrome, or Firefox)
2. In the address bar at the top, type: `git-scm.com/download/mac`
3. Press Enter
4. A download will start automatically
5. Wait for it to finish

#### 4b. Find and run the Git installer

1. Open **Finder** (the blue smiley face icon in your dock at the bottom)
2. Click **"Downloads"** in the left sidebar
3. Look for a file that looks like: `git-2.x.x-intel-universal2.dmg` (the numbers might be different)
4. **Double-click** it (press the left mouse button twice quickly)
5. A new window will open showing the Git installer

#### 4c. Install Git

1. In the new window, you'll see a Git icon
2. **Double-click** the Git icon (it usually says "Git Installer" or has a package symbol)
3. A popup will appear asking for your **Mac password** — type it
4. Click **"Install Software"**
5. Wait for installation to finish (about 1-2 minutes)
6. You'll see a message: **"The install was successful"**
7. Click **"Close"**
8. Close all the installer windows

#### 4d. Verify Git was installed

1. **Close Terminal completely** — Click the red button in the top left corner
2. Open Terminal again (Cmd + Space, type Terminal, press Enter)
3. Type this command and press Enter:
```bash
git --version
```

**What should you see?**
- ✅ If you see: `git version 2.40.0` (or any version number) — Git is installed! Move to Step 5.
- ❌ If you see: `command not found: git` — Git didn't install correctly. Try restarting your Mac and running this command again.

---

### Step 5: Clone the repository (download the project)

**What does "clone" mean?** It means downloading a copy of the project from GitHub to your computer.

Make sure Terminal is still showing you're in the Demo folder. Type this command and press Enter:
```bash
git clone https://github.com/Zrokool/Calc-Demo.git
```

**What will happen?** You'll see text scrolling in Terminal. Wait for it to finish.

Now move into the Calc-Demo folder:
```bash
cd Calc-Demo
```

---

### Step 6: Create your first file

**What is VSCode?** It's a program for editing text files. It will open when you run this command.

Type this and press Enter:
```bash
code vision.md
```

**What will happen?**
1. VSCode will open (it might take a few seconds)
2. You'll see an empty file ready for you to type in

**Write something in the file:**

Copy and paste this text (or write your own):
```
# My Vision

I am learning to use Git and GitHub.

## My goals:
- Understand version control
- Complete this project
- Learn to collaborate
```

**Save the file:**
1. Press **Cmd + S** (Command key and S at the same time)
2. You'll see the filename at the top stop having a dot next to it — that means it's saved

**Close VSCode:**
1. Click the red button in the top left corner of VSCode
2. You're back in Terminal

---

### Step 7: Save your work to GitHub

#### 7a. Set up your Git identity (first time only)

This tells Git who you are. Type these commands:

```bash
git config --global user.name "Your Full Name"
```

Replace `Your Full Name` with your actual name (example: `Jane Smith`)

Press Enter, then type:

```bash
git config --global user.email "your.email@gmail.com"
```

Replace `your.email@gmail.com` with your actual email address.

Press Enter.

#### 7b. Create a GitHub personal access token (first time only)

**What is a token?** It's a special password that lets Git access your GitHub account.

1. Open your browser
2. Go to: `https://github.com/settings/tokens`
3. Sign in if needed
4. Click the blue button **"Generate new token"**
5. Click **"Generate new token (classic)"**
6. In the box labeled "Note", type: `Calc-Demo`
7. Scroll down and look for a box labeled **"repo"** — check it (click the checkbox)
8. Scroll down and click the green button **"Generate token"**
9. **A long code will appear** — this is your token
10. **Copy it** (Cmd + C) and paste it into a text file so you don't lose it
11. ⚠️ **Important:** You'll only see this token once. If you leave this page without copying it, you have to generate a new one.

#### 7c. Upload your file to GitHub

Go back to Terminal and type these commands one at a time, pressing Enter after each:

```bash
git add vision.md
```

```bash
git commit -m "Add my vision file"
```

```bash
git push
```

**What will happen next?**

Terminal will ask for your username and password:

```
Username for 'https://github.com': 
```

1. Type your **GitHub username** (the name you use to log in)
2. Press Enter
3. It will then ask:

```
Password for 'https://username@github.com':
```

4. Paste your **personal access token** (that long code you saved earlier)
5. Press Enter
6. The password won't show as you type — this is normal

**Wait for success message:**

You should see:
```
Enumerating objects: 3, done.
To https://github.com/Zrokool/Calc-Demo.git
   abc1234..def5678  main -> main
```

**🎉 Success!** Your file is now on GitHub!

---

## Quick Reference: Upload changes later

After your first time, here's the quick way to upload changes:

```
git add filename.txt
git commit -m "What you changed"
git push
```

That's it!

---

## Troubleshooting

**"Git is not recognized" (Windows)**
- Close PowerShell
- Restart your computer
- Open PowerShell again
- Try `git --version`

**"command not found: git" (Mac)**
- Close Terminal
- Restart your Mac
- Open Terminal again
- Try `git --version`

**"Authentication failed" when pushing**
- Make sure your token is correct
- Check you copied the entire token (it's long)
- Generate a new token at: https://github.com/settings/tokens

**"fatal: 'origin' does not appear to be a git repository"**
- Make sure you're in the Calc-Demo folder
- Check by typing `pwd` and pressing Enter
- You should see a path ending in `/Calc-Demo`
