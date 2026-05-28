# Contributing to LinkedIn 360-Degree Analysis

Thank you for interest in improving this project! Here's how you can help.

## Ways to Contribute

### 1. Report Issues
Found a bug? Have a suggestion?

**Open an issue:**
1. Go to the Issues tab
2. Click "New issue"
3. Describe what you found (be specific)
4. Include example if possible

**Good issue examples:**
- "Claude doesn't recognize Reforge PM framework"
- "The HTML output is cutting off text for long names"
- "Suggestion: add Executive readiness level indicator"

### 2. Improve Documentation
See a typo or confusing explanation?

**How to contribute:**
1. Fork the repo
2. Edit the file
3. Commit with a clear message
4. Submit a Pull Request

**Docs that often need help:**
- README.md (clarity improvements)
- USAGE-GUIDE.md (add tips you discovered)
- Inline comments in the skill

### 3. Suggest New Frameworks
Want to add a framework for sales leaders, engineers, or other roles?

**How to suggest:**
1. Open an issue with title: "Suggest new framework: [Role]"
2. Describe the 8-10 key competencies
3. Give 2-3 example definitions

**We're interested in:**
- VP Engineering
- VP Sales
- Head of HR
- CTO
- Founding team roles

### 4. Improve the Skill Definition
Found a better dimension definition or signal word?

**How to contribute:**
1. Fork the repo
2. Edit `linkedin-360-skill.md`
3. Make improvements
4. Include reasoning in PR description

**Areas we're always refining:**
- Dimension/competency definitions
- Signal words (words that indicate each dimension)
- Output formats
- Edge case handling

### 5. Create Examples
Build an analysis using your own recommendations? Share it!

1. Create a folder: `examples/[your-name].html`
2. Add your analysis
3. Add a README explaining what role/context it's for
4. Submit PR

This helps others see what output looks like.

### 6. Build Tools on Top
Want to build a web interface, bot, or integration?

**You can:**
- Fork and build
- Create a new repo that uses the skill
- Link back to us
- Let us know (we might feature it)

**Examples:**
- Web form that generates analyses
- Slack bot that analyzes recommendations
- LinkedIn integration (respecting ToS)
- Video tutorial

## Code of Conduct

Be respectful. This is a collaborative project built by the community.

- Be kind to other contributors
- Assume good intent
- Provide constructive feedback
- Welcome diverse perspectives

## Pull Request Process

1. **Fork the repo**
   ```bash
   # Click "Fork" on GitHub
   ```

2. **Create a branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make changes**
   - Edit the files you want to improve
   - Keep changes focused (one feature per PR)

4. **Test your changes**
   - If it's the skill: paste into Claude and verify
   - If it's docs: check formatting
   - If it's code: run locally

5. **Commit clearly**
   ```bash
   git commit -m "Improve: [what you improved]"
   ```

6. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

7. **Open a Pull Request**
   - Go to GitHub
   - Click "Compare & pull request"
   - Describe what you changed and why
   - Click "Create pull request"

8. **Address feedback**
   - Maintainers may ask questions
   - Make requested changes
   - Push updates to the same branch

9. **Merge**
   - Maintainer merges when ready
   - You're a contributor!

## Good First Issues

Looking to get started?

- **Documentation:** Improve clarity in existing docs
- **Examples:** Create an example analysis
- **Testing:** Verify the skill works with edge cases
- **Typos:** Fix grammar/spelling

These are great entry points!

## Questions?

- **Open an issue:** For questions about contributions
- **Comment on PR:** For discussion about a specific change
- **Email:** For sensitive topics

## Recognition

All contributors are recognized in:
- CONTRIBUTORS.md file
- Commit history
- GitHub insights

Thank you for making this better! 🙌

---

## Contributor Checklist

Before submitting a PR, check:

- [ ] Changes are focused and clear
- [ ] Documentation is updated if needed
- [ ] Grammar/spelling is correct
- [ ] Code/skill logic is tested
- [ ] Commit messages are descriptive
- [ ] No unrelated files are included

---

## What We're Looking For

**High priority:**
- Bug fixes
- Documentation improvements
- New frameworks (with clear definitions)
- Skill definition refinements

**Medium priority:**
- Quality examples
- Edge case handling
- Testing improvements

**Lower priority (but welcome):**
- UI/design suggestions
- Tool integrations
- Meta discussions

---

## Getting Help

Stuck? Don't know where to start?

1. Comment on an issue you're interested in
2. Open a discussion
3. Ask in a PR

We're here to help new contributors succeed.

---

**Thanks for contributing!** 🚀
