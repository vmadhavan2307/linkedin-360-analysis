# How to Use the LinkedIn 360-Degree Analysis Skill

A step-by-step guide to analyze your LinkedIn recommendations using Claude.

## Prerequisites

- Access to Claude (free at [claude.ai](https://claude.ai) or via API/subscription)
- 10+ LinkedIn recommendations (5+ minimum, but more is better)

## Step 1: Get Your LinkedIn Recommendations

1. Go to your LinkedIn profile
2. Scroll down to the "Recommendations" section
3. If you have a "View all recommendations" link, click it
4. Select all the recommendation text (Cmd+A on Mac, Ctrl+A on Windows)
5. Copy (Cmd+C / Ctrl+C)
6. Paste into a text editor or directly prepare for pasting into Claude

**Tip:** Include all metadata (recommender name, title, date, relationship type)

## Step 2: Choose Your Framework

Decide which framework makes sense for your goal:

### Universal Mode
**Best for:** Understanding your overall strengths

"I want to see all 7 core dimensions of my strengths"

### Executive Mode
**Best for:** VP/Director interviews and executive positioning

"I'm preparing for VP/Director roles"

### Reforge PM Mode
**Best for:** PM-specific roles and career progression

"I'm a product manager and want to understand my PM competencies"

## Step 3: Open Claude

Go to [claude.ai](https://claude.ai) and create a new chat.

## Step 4: Copy the Skill (One-time)

Copy the entire `linkedin-360-skill.md` file from the repo.

In your Claude chat, paste the skill file content. This tells Claude how to analyze your recommendations.

## Step 5: Paste Your Recommendations

After pasting the skill, paste your LinkedIn recommendations into the same chat.

## Step 6: Ask Claude to Analyze

Send a message like one of these:

### For Universal Mode:
```
I'm using the linkedin-360-analysis skill to understand my strengths.

Here are my recommendations:

[YOUR RECOMMENDATIONS HERE]

Please analyze using the Universal framework mode and give me a summary of my core strengths.
```

### For Executive Mode:
```
I'm using the linkedin-360-analysis skill and preparing for VP Product roles.

Here are my recommendations:

[YOUR RECOMMENDATIONS HERE]

Please analyze using the Executive framework mode. Show me the tier-level assessment and what I should emphasize in interviews.
```

### For Reforge PM Mode:
```
I'm using the linkedin-360-analysis skill as a product manager.

Here are my recommendations:

[YOUR RECOMMENDATIONS HERE]

Please analyze using the Reforge PM framework mode. Tell me my PM archetype and readiness for Senior PM / PM Manager roles.
```

## Step 7: Review the Analysis

Claude will provide:
- **Summary** of your key strengths
- **Detailed breakdown** by dimension/competency
- **Evidence** from your recommendations
- **Positioning guidance** for specific roles

## Step 8 (Optional): Generate HTML Version

If you want to share with recruiters or save for later, ask Claude:

```
Now generate an HTML version of this analysis that I can save and share. 
Include the full analysis with all details.
```

Claude will generate a standalone HTML file you can:
- Save to your computer
- Email to recruiters
- Share with your network
- Print to PDF

## Tips & Best Practices

### Quality of Recommendations Matters
- **Better input:** Detailed recommendations with specific examples
- **Weaker input:** Generic praise ("great person")
- **Sweet spot:** 20+ recommendations with diverse recommender types

### Recommender Diversity
The analysis is strongest when you have:
- Managers (understand your execution)
- Peers (understand your collaboration)
- Direct reports (understand your leadership)
- Customers/clients (understand your external impact)

### Timespan Matters
- Recommendations spanning multiple years show career evolution
- Recent recommendations show current capability
- Old recommendations show foundational strengths

### Ask Follow-ups
Don't stop at the first analysis. Ask Claude:
- "What am I missing? What should I develop?"
- "How does this compare to typical VP Product profiles?"
- "Generate a 1-page summary I can use in applications"
- "Create interview talking points for [specific company]"
- "Compare my Executive tier balance to the market"

## Common Questions

### Q: Do I have to paste the whole skill file every time?
**A:** No. Once you paste the skill in a chat, you can reuse that chat. Just paste new recommendations if you want to analyze a different set.

### Q: Can I use this for feedback other than LinkedIn recommendations?
**A:** Yes. You can adapt it for peer reviews, customer testimonials, 360 feedback, or any multi-source feedback. The skill is modular.

### Q: How long does analysis take?
**A:** 30–60 seconds, depending on recommendation length and Claude's response time.

### Q: Is the analysis always accurate?
**A:** Claude will accurately identify patterns in what people wrote. If recommendations are vague, the analysis will reflect that. Quality input = quality output.

### Q: Can I share my analysis?
**A:** Absolutely. Generate the HTML version or screenshot the text. Your recommendations are your own data.

## Troubleshooting

### "Claude doesn't understand the skill"
- Make sure you pasted the entire `linkedin-360-skill.md` file
- Include the YAML header at the top
- Try rephrasing your analysis request (Claude is good at understanding variations)

### "The analysis seems shallow"
- You may have fewer than 10 recommendations (quality goes up with more input)
- Your recommendations may be generic (can't extract signal from noise)
- Try the other framework modes to get different angles

### "I want more detail"
- Ask Claude to "expand on the [dimension]" with more evidence
- Request "deeper analysis of why [strength] is rare"
- Ask for "concrete examples from recommendations showing [competency]"

## Next Steps After Analysis

### For Job Search:
1. Save the HTML version
2. Extract key talking points
3. Use in cover letters and interviews
4. Reference specific recommender quotes in conversations

### For Self-Awareness:
1. Share with a mentor or coach
2. Discuss with direct reports to validate
3. Use gaps to guide development priorities
4. Re-analyze annually to track growth

### For Coaching Others:
1. Run the analysis on your reports' recommendations
2. Use as a foundation for development conversations
3. Compare to role requirements to identify gaps
4. Track progress over time

## Getting Help

- **Question about the skill?** Open an issue on GitHub
- **Want to improve it?** Submit a PR or fork the repo
- **Found a bug?** Report it on GitHub
- **Have an idea for a new framework?** Suggest it

---

**Ready to go?** Start with Step 1 and work through to Step 7. Most analyses take 2-3 minutes start to finish.
