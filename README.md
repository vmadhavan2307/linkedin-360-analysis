# LinkedIn 360-Degree Analysis Skill

Synthesize your LinkedIn recommendations into a comprehensive strength profile using Claude AI. No server, no cost to you—runs on the user's tokens.

## What It Does

Takes 10+ LinkedIn recommendations and analyzes them across three professional frameworks:

- **Universal Mode** — 7 core dimensions (intellectual depth, execution, technical mastery, customer obsession, cross-functional leadership, people development, personal excellence)
- **Executive Mode** — 9 dimensions organized in 3 tiers (Strategic Leadership, People Leadership, Foundational Excellence) + tier-level assessment
- **Reforge PM Mode** — 8 PM competencies (strategy, execution, data, user research, design collaboration, technical acumen, cross-functional leadership, communication) + PM archetype analysis

Perfect for:
- Job candidates preparing for executive interviews
- Career transitions and positioning
- Understanding how different people perceive you
- Building interview talking points
- Self-awareness on professional strengths

## How It Works

No installation. No servers. Just copy, paste, and run.

### Quick Start (2 minutes)

1. **Get your recommendations**
   - Go to your LinkedIn profile
   - Scroll to recommendations section
   - Copy all recommendation text (paste into a document first if easier)

2. **Open Claude**
   - Go to [claude.ai](https://claude.ai)
   - Start a new chat

3. **Paste and analyze**
   ```
   I'm using the linkedin-360-analysis skill. Here are my recommendations:

   [PASTE YOUR RECOMMENDATIONS HERE]

   Please analyze using the Executive framework mode.
   ```

4. **Get results**
   - Claude provides detailed analysis across your chosen framework
   - Ask for HTML version if you want to share

## What You Get

### Analysis Output

Each framework provides:
- **Summary** — Core themes and differentiators
- **Dimensional breakdown** — Strength ratings with evidence
- **Narrative** — How strengths fit together, career arc
- **Role positioning** — What to emphasize for specific roles
- **Visual/structured output** — Easy to read and share

### Example Output

See `example-output.html` for a complete sample analysis across all three frameworks.

## Frameworks Explained

### Universal Mode
Best for: Understanding your overall strengths, general career positioning

Output includes:
- 7 dimensions with frequency counts (how many recommendations mention each)
- Recommender diversity (managers vs. peers vs. direct reports vs. customers)
- Career arc narrative
- Positioning for different role types

### Executive Mode
Best for: VP/Director/C-level positioning, executive interviews

Output includes:
- 3-tier scorecard (Strategic Leadership ✓✓✓, People Leadership ✓✓✓, Foundational Excellence ✓✓✓)
- Tier-by-tier assessment
- Executive narrative
- Interview emphasis points
- Ready for executive search conversations

### Reforge PM Mode
Best for: PM-specific roles (Senior PM, PM Manager, Director PM)

Output includes:
- 8 PM competencies with readiness ratings
- Recommender validation per competency
- PM archetype analysis ("Strategic-Execution PM," etc.)
- Stage assessment (Senior PM ready? PM Manager ready?)
- What to emphasize for PM career progression

## The Skill File

**Location:** `linkedin-360-skill.md`

This is the actual skill definition. It includes:
- Complete framework definitions (all 3 modes)
- Workflow instructions for Claude
- Dimension/competency reference with signal words
- Output format specifications
- Edge case handling

## Token Cost

**Zero for you.**

- **Claude.ai users:** Uses their free or paid Claude tokens (they pay, not you)
- **API users:** Uses the user's API tokens
- **No infrastructure:** No servers, no hosting costs

This is completely decentralized—the skill is just a prompt template.

## Privacy

- Recommendations only go to Claude (Anthropic's API)
- Data does NOT touch this repo or any third-party server
- Each user's analysis is independent
- You don't need to log in or create an account

## How to Share This

### Option 1: Link directly to this repo
Share the GitHub URL. People copy the `linkedin-360-skill.md` file.

### Option 2: Share as a gist
```
Copy linkedin-360-skill.md → create a GitHub gist
Share the gist link
People copy-paste into Claude
```

### Option 3: Embed in your own document
You can embed the skill in a newsletter, blog post, or guide.

### Option 4: Post to communities
r/careerguidance, r/productivity, career coaching communities, LinkedIn, etc.

**Example post:**
> "I created a Claude skill that analyzes your LinkedIn recommendations into a 360-degree strength profile. It synthesizes feedback from managers, peers, direct reports, and customers across three frameworks. Uses your tokens, completely free. [LINK]"

## Example Usage

### For a job candidate:

```
I'm targeting VP Product roles at B2B SaaS companies. 
Here are my 26 LinkedIn recommendations:

[PASTE RECOMMENDATIONS]

Please analyze using the Executive framework mode to show 
how my strengths align with VP Product expectations.
```

→ Claude provides tier-level assessment, interview talking points, and positioning guidance.

### For self-awareness:

```
I want to understand how different people perceive my strengths.
Here are my recommendations:

[PASTE RECOMMENDATIONS]

Please analyze using the Universal framework mode.
```

→ Claude shows which strengths are consistent across managers, peers, direct reports, and customers.

### For PM-specific positioning:

```
I'm a product manager considering a promotion to Senior PM.
Here are my LinkedIn recommendations:

[PASTE RECOMMENDATIONS]

Please analyze using the Reforge PM framework and tell me 
my readiness for Senior PM / PM Manager roles.
```

→ Claude rates your 8 PM competencies, identifies gaps, and assesses stage readiness.

## The Skill is Modular

The skill can be extended to analyze:
- Peer reviews (360 feedback from colleagues)
- Customer testimonials
- Stakeholder feedback
- Any multi-source feedback

Just modify the dimension definitions for your use case.

## Files in This Repo

```
linkedin-360-analysis/
├── README.md                          (this file)
├── linkedin-360-skill.md              (the skill definition)
├── FRAMEWORK-DEFINITIONS.md           (detailed framework specs)
├── example-output.html                (sample analysis across all 3 modes)
├── REDDIT-POST-TEMPLATE.md            (how to share on Reddit)
└── USAGE-GUIDE.md                     (step-by-step guide for users)
```

## FAQ

**Q: Do I need a Claude API key?**  
A: No. Use claude.ai (web interface) for free. API users can use their own key if they have one.

**Q: How many recommendations do I need?**  
A: 10+ recommended for meaningful patterns. Works with as few as 5, but patterns are clearer with more.

**Q: Can I use this for other types of feedback?**  
A: Yes. The framework is generic. You can adapt it for peer reviews, customer testimonials, 360 feedback, etc.

**Q: Is my data safe?**  
A: Yes. Data only goes to Claude (Anthropic's API). It doesn't touch this repo, my servers, or any third party.

**Q: How long does analysis take?**  
A: 30–60 seconds depending on recommendation length and Claude's response time.

**Q: Can I customize the frameworks?**  
A: Absolutely. Edit `linkedin-360-skill.md` to modify dimensions, add new frameworks, or adapt for your use case.

**Q: Can I monetize this or offer it as a service?**  
A: Yes. You can offer to run analyses for others (they share recommendations, you provide HTML output). The skill itself is open-source under MIT.

## For Recruiters & Coaches

This skill is useful for:
- **Recruiters:** Quickly understand candidate strengths from public LinkedIn data
- **Coaches:** Offer as a client deliverable for career positioning
- **Teams:** Analyze peer feedback to understand team dynamics
- **HR:** Understand employee strengths for role matching

You can:
1. Use the skill with client recommendations
2. Generate HTML output
3. Share the analysis with the person
4. Use in coaching/mentoring conversations

## Contributing

Have ideas for improvements?
- Suggest new frameworks
- Improve dimension definitions
- Add edge case handling
- Submit PR with refinements

## License

MIT License. Use, modify, share freely. Attribution appreciated but not required.

## About the Author

This skill was created to solve a real problem: LinkedIn gives you raw recommendation data, but no tools to extract the actual signal from the noise. It's designed to work with Claude and scale infinitely with zero infrastructure cost.

Questions? Open an issue or reach out.

---

## Next Steps

1. **Try it:** Copy `linkedin-360-skill.md`, paste into Claude.ai with your recommendations
2. **Share it:** Send the repo link to friends/colleagues doing job searches
3. **Adapt it:** Modify frameworks for your specific use case
4. **Contribute:** Suggest improvements or new frameworks

**Ready to go?** Start here: [Quick Start Guide](USAGE-GUIDE.md)
