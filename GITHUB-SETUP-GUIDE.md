# GitHub Setup Guide

Complete step-by-step instructions to create and set up your LinkedIn 360-Degree Analysis skill repo on GitHub.

## Option A: Quick Setup (5 minutes)

If you just want to get it online quickly:

### 1. Create a GitHub Account (if you don't have one)
- Go to [github.com](https://github.com)
- Click "Sign up"
- Follow the prompts

### 2. Create a New Repository
- Click the "+" icon in the top right
- Select "New repository"
- Name: `linkedin-360-analysis`
- Description: "Synthesize LinkedIn recommendations into a 360-degree strength profile using Claude. Free, runs on your tokens."
- Select "Public"
- Check "Add a README file"
- License: "MIT License"
- Click "Create repository"

### 3. Add the Skill File
- Click "Add file" → "Create new file"
- Name: `linkedin-360-skill.md`
- Paste the entire skill content
- Click "Commit new file"

### 4. Add Example Output
- Click "Add file" → "Upload files"
- Upload `example-output.html`
- Click "Commit changes"

### 5. Share Your Repo
- Copy the repo URL (e.g., `https://github.com/your-username/linkedin-360-analysis`)
- Use this link everywhere

**Done!** Your repo is live.

---

## Option B: Proper Setup (15 minutes)

For a more professional, complete repo setup:

### 1. Install Git (if needed)

**Mac:**
```bash
brew install git
```

**Windows:**
- Download from [git-scm.com](https://git-scm.com/download/win)
- Run installer

**Linux:**
```bash
sudo apt-get install git
```

### 2. Configure Git (first time only)
```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

### 3. Create Local Folder
```bash
mkdir linkedin-360-analysis
cd linkedin-360-analysis
```

### 4. Initialize Git
```bash
git init
```

### 5. Add All Files

Copy these files into your folder:
```
linkedin-360-analysis/
├── README.md
├── linkedin-360-skill.md
├── USAGE-GUIDE.md
├── example-output.html
├── landing-page.html
├── REDDIT-POST-TEMPLATE.md
├── LICENSE
└── .gitignore
```

### 6. Stage Files
```bash
git add .
```

### 7. Create Initial Commit
```bash
git commit -m "Initial commit: LinkedIn 360-Degree Analysis skill"
```

### 8. Create Repository on GitHub
- Go to [github.com/new](https://github.com/new)
- Repository name: `linkedin-360-analysis`
- Description: "Synthesize LinkedIn recommendations into a 360-degree strength profile using Claude"
- Public
- Do NOT initialize with README (you already have one)
- Click "Create repository"

### 9. Push to GitHub
GitHub will show you commands. Run these:

```bash
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/linkedin-360-analysis.git
git push -u origin main
```

(Replace `YOUR-USERNAME` with your actual GitHub username)

### 10. Verify
- Go to your repo URL: `github.com/YOUR-USERNAME/linkedin-360-analysis`
- Check that all files appear
- Test the README renders properly

**Done!** Repo is live and version-controlled.

---

## File Structure (What Goes Where)

```
linkedin-360-analysis/
├── README.md                      (Main documentation - what people see first)
├── linkedin-360-skill.md          (The actual skill - core file)
├── USAGE-GUIDE.md                 (Step-by-step how to use)
├── REDDIT-POST-TEMPLATE.md        (Share on Reddit)
├── example-output.html            (Sample analysis output)
├── landing-page.html              (Share this as a webpage)
├── LICENSE                        (MIT License)
├── .gitignore                     (What to ignore in version control)
└── .github/                       (Optional - GitHub settings)
    └── ISSUE_TEMPLATE/            (Optional - issue templates)
```

---

## What Each File Does

| File | Purpose | Visibility |
|------|---------|-----------|
| `README.md` | Main documentation, landing page | ⭐⭐⭐ (Primary) |
| `linkedin-360-skill.md` | The actual skill definition | ⭐⭐⭐ (Download/copy) |
| `USAGE-GUIDE.md` | How to use the skill | ⭐⭐ (Reference) |
| `example-output.html` | Show what analysis looks like | ⭐⭐ (Inspiration) |
| `landing-page.html` | Share as standalone page | ⭐ (Optional) |
| `REDDIT-POST-TEMPLATE.md` | For sharing on Reddit | ⭐ (Reference) |
| `LICENSE` | MIT license | ⭐ (Legal) |
| `.gitignore` | Git settings | ⭐ (Automatic) |

---

## Customization

### Change the GitHub Description
1. Go to repo settings (gear icon)
2. Scroll to "About"
3. Add description and topics

**Suggested topics:**
```
claude
ai
skill
linkedin
career
product-management
strengths-assessment
```

### Add Topics to Repo
1. Go to repo main page
2. Click gear icon next to "About"
3. Add topics (above)

### Enable Discussions (Optional)
1. Settings → Features
2. Check "Discussions"
3. Allows community Q&A

### Create Releases
1. Go to "Releases"
2. Click "Create a new release"
3. Tag: `v1.0`
4. Title: "Initial release"
5. Description: "First public version of the skill"
6. Publish release

---

## Next Steps After Repo Creation

### 1. Verify Everything Works
- [ ] README displays properly
- [ ] All files are visible
- [ ] Links work
- [ ] Code blocks display correctly

### 2. Test the Skill
- [ ] Copy `linkedin-360-skill.md` content
- [ ] Paste into Claude with recommendations
- [ ] Verify analysis works
- [ ] Make sure it matches `example-output.html`

### 3. Share the Repo
- [ ] Post to Reddit (use REDDIT-POST-TEMPLATE.md)
- [ ] Share in your network
- [ ] Add to your LinkedIn profile
- [ ] Include in portfolio

### 4. Monitor & Maintain
- [ ] Watch for GitHub issues/questions
- [ ] Respond to comments
- [ ] Track usage (stars, forks, issues)
- [ ] Update based on feedback

---

## GitHub Tips

### Getting Your Repo Discovered
- **Stars:** Encourage people to star it
- **Topics:** Use relevant tags (claude, ai, career, etc.)
- **GitHub Trending:** If you get traction, it may appear
- **Social media:** Share the link widely

### Responding to Issues
1. Someone opens an issue
2. You get notified
3. Click "Reply"
4. Provide helpful response
5. Close issue when resolved

### Accepting Contributions
1. Someone forks your repo
2. They make changes
3. They submit a Pull Request (PR)
4. You review their changes
5. Accept or request modifications
6. Merge the PR

**Set expectations in README:**
```
## Contributing

Suggestions welcome! Feel free to:
- Open an issue for bugs or feature requests
- Submit PRs to improve the skill
- Suggest new frameworks or dimensions

All contributions are welcome!
```

---

## Troubleshooting

### "I pushed but files don't appear on GitHub"
```bash
git status  # See what's staged
git add .   # Stage everything
git commit -m "Add files"
git push    # Push to GitHub
```

### "I see 'fatal: not a git repository'"
```bash
git init    # Initialize git in current folder
```

### "README doesn't render properly"
- Check markdown syntax
- Make sure it's named exactly `README.md` (capital letters matter)
- Try viewing in raw format to debug

### "I want to delete the repo"
1. Settings (gear icon)
2. Scroll to "Danger zone"
3. Click "Delete this repository"
4. Type the repo name to confirm

---

## You Now Have

✅ A public GitHub repo  
✅ Professional documentation  
✅ Example output to showcase  
✅ Clear usage instructions  
✅ MIT license (legal clarity)  
✅ Shareable link  
✅ Version control  

---

## Quick Links

- **Your repo:** `https://github.com/YOUR-USERNAME/linkedin-360-analysis`
- **Raw skill file:** `https://github.com/YOUR-USERNAME/linkedin-360-analysis/blob/main/linkedin-360-skill.md`
- **Raw skill (for direct copy):** `https://raw.githubusercontent.com/YOUR-USERNAME/linkedin-360-analysis/main/linkedin-360-skill.md`

**Use the "raw" link when directing people to copy the skill.**

---

## What's Next?

1. **Create the repo** (Option A or B above)
2. **Test it works** (copy skill + recommendations into Claude)
3. **Post to Reddit** (use REDDIT-POST-TEMPLATE.md)
4. **Share in your network** (send the link)
5. **Monitor engagement** (respond to questions, iterate)

---

**Questions?** Open an issue on your repo, and you can work through problems together with your community.
