# Reddit Post Templates

Use these templates to share the skill on Reddit. Customize based on the subreddit.

---

## Template 1: r/careerguidance (Career transitions)

**Title:**
```
I built a Claude skill that analyzes your LinkedIn recommendations 
into a 360-degree strength profile. Free, uses your tokens.
```

**Body:**
```
I'm in the middle of a career transition and got frustrated with how generic 
LinkedIn's built-in tools are. So I created a skill for Claude that actually 
*analyzes* your recommendations instead of just showing them.

Here's what it does:

**Three Analysis Frameworks:**
1. **Universal Mode** — Shows your 7 core strengths across managers, peers, direct reports, customers
2. **Executive Mode** — 9 dimensions across 3 tiers (Strategic, People, Foundational) for VP/Director roles
3. **Reforge PM Mode** — 8 PM competencies if you're a product manager

**Why this matters:**
- LinkedIn gives you raw data; this extracts the actual signal
- Shows which strengths are consistent vs. role-specific
- Generates interview talking points automatically
- Differentiates genuine strength from generic praise

**How to use (free, on your tokens):**
1. Copy your LinkedIn recommendations
2. Paste into Claude.ai along with the skill
3. Get a detailed analysis across your chosen framework
4. (Optional) Ask for HTML to share with recruiters

**Example output:**
I analyzed my own 26 recommendations (18-year career arc) and got insights 
like: "You're exceptional at cross-functional influence, validated by 8 
recommenders across manager/peer/engineer/designer/customer. This is rare."

That's the kind of signal that matters in interviews.

**Cost:** Zero for you. Uses your Claude tokens (free tier works, or your subscription).

**Privacy:** Recommendations only go to Claude—no third-party servers, no infrastructure costs, no data collection.

The skill is open-source and free to use, adapt, or share.

If you're job searching, prepping for interviews, or just want to understand 
how people actually perceive you, this might be useful.

[LINK TO GITHUB REPO]

Happy to answer questions!
```

---

## Template 2: r/productivity (Automation/tools angle)

**Title:**
```
Built a free Claude skill that analyzes LinkedIn recommendations 
into a professional strengths profile. No server costs.
```

**Body:**
```
I built a productivity tool around Claude that might be useful for people 
doing career stuff.

**The problem:**
LinkedIn has your recommendations, but they're just a wall of text. 
No synthesis, no patterns, no actionable insights.

**The solution:**
A Claude skill that:
- Takes 10+ recommendations as input
- Analyzes across three professional frameworks
- Outputs a structured strength profile
- Generates interview talking points
- Exports to HTML for sharing

**Why I built it this way:**
- No servers, no hosting costs, no infrastructure
- Uses user's own tokens (they pay, not me)
- Completely decentralized
- Scales infinitely with zero marginal cost
- Privacy-first (data never leaves the user)

**Tech stack:**
- Claude AI (backbone)
- Markdown skill definition (portable)
- HTML output template (shareable)
- Git-based distribution

**Frameworks:**
1. Universal (7 dimensions)
2. Executive (3 tiers)
3. Reforge PM (8 competencies)

**How it works:**
User copy-pastes: skill definition + recommendations → Claude → structured analysis

**Cost to me:** $0 (no infrastructure)  
**Cost to user:** Whatever Claude tokens they use (often free if they have pro)

The whole thing is open-source and anyone can adapt it for other types of feedback 
(peer reviews, customer testimonials, 360 feedback, etc).

[LINK TO GITHUB REPO]

Curious if anyone else has built similar analysis tools around Claude?
```

---

## Template 3: r/jobs (Job search focused)

**Title:**
```
I created a free tool that analyzes your LinkedIn recommendations 
to prep you for executive interviews. Uses your tokens, not mine.
```

