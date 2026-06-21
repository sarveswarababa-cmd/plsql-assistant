# 🗄️ PL/SQL AI Assistant
### Built by V. Sarveswarababa | Powered by Claude AI

A professional Oracle PL/SQL tool with 4 modes:
- 📄 PL/SQL → Auto Documentation
- ✍️ English → Oracle SQL Writer
- 🔍 Code Reviewer with fixes
- 🐛 Bug Debugger with diagnosis

---

## ✅ STEP-BY-STEP SETUP & DEPLOYMENT

---

## PART 1 — Install Tools on Your PC (One-time setup)

### Step 1: Install Node.js
1. Go to 👉 https://nodejs.org
2. Download **LTS version** (the green button)
3. Install it — click Next → Next → Finish
4. To verify, open **Command Prompt** and type:
   ```
   node --version
   ```
   You should see something like `v20.x.x`

### Step 2: Install Git
1. Go to 👉 https://git-scm.com/downloads
2. Download for Windows → Install (all defaults are fine)
3. To verify, open Command Prompt and type:
   ```
   git --version
   ```

---

## PART 2 — Get Your Anthropic API Key

### Step 3: Create API Key
1. Go to 👉 https://console.anthropic.com
2. Sign up with your email (free account)
3. Click **"API Keys"** in the left menu
4. Click **"Create Key"**
5. Copy the key — it looks like: `sk-ant-api03-xxxxxxxxxxxx`
6. ⚠️ Save it somewhere safe — you won't see it again!

> 💡 Free tier gives you enough credits to test. You can add a card later for more.

---

## PART 3 — Run the App on Your Computer

### Step 4: Download this project
Open **Command Prompt** and run these commands one by one:

```bash
# Go to your Documents folder
cd C:\Users\YourName\Documents

# Create and enter the project folder
mkdir plsql-assistant
cd plsql-assistant
```

Then copy all the project files into this folder (App.js, package.json, etc.)

### Step 5: Set up your API Key
In the project folder, create a file called `.env`:

```bash
# In Command Prompt:
echo REACT_APP_ANTHROPIC_API_KEY=sk-ant-api03-YOURKEY > .env
```

Or open Notepad, type this and save as `.env` in the project folder:
```
REACT_APP_ANTHROPIC_API_KEY=sk-ant-api03-YOURKEY
```
Replace `sk-ant-api03-YOURKEY` with your actual key from Step 3.

### Step 6: Install and Run
```bash
# Install all dependencies (takes 2-3 minutes first time)
npm install

# Start the app
npm start
```

✅ The app opens automatically at: **http://localhost:3000**

---

## PART 4 — Deploy to Internet (Free, Permanent URL)

### Step 7: Create GitHub account
1. Go to 👉 https://github.com
2. Sign up (free)

### Step 8: Push your code to GitHub
```bash
# Inside your project folder:
git init
git add .
git commit -m "PL/SQL AI Assistant - first version"

# Go to github.com → New Repository → name it "plsql-assistant"
# Then run (replace YOUR_USERNAME):
git remote add origin https://github.com/YOUR_USERNAME/plsql-assistant.git
git push -u origin main
```

### Step 9: Deploy on Vercel (Free hosting)
1. Go to 👉 https://vercel.com
2. Sign up with your GitHub account
3. Click **"New Project"**
4. Click **"Import"** next to your `plsql-assistant` repo
5. Click **"Environment Variables"**
6. Add:
   - Name: `REACT_APP_ANTHROPIC_API_KEY`
   - Value: `sk-ant-api03-YOURKEY` (your real key)
7. Click **"Deploy"**

✅ In 2 minutes you get a live URL like:
**https://plsql-assistant-yourname.vercel.app**

---

## 🔁 How to Update Your App Later

Whenever you change the code:
```bash
git add .
git commit -m "describe what you changed"
git push
```
Vercel automatically redeploys! ✨

---

## ❓ Troubleshooting

| Problem | Solution |
|---|---|
| `npm not found` | Reinstall Node.js from nodejs.org |
| App shows "API key missing" | Check your .env file has the key correctly |
| App opens but Claude doesn't respond | Check your API key is valid at console.anthropic.com |
| `git push` asks for password | Use a GitHub Personal Access Token instead |

---

## 📁 Project File Structure

```
plsql-assistant/
├── public/
│   └── index.html          ← App HTML shell
├── src/
│   ├── index.js            ← React entry point
│   └── App.js              ← MAIN APP (all logic + UI)
├── .env                    ← Your API key (never share!)
├── .env.example            ← Template for .env
├── .gitignore              ← Keeps .env out of GitHub
├── package.json            ← Project config
└── README.md               ← This guide
```

---

## 🚀 What Each Mode Does

| Mode | You Give It | You Get Back |
|---|---|---|
| 📄 PL/SQL → Docs | A procedure / function / package | Full technical documentation |
| ✍️ English → SQL | Plain English requirement | Optimized Oracle SQL + explanation |
| 🔍 Code Review | Any PL/SQL code | Score, issues found, improved version |
| 🐛 Debug / Fix | Buggy code + error | Diagnosis, fixed code, prevention tips |

---

Built with ❤️ using React + Claude AI
