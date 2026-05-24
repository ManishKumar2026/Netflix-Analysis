# 📤 How to Upload This Project to GitHub — Step by Step

Follow these steps carefully. Even if you've never used GitHub before, you can do this!

---

## STEP 1 — Create a GitHub Account (if you don't have one)

1. Go to https://github.com
2. Click **"Sign up"**
3. Enter your email, create a password, choose a username
4. Verify your email

---

## STEP 2 — Create a New Repository on GitHub

1. After logging in, click the **"+"** button at the top-right of GitHub
2. Click **"New repository"**
3. Fill in:
   - **Repository name:** `netflix-eda`
   - **Description:** `Exploratory Data Analysis on Netflix Movies and TV Shows dataset`
   - **Visibility:** Public (so recruiters can see it!)
   - ✅ Check **"Add a README file"** → UNCHECK this (we already have one)
4. Click **"Create repository"**

---

## STEP 3 — Install Git on Your Computer

### Windows:
1. Go to https://git-scm.com/download/win
2. Download and install Git
3. During install, choose "Git from the command line and also from 3rd-party software"

### Mac:
Open Terminal and run:
```bash
xcode-select --install
```

### Linux (Ubuntu):
```bash
sudo apt install git
```

**Verify installation:**
```bash
git --version
# Should show: git version 2.x.x
```

---

## STEP 4 — Configure Git (One-time setup)

Open your Terminal (Mac/Linux) or Git Bash (Windows) and run:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@gmail.com"
```

Replace with your actual name and the email you used for GitHub.

---

## STEP 5 — Navigate to Your Project Folder

If your project is saved in Downloads:
```bash
# Windows (Git Bash)
cd ~/Downloads/netflix-eda

# Mac / Linux
cd ~/Downloads/netflix-eda
```

Or wherever you saved the project folder.

---

## STEP 6 — Initialize Git in the Project Folder

```bash
# Initialize a git repository
git init

# Check what files are in the folder
ls
```

You should see: `Netflix_EDA.ipynb`, `netflix_titles.csv`, `requirements.txt`, `README.md`, `plots/`

---

## STEP 7 — Connect to Your GitHub Repository

Copy the URL of your GitHub repo. It looks like:
`https://github.com/YOUR_USERNAME/netflix-eda.git`

Then run:
```bash
git remote add origin https://github.com/YOUR_USERNAME/netflix-eda.git
```

Replace `YOUR_USERNAME` with your actual GitHub username.

---

## STEP 8 — Add All Files and Commit

```bash
# Stage all files (prepare them for upload)
git add .

# Commit = save a snapshot with a message
git commit -m "Initial commit: Netflix EDA project with visualizations"
```

---

## STEP 9 — Push (Upload) to GitHub

```bash
git branch -M main
git push -u origin main
```

Git will ask for your GitHub **username** and **password** (or a personal access token).

### If it asks for a token instead of password:
1. Go to GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Click "Generate new token"
3. Check the **"repo"** scope
4. Copy the token and paste it as your password

---

## STEP 10 — Verify on GitHub 🎉

1. Go to `https://github.com/YOUR_USERNAME/netflix-eda`
2. You should see all your files uploaded!
3. The README.md will automatically display as the project description

---

## 🔄 Updating Your Project Later

Whenever you make changes:
```bash
git add .
git commit -m "Updated analysis / added new chart"
git push
```

---

## 💡 Pro Tips for a Great GitHub Profile

- Add a **profile picture** and **bio** on GitHub
- Pin this repository to your profile
- Add **topics** to your repo: `python`, `data-analysis`, `pandas`, `matplotlib`, `netflix`, `eda`
- Share the link on LinkedIn!

---

## ❓ Common Errors and Fixes

| Error | Fix |
|-------|-----|
| `git: command not found` | Install Git from git-scm.com |
| `Permission denied` | Use a Personal Access Token as password |
| `remote origin already exists` | Run: `git remote remove origin` then add again |
| Files too large | Add large files to `.gitignore` |

---

*You've got this! 💪 Once it's up, share the link proudly.*