**Body:**
```
In the middle of a job search and realized I wasn't using my LinkedIn 
recommendations strategically. So I built a tool to extract actual insights.

**What it does:**
- Takes your LinkedIn recommendations (10+)
- Analyzes them across three professional frameworks
- Extracts your actual strengths (not generic praise)
- Generates interview talking points
- Shows recommender validation (manager vs. peer vs. customer perspective)

**The three modes:**

*Universal* — General strength assessment  
*Executive* — Tier-based analysis for VP/Director roles  
*Reforge PM* — PM competency assessment (if you're a product person)

**Why I made this:**
Most analysis tools are generic. This one actually reads your recommendations 
and extracts patterns. Like:

"You mention 'calm under pressure' 8 times across different people, but 'data-driven' 
only 2 times. Here's what to emphasize in interviews..."

**How to use:**
1. Copy your recommendations from LinkedIn
2. Paste into Claude with the skill
3. Get analysis in 30 seconds
4. Export to HTML to share with recruiters

**Cost:** Free (uses your Claude tokens)

**If you're job searching:**
- Great for interview prep
- Shows you how different people perceive your strengths
- Identifies gaps in perception
- Generates talking points backed by real feedback

The skill is open-source and free. No sign-up, no account, no data collection.

[LINK TO GITHUB REPO]

Currently using this to prep for Director PM interviews. Highly recommend.
```

---

## Template 4: r/ProductManagement (PM-focused)

**Title:**
```
I built a Claude skill that analyzes PM recommendations 
and tells you your PM archetype + readiness for promotion
```

**Body:**
```
As a product manager in career transition, I needed to understand how other 
PMs, designers, engineers, and managers actually perceive my PM strengths.

So I built a skill for Claude that analyzes recommendations across 8 PM 
competencies (Reforge framework):

1. Product Strategy & Vision
2. Execution & Delivery
3. Data & Analytics
4. User Research & Discovery
5. Design Collaboration
6. Technical Acumen
7. Cross-Functional Leadership
8. Communication & Articulation

**What it outputs:**
- Rating for each competency
- Recommender validation (manager vs. engineer vs. designer perspective matters)
- Your PM archetype ("Strategic-Execution PM," "Design-focused PM," etc.)
- Stage readiness (Senior PM? PM Manager? Director PM?)
- What to emphasize for next-level roles

**Example insight:**
"You're a Balanced Strategic-Execution PM—strong in both vision and delivery. 
That's rare. Most PMs are strong in one or the other. Best suited for: 
scaling products at critical inflection points or building PM orgs in complex domains."

**How to use:**
```
Paste recommendations + skill → Claude analyzes → get output
```

**Cost:** Free (your Claude tokens)

**Who this is for:**
- PMs prepping for Senior PM interviews
- PMs wanting to understand their strengths
- PMs considering PM Manager roles
- Teams wanting to understand team composition

Open-source, no sign-up, no data collection.

[LINK TO GITHUB REPO]

Curious if other PMs have thought about this. Feels like PM positioning is 
often more art than science.
```

---

## Template 5: r/careerguidance (Detailed, educational)

**Title:**
```
Career Tool: Free Claude skill that synthesizes LinkedIn recommendations 
into a structured strength profile across 3 professional frameworks
```

