# Create Your First GitHub Repository

A beginner-friendly guide using VSCode to create your first repository.

---

## FIRST: Create a GitHub Account

You need a GitHub account before you can upload your code. This is free and takes 5 minutes.

### Step 1: Go to GitHub

1. Open your browser (Chrome, Safari, Firefox, or Edge)
2. In the address bar, type: `github.com`
3. Press Enter

### Step 2: Click "Sign up"

You'll see the GitHub homepage. Click the green **Sign up** button (top right corner).

### Step 3: Enter your email

1. Type your email address in the box
2. Click the green **Continue** button

### Step 4: Create a password

1. Create a password (at least 15 characters, mix of letters, numbers, and symbols)
2. Type it in the box
3. Click **Continue**

### Step 5: Choose your username

1. Enter a username (this is what people will see, example: `JohnSmith42`)
2. GitHub will tell you if it's available
3. Click **Continue**

### Step 6: Email verification

1. GitHub will send you a verification code to your email
2. Check your email inbox
3. Copy the code GitHub sent you
4. Paste it into the box on the GitHub page
5. Click **Continue**

### Step 7: Answer a question

1. GitHub asks "How many team members will be using GitHub?"
2. Select: **Just me**
3. Click **Continue**

### Step 8: Finish setup

1. Click **Create account**
2. You're done! You now have a GitHub account.

---

**Keep your username and password safe. You'll need them later!**

---

## SECOND: Install VSCode

VSCode is the program you'll use to create files and commit your code. It's free and easy to install.

### Windows

1. Open your browser
2. In the address bar, type: `code.visualstudio.com`
3. Press Enter
4. Click the blue **Download for Windows** button
5. Wait for the download to finish
6. Open your Downloads folder
7. Double-click `VSCodeUserSetup-x64-x.xx.x.exe`
8. Click **I accept the agreement**
9. Click **Next**
10. Keep clicking **Next** until you see **Install**
11. Click **Install**
12. Click **Finish**
13. VSCode will open automatically

### macOS

1. Open your browser
2. In the address bar, type: `code.visualstudio.com`
3. Press Enter
4. Click the **Download for Mac** button
5. Wait for the download to finish
6. Open Finder and go to Downloads
7. Double-click `VSCode-darwin-universal.zip`
8. Drag the **Visual Studio Code** app to your Applications folder
9. Open Applications folder
10. Double-click **Visual Studio Code**
11. VSCode will open

---

---

## Install Git

Git needs to be installed on your computer before you start. It runs in the background.

### Windows

1. Open your browser and go to: `git-scm.com/download/win`
2. The download starts automatically
3. Open your Downloads folder and double-click the `Git-2.x.x-64-bit.exe` file
4. Click **Next** on every screen
5. When you see "Adjusting your PATH environment", make sure `Git from the command line and also from 3rd-party software` is selected
6. Keep clicking **Next** until you see **Install**, then click it
7. Click **Finish**
8. Restart your computer

### macOS

1. Open your browser and go to: `git-scm.com/download/mac`
2. The download starts automatically
3. Open Finder, go to Downloads
4. Double-click the `.dmg` file
5. Double-click the Git installer icon
6. Enter your Mac password
7. Click **Install Software**
8. Wait for it to finish and click **Close**
9. Restart your computer

---

## OPTIONAL: Install GitHub Extension for VSCode

This extension makes it easier to manage your repositories directly in VSCode. It's helpful but not required.

### Windows & macOS

1. Open **VSCode**
2. Click the **Extensions** icon on the left sidebar (looks like four small squares)
3. In the search box, type: `GitHub`
4. Find **"GitHub"** by GitHub (the official one)
5. Click **Install**

You now have GitHub integration in VSCode! This lets you manage your repositories more easily from within VSCode.

---

---

# Create Your First Repository

---

## Step 1: Create a folder on your computer

### Windows

1. Click **File Explorer** (or press `Win + E`)
2. Click **Documents** in the left sidebar
3. Right-click in the empty space
4. Click **New** → **Folder**
5. Name it: `MyFirstProject`

### macOS

1. Open **Finder**
2. Click **Documents** in the left sidebar
3. Right-click in the empty space
4. Click **New Folder**
5. Name it: `MyFirstProject`

---

## Step 2: Open the folder in VSCode

### Windows & macOS

1. Open **VSCode**
2. Click **File** → **Open Folder**
3. Find and select your `MyFirstProject` folder
4. Click **Open**
5. Click **Yes, I trust the authors** (if it asks)

---

## Step 3: Create your first file

1. In VSCode, look at the left sidebar
2. Hover over the folder name and click the **New File** icon (looks like a sheet of paper with a +)
3. Name it: `README.md`
4. Press Enter

A new file opens. Type this:

```
# My First Project

Hello! This is my first GitHub repository.

## What I'm learning:
- How to use Git
- How to commit changes
- How to push to GitHub
```

**Save the file:**
- Press **Ctrl + S** (Windows) or **Cmd + S** (macOS)

---

## Step 4: Commit your changes in VSCode

Now you'll save your work using Git.

### Option A: Use VSCode UI (Easiest)

#### 4a. Open the Source Control panel

1. On the left sidebar, click the **Source Control** icon (looks like three dots connected)
2. You'll see a section that says "Source Control"

#### 4b. Initialize Git

1. Click the blue button that says **Initialize Repository**
2. Select your `MyFirstProject` folder (it should already be selected)
3. Click **Initialize Repository**