**Body:**
```
I've been working on a career positioning project and created a reusable 
Claude skill for analyzing LinkedIn recommendations. Thought it might be useful 
for others here.

**The problem it solves:**

LinkedIn recommendations are great but... they're noise. You get a bunch of 
praise that sounds similar. Hard to extract actual signal:

- Which strengths are real vs. role-specific perception?
- How do managers' views differ from peers' views?
- What should I actually emphasize in interviews?
- Am I ready for the next level?

**The solution:**

A Claude skill that:
1. Parses recommendations
2. Recognizes recommender types (manager vs. peer vs. direct report vs. customer)
3. Analyzes across a professional framework (3 options)
4. Outputs structured insights
5. Generates position-specific talking points

**Three frameworks to choose from:**

**1. Universal (General positioning)**
- 7 dimensions: intellectual depth, execution, technical mastery, customer obsession, 
  cross-functional leadership, people development, personal excellence
- Best for: Understanding yourself, general career positioning

**2. Executive (VP/Director level)**
- 9 dimensions organized in 3 tiers
  - Strategic Leadership: Vision, Execution, Customer Insight
  - People Leadership: Team Building, Cross-Functional Influence, Learning Agility
  - Foundational Excellence: Intellectual Rigor, Presence, Integrity
- Best for: Exec interviews, promotions to VP/Director
- Output: Tier-level scorecard, interview emphasis points

**3. Reforge PM (Product Management specific)**
- 8 PM competencies: Strategy, Execution, Data, User Research, Design Collaboration, 
  Technical Acumen, Cross-Functional Leadership, Communication
- Best for: PM-specific roles, SM/PM Manager/Director PM positioning
- Output: Competency ratings, PM archetype, stage readiness assessment

**How it works:**

No installation. No servers. No infrastructure.

```
1. Copy your LinkedIn recommendations
2. Go to claude.ai
3. Paste: the skill + your recommendations
4. Ask Claude to analyze using your preferred framework
5. Get detailed analysis + interview talking points
6. (Optional) Ask for HTML to share with recruiters
```

**Cost:**

Free for you.
- Uses user's Claude tokens (they pay, not you)
- No infrastructure costs
- Scales infinitely at zero marginal cost
- Completely decentralized

**Privacy:**

Your data only goes to Claude. No third-party servers, no data collection.

**Example use cases:**

- Job candidate prepping for VP Product interview: "Analyze using Executive mode"
- PM wanting to understand strengths: "Analyze using Reforge PM mode"
- Career transition: "Analyze using Universal mode to see broad patterns"
- Team understanding dynamics: "Analyze peer feedback to see team composition"

**The repo includes:**

- Skill definition (copy-paste into Claude)
- Example output (what you'll get)
- Usage guide (step-by-step)
- Reddit post template (share with others)
- Landing page guide (how to explain it)

**Current status:**

Open-source, MIT license. Free to use, modify, share.

I'm currently using this to prep for Director PM interviews and it's been really 
useful for understanding how people actually perceive my strengths (vs. how I perceive myself).

Curious if this is useful for others in career transition. Happy to answer questions.

[LINK TO GITHUB REPO]
```

---

## Posting Tips

1. **Post once per subreddit** (don't spam)
2. **Customize the title** for each community
3. **Adjust tone** based on subreddit culture
4. **Include a GitHub link** (or gist) for easy access
5. **Be honest** about what it does (and doesn't do)
6. **Expect questions** — be ready with clear answers
7. **Don't oversell** — it's a tool, not magic
8. **Offer to help** — "happy to run analysis for anyone interested"

## Best Subreddits to Share On

- r/careerguidance (career transitions)
- r/jobs (job search)
- r/productivity (automation/tools)
- r/ProductManagement (PM-specific)
- r/Entrepreneur (startup founders)
- r/Executive (executive positioning)
- r/IAmA (could do AMA about career transitions)

## Sample Comment Responses

**"How much does this cost?"**
```
Free. Uses your Claude tokens (so if you have Pro, it's included in your subscription. 
If you use the free tier, it's completely free). Zero cost to me, zero cost to you 
beyond whatever you're already paying for Claude.
```

**"Is this safe / does it collect data?"**
```
Completely safe. Your recommendations only go to Claude (Anthropic's API). 
They don't touch my servers or any third party. No data collection, no tracking.
```

**"Can I use this for [non-LinkedIn thing]?"**
```
Yes! The skill is modular. You can adapt the frameworks for peer reviews, 
customer testimonials, 360 feedback, or any multi-source feedback.
```

**"This seems overly complicated for just summarizing recommendations"**
```
Fair point. What makes it different: it recognizes recommender types (manager 
vs. peer vs. customer), extracts patterns, and maps to specific frameworks 
(executive vs. PM vs. general). Simple summary tools exist; this is about 
extracting signal from noise.
```

---

## After You Post

**Track engagement:**
- Which template got best response?
- What questions came up?
- Did people actually use it?
- What feedback did you get?

**Iterate:**
- Refine based on feedback
- Update README with common questions
- Improve documentation based on confusion points

**Expand:**
- Share in other communities
- Build simple landing page (next section)
- Consider web version if demand exists