You'll now see your file listed under "Changes".

#### 4c. Stage your file

1. You should see `README.md` listed under "Changes"
2. Click the **+** button next to `README.md`
3. It will move to a section called "Staged Changes"

#### 4d. Commit

1. In the message box at the top (where it says "Message"), type: `Add README file`
2. Click the blue **Commit** button
3. Done! Your file is now committed locally.

---

### Option B: Use Terminal Commands

If you prefer using the terminal, here are the Git commands that do the same thing:

#### 4a. Open Terminal in VSCode

Press **Ctrl + `** (Windows) or **Cmd + `** (macOS) to open the terminal at the bottom of VSCode.

#### 4b. Initialize Git

Type this command and press Enter:
```
git init
```

This tells Git to start tracking changes in your folder.

#### 4c. Stage your file

Type this command and press Enter:
```
git add .
```

**What does this do?** The `.` means "add all files". This prepares your files to be committed.

#### 4d. Commit your changes

Type this command and press Enter:
```
git commit -m "Add README file"
```

**What does this do?** This creates a snapshot of your work. The `-m` means "message", and `"Add README file"` is the description of what you changed.

**You should see:**
```
[main (root-commit) abc1234] Add README file
 1 file changed, 5 insertions(+)
 create mode 100644 README.md
```

---

**Use whichever option feels more comfortable to you. Both do the same thing.**

---

## Step 5: Create a repository on GitHub.com

1. Open your browser
2. Go to: `https://github.com/new`
3. In the **Repository name** box, type: `MyFirstProject`
4. Leave everything else as default
5. Scroll down and click **Create repository**
6. **Copy the URL** from the line that says `https://github.com/YourUsername/MyFirstProject.git`
7. Keep this page open

---

## Step 6: Connect your folder to GitHub in VSCode

### 6a. Add the remote connection

1. Go back to VSCode
2. Press **Ctrl + `** (Windows) or **Cmd + `** (macOS) to open the terminal at the bottom
3. Copy and paste this command (replace `YourUsername` with your actual GitHub username):

```
git remote add origin https://github.com/YourUsername/MyFirstProject.git
```

**What does this do?** This connects your local folder to your GitHub repository.

4. Press Enter

### 6b. Create a GitHub personal access token

1. Open your browser
2. Go to: `https://github.com/settings/tokens`
3. Click **Generate new token** → **Generate new token (classic)**
4. In "Note", type: `MyFirstProject`
5. Check the **repo** box
6. Click **Generate token**
7. **Copy the token** (it's a long code)
8. Save it in a text file somewhere safe

---

## Step 7: Push to GitHub

Now you upload your committed code to GitHub.

### Option A: Use VSCode UI (Easiest)

#### 7a. Set your Git identity (first time only)

1. Press **Ctrl + `** (Windows) or **Cmd + `** (macOS) to open the terminal
2. Type:
```
git config --global user.name "Your Name"
```
3. Press Enter, then type:
```
git config --global user.email "your.email@gmail.com"
```
4. Press Enter

#### 7b. Push your code

1. In VSCode, go to **Source Control** (left sidebar)
2. Click the three dots **...** menu
3. Click **Push**
4. VSCode might ask for your credentials:
   - **Username:** Your GitHub username
   - **Password:** Paste your personal access token

Done! Your repository is now on GitHub! 🎉

---

### Option B: Use Terminal Commands

#### 7a. Set your Git identity (first time only)

Type these commands in the terminal (press Enter after each):

```
git config --global user.name "Your Name"
```

```
git config --global user.email "your.email@gmail.com"
```

#### 7b. Push to GitHub

Type this command and press Enter:

```
git push -u origin main
```

**What does this do?** This uploads your commits to GitHub. When it asks for credentials:
- **Username:** Your GitHub username
- **Password:** Paste your personal access token

---

**Use whichever option feels more comfortable to you. Both do the same thing.**

---

## Make changes later

To upload new changes, you have two options:

### Option A: Use VSCode UI

1. Edit or create a file in VSCode
2. Press **Ctrl + S** or **Cmd + S** to save
3. Go to **Source Control**
4. Click **+** next to your file
5. Type a message describing what you changed
6. Click **Commit**
7. Click the **...** menu and click **Push**

### Option B: Use Terminal Commands

1. Edit or create a file in VSCode
2. Press **Ctrl + S** or **Cmd + S** to save
3. Press **Ctrl + `** (Windows) or **Cmd + `** (macOS) to open the terminal
4. Type and press Enter:
```
git add .
```
5. Type and press Enter:
```
git commit -m "Description of what you changed"
```
6. Type and press Enter:
```
git push
```

**What do these commands do?**
- `git add .` = Stage all your changes
- `git commit -m "..."` = Create a snapshot with a description
- `git push` = Upload to GitHub

---

**Use whichever option feels more comfortable to you. Both do the same thing!**

---

## Troubleshooting

**"Initialize Repository" button doesn't appear**
- Make sure you opened VSCode with a folder (not just a file)
- Go to **File** → **Open Folder** and select your `MyFirstProject` folder

**"Push" doesn't work**
- Make sure you completed Step 6a (adding the remote)
- Check your personal access token is correct

**Can't find a button**
- Look for icons on the left sidebar
- Source Control icon looks like three dots with lines

**"Authentication failed"**
- Generate a new personal access token at: https://github.com/settings/tokens
- Make sure you copied the entire token
