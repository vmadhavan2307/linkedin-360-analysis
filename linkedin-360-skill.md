---
name: linkedin-360-analysis
description: Analyze LinkedIn recommendations to create a comprehensive 360-degree strength profile. Use this skill whenever a user provides their LinkedIn recommendations (pasted text, document, or reference to a profile) and wants to understand their core strengths, understand how strengths appear across different relationships, extract themes for career positioning, or build career narrative. This skill synthesizes feedback from multiple stakeholders (peers, managers, direct reports, customers) across time into dimensionalized strengths, key themes, and strategic career positioning insights.
---

# LinkedIn 360-Degree Strength Analysis

A skill for synthesizing LinkedIn recommendations into a comprehensive 360-degree view of professional strengths. Takes all public recommendations from a LinkedIn profile and extracts core themes, dimensions, and strategic positioning insights.

## When to Use This Skill

Use this skill when:
- User provides LinkedIn recommendations (as pasted text, document, or list)
- User asks for career narrative, strength summary, or positioning
- User needs to understand how others perceive them across relationships
- User is preparing for interviews, job search, or career transitions
- User wants to distill feedback into dimensions (leadership, technical, execution, etc.)
- User has 10+ recommendations spanning different roles/companies/time periods
- User targets executive/director roles and wants framework-aligned analysis
- User targets PM roles and wants Reforge-aligned competencies

## Framework Selection

This skill operates in **three modes** based on user context:

1. **Universal Mode** (default): 7-dimension framework for any professional
2. **Executive Mode** (when user mentions VP/Director/C-level roles): 9-dimension framework aligned to McKinsey leadership competencies
3. **Reforge PM Mode** (when user targets PM-specific roles): Product management competencies from Reforge curriculum

**Auto-detection**: Skill will detect intent from user language:
- "I'm targeting VP Product / Director role" → Executive mode
- "I'm a product manager / targeting PM roles" + "I have PM background" → Reforge PM mode
- "What are my strengths?" / no role specified → Universal mode

User can also explicitly specify: *"Analyze using [Universal/Executive/Reforge] framework."*

## Workflow

### Step 1: Intake & Parse

If the user provides recommendations as text:
- Count total recommendations and time span (earliest to most recent)
- Extract metadata: recommender name, role/title, relationship type (peer, manager, direct report, customer), date, company context
- Note if any recommendations have explicit relationship context (e.g., "managed directly," "reported to," "worked with")

If the user provides a document (plain text, PDF, or pasted content):
- Parse the full text into individual recommendations
- Preserve all metadata and context clues

### Step 2: Pattern Recognition Across Dimensions

Analyze recommendations for recurring themes. The dimensions you use depend on the framework mode:

---

## FRAMEWORK DEFINITIONS

### UNIVERSAL MODE: 7-Dimension Framework

Use this for any professional at any level when no specific role is targeted. Most general-purpose; works across functions and seniority.

1. **Intellectual Depth** — First-principles thinking, system understanding, analytical rigor, domain knowledge
   - *Signal words*: "analytical," "nuance," "understands the system," "first-principles," "thought leader," "depth in [domain]"
   
2. **Execution & Delivery** — Zero-to-one ability, roadmap clarity, moving ideas to shipped outcomes, navigating ambiguity
   - *Signal words*: "shipping," "delivery," "roadmap," "clarity," "moving things forward," "getting things done," "ambiguity"
   
3. **Technical Mastery** — Technical depth, systems thinking, data fluency, architecture understanding, engineering collaboration
   - *Signal words*: "technical," "data-driven," "systems," "analysis," "engineering," "understands architecture"
   
4. **Customer Obsession** — User advocacy, listening to customer needs, UX focus, customer-first decision-making
   - *Signal words*: "voice of customer," "listens," "user needs," "UX," "customer focus," "empathy"
   
5. **Cross-Functional Leadership** — Alignment across functions, peer credibility, partnership mindset, stakeholder management
   - *Signal words*: "collaborates," "cross-functional," "stakeholder," "alignment," "partnership," "peer"
   
6. **People Development** — Mentorship, team building, growth-oriented, psychological safety, career investment
   - *Signal words*: "mentorship," "developed team," "coaching," "growth," "development," "people leadership," "trust"
   
7. **Personal Excellence** — Calm under pressure, humility, articulate communication, composure, work ethic
   - *Signal words*: "humble," "calm," "articulate," "composed," "patient," "pleasure to work with," "respectful"

For each recommendation:
- Identify which 1-3 dimensions it primarily supports
- Extract 1-2 key quotes or paraphrased claims that evidence the dimension
- Note the recommender type (manager, peer, direct report, customer, external) — this provides perspective diversity

---

### EXECUTIVE MODE: 9-Dimension Framework (McKinsey + VP/Director)

Use this when user targets Director, VP, or C-level roles. Organized in three tiers: Strategic Leadership, People Leadership, Foundational Excellence. Based on McKinsey Leadership Model with product-specific customization.

**Tier 1: Strategic Leadership**

1. **Vision & Strategy** — Sets multi-year direction; understands market/business dynamics; makes first-principles choices about what matters
   - *Signal words*: "strategic thinking," "marketplace economics," "understands the system," "sets direction," "drives roadmap," "long-term value," "first-principles," "nuance"

2. **Execution at Scale** — Ships complex initiatives; manages dependencies; maintains quality while scaling; delivers results under pressure
   - *Signal words*: "shipped," "delivers," "execution," "manages complexity," "roadmap," "scales," "speed and precision," "month over month," "quality metrics"

3. **Customer/Market Insight** — Grounds strategy in deep understanding of user/market needs; advocates for customer in tradeoffs; owns customer discovery
   - *Signal words*: "voice of customer," "customer obsession," "user-centric," "market insight," "understands needs," "customer discovery," "empathy," "design partnership"

**Tier 2: People Leadership**

4. **Team Building & Talent** — Recruits and develops strong teams; builds culture and psychological safety; retains talent; grows people into new roles
   - *Signal words*: "built team," "developed talent," "mentorship," "people leadership," "grew from X to Y," "career development," "culture," "coaching"

5. **Cross-Functional Influence** — Builds alignment across functions without direct authority; influences peers and executives; manages stakeholders
   - *Signal words*: "cross-functional," "stakeholder management," "alignment," "influence," "collaboration," "partnership," "brings together," "negotiates"

6. **Learning Agility & Adaptability** — Moves into new domains/companies and learns quickly; adapts strategy based on data; thrives in ambiguity; learns from mistakes
   - *Signal words*: "navigated ambiguity," "learned domain," "adaptive," "new domain," "evolution," "ambiguity," "learns quickly," "changes approach"

**Tier 3: Foundational Excellence**

7. **Intellectual Rigor & Judgment** — First-principles thinking; analytical depth; makes sound tradeoff decisions; understands systems holistically
   - *Signal words*: "analytical," "first-principles," "intellectual depth," "rigor," "nuanced," "understands systems," "thoughtful," "analytical framework"

8. **Presence & Communication** — Clear articulation to all levels; calm and composed under pressure; credible; inspires confidence through bearing
   - *Signal words*: "articulate," "calm," "composed," "poised," "clear communicator," "presence," "confident," "respectful," "listens"

9. **Integrity, Humility & Trust** — Honest about limitations; doesn't fake expertise; admits mistakes; intellectually honest; builds trust through consistency
   - *Signal words*: "humble," "honest," "integrity," "transparent," "admits uncertainty," "trust-building," "intellectually honest," "authentic"

---

### REFORGE PM MODE: 8-Dimension PM Competency Framework

Use this when user is a product manager or targets PM-specific roles. Based on Reforge product leadership curriculum with customization for PM-stage hiring. 

**Note**: Verify current Reforge curriculum at reforge.com. This reflects their core PM competency model but may differ from their latest version.

1. **Product Strategy & Vision** — Develops multi-year product vision; identifies market opportunities; defines strategic priorities; aligns roadmap to business goals
   - *Signal words*: "product vision," "strategic roadmap," "identifies opportunities," "prioritizes," "marketplace opportunity," "strategy," "business impact," "long-term vision"

2. **Execution & Delivery** — Ships features/products; manages complex dependencies; maintains velocity; delivers results on timeline; navigates tradeoffs
   - *Signal words*: "shipped," "delivery," "execution," "manages scope," "prioritization," "timeline," "velocity," "delivers month over month," "zero to one"

3. **Data & Analytics** — Uses metrics to drive decisions; sets up success metrics; interprets data; tests hypotheses; quantifies impact
   - *Signal words*: "data-driven," "metrics," "A/B testing," "analytics," "quantifies impact," "measures success," "hypothesis," "measurement," "ROI"

4. **User Research & Discovery** — Understands user needs deeply; conducts discovery; advocates for user voice; balances user needs with business goals
   - *Signal words*: "user research," "voice of customer," "discovery," "understands needs," "customer research," "user testing," "user empathy," "customer obsession"

5. **Design Collaboration** — Partners effectively with designers; advocates for UX; understands design tradeoffs; balances user experience with constraints
   - *Signal words*: "design partnership," "UX focus," "collaborates with design," "design-driven," "user experience," "design thinking," "design collaboration"

6. **Technical Acumen & Systems Thinking** — Understands technical architecture; communicates with engineers effectively; makes technical tradeoffs; thinks systemically
   - *Signal words*: "technical depth," "understands architecture," "works with engineering," "technical tradeoffs," "systems thinking," "platform knowledge," "technical background"

7. **Cross-Functional Leadership & Influence** — Aligns teams across functions; influences without authority; manages stakeholders; builds partnerships
   - *Signal words*: "cross-functional," "influence," "stakeholder management," "alignment," "collaboration," "partnership," "brings teams together," "executive presence"

8. **Communication & Articulation** — Clearly articulates strategy/vision; writes compelling narratives; presents to executives; inspires through communication
   - *Signal words*: "articulate," "communicates vision," "clear writer," "inspires," "storytelling," "presentation," "clarity," "communication"

---

For each recommendation in Reforge mode:
- Identify which 1-3 PM competencies it supports
- Extract quotes that demonstrate PM-level competency (not just execution-level work)
- Note whether signals are from peers, managers, skip-level, or cross-functional partners (designers, engineers, executives)
- Highlight gaps: Which PM competencies have weak or missing signals?



### Step 3: Synthesize Core Themes

**Framework-independent patterns** to look for:

- **Consistency**: Which dimensions appear across 5+ recommendations? Those are core strengths (regardless of framework).
- **Recommender agreement**: Do managers, peers, and direct reports all mention the same dimension? Strong signal of genuine strength vs. role-specific perception.
- **Specificity**: Quotes with examples ("did X, achieved Y") are stronger than generic praise ("great leader").
- **Evolution over time**: Does a strength get stronger or differently framed as the person progresses? Shows growth trajectory.
- **Uniqueness**: Which strengths don't appear in every recommendation? Those are differentiators.

**Framework-specific synthesis**:

- **Universal mode**: Look for natural clusters. The 7 dimensions will often group into 2-3 meta-themes (e.g., "intellectual + execution" or "people + customer focus").

- **Executive mode**: Tier-check balance. Ideally, executive strength profile should have:
  - At least 2/3 Strategic dimensions strong (Vision, Execution, Customer Insight)
  - At least 2/3 People dimensions strong (Team, Influence, Adaptability)
  - All 3/3 Foundational dimensions strong (Rigor, Presence, Integrity)
  - If a tier is weak, that's a development area for the role.

- **Reforge PM mode**: PM-specificity check. Look for:
  - Which competencies have "strategic" signals vs. "execution" signals (shows career stage readiness)
  - Whether user has technical depth or is more business/user-focused (shows PM archetype)
  - Recommender diversity: Does signal come from engineers, designers, customers, or mostly managers? Balanced = credible; skewed = role-specific perception.

### Step 4: Build the 360 Constellation

Output structure depends on framework mode:

---

#### UNIVERSAL MODE OUTPUT

**A. Executive Summary (2-3 sentences)**
The one sentence that captures the essence: "Your core strength is [X + Y], which is rare because [why rare]."

**B. Seven Dimensions with Evidence**
For each dimension:
- Definition (what it means in this person's case)
- Frequency (how many recommendations mention it)
- Key quotes (2-3 strongest quotes or paraphrased evidence)
- Recommender diversity (who said it: managers? peers? direct reports? customers?)

**C. Core Narrative**
- What's the overarching story? How do these dimensions fit together?
- What's rare or differentiated about this combination?
- How has this evolved across the person's career arc?

**D. Career Arc Insights**
- Scope expansion: Has the person taken on increasingly complex/larger problems?
- Org impact: Evidence of building/developing teams?
- Domain shifts: Successfully moved into new areas? How?
- Growth: Are early strengths deepening or evolving?

**E. Positioning for Specific Roles**
- What role types would most value these strengths?
- What industries/company stages are best fit?
- What should this person emphasize in interviews?
- What potential gaps exist for certain role types?

---

#### EXECUTIVE MODE OUTPUT

**A. Executive Summary**
Headline capturing rare executive combination: "Strategic [dimension] + People [dimension] + exceptional [foundational]. Differentiated by: [unique aspect]."

**B. Tier Scorecard**
For each tier (Strategic, People, Foundational), show:
- Dimensions present (✓ strong / ◐ moderate / ✗ weak)
- Representative quotes from recommenders
- Recommender breakdown by type (managers / peers / direct reports / customers)

Example:
```
STRATEGIC LEADERSHIP: ✓✓✓ (All strong)
  ✓ Vision & Strategy — "Distill complex challenges into clear direction" (Peer, Peer, Manager)
  ✓ Execution at Scale — "Shipped X, managed Y dependencies, maintained Z metrics" (Manager, Manager, Skip-level)
  ✓ Customer Insight — "Advocates for customer in tradeoffs" (Designer, Customer, Manager)

PEOPLE LEADERSHIP: ✓✓◐
  ✓ Team Building — "Grew 4→10, developed X talent" (Manager, Direct report, Direct report)
  ✓ Cross-Functional Influence — "Aligns across functions" (Peer, Peer, Peer)
  ◐ Learning Agility — Some evidence of domain shifts, but fewer recent examples

FOUNDATIONAL EXCELLENCE: ✓✓✓
  ✓ Intellectual Rigor — "First-principles thinking," "analytical depth" (Multiple)
  ✓ Presence & Communication — "Calm, articulate, composed" (Multiple)
  ✓ Integrity & Humility — "Humble," "honest," "intellectually honest" (Multiple)
```

**C. Executive Narrative**
- How does this profile compare to typical VP/Director roles?
- What's your strongest executive differentiator?
- Any tier-level gaps? (e.g., "People Leadership underdeveloped" vs. Strategic strength)
- How has your executive profile evolved across roles?

**D. Role Fit Analysis**
For user-specified role (VP Product, VP Eng, COO, etc.):
- Which dimensions are most critical for the role
- Where you're overqualified / at parity / underdeveloped
- What to emphasize in interviews
- What might need development or mentoring

**E. Tier-Level Positioning**
- Strategic-heavy + People-moderate = Good for smaller scaling teams, new markets, specialized domains
- People-heavy + Strategic-moderate = Good for organizational turnarounds, team-scaling, culture building
- Balanced = Ready for broader executive scope (GM, VP Gen Mgmt)

---

#### REFORGE PM MODE OUTPUT

**A. Executive Summary**
"Strongest in [PM competencies], differentiated by [rare combo], with [arch-type: strategy-focused / execution-focused / design-focused / data-focused / engineering-focused]."

**B. PM Competency Scorecard**
For each competency:
- Strength rating (strong / moderate / weak)
- Key evidence quotes
- Source diversity: Do quotes come from engineers? Designers? Manager? Other PMs? Stakeholders?

Example:
```
PRODUCT STRATEGY & VISION: ⭐⭐⭐⭐⭐
"Distill complex challenges into clear strategic direction" (Manager, 2025)
"Sophisticated perspective on marketplace economics" (Peer, 2026)
Source diversity: Manager, Peer, Customer
Interpretation: Strong strategic thinking, validated by multiple perspectives

EXECUTION & DELIVERY: ⭐⭐⭐⭐⭐
"Excellent job taking initiatives from zero to one" (Peer, 2026)
"Delivers results with speed and precision" (Manager, 2025)
Source diversity: Manager (2×), Peer (2×), Skip-level (1×)
Interpretation: Consistently strong execution, multi-stakeholder validation

DATA & ANALYTICS: ⭐⭐⭐⭐
"Analytic sense and attention to detail" (Peer, 2013)
"Depth in data analysis" (Manager, 2013)
Source diversity: Manager, Peer (but older recommendations)
Interpretation: Strong data skills, but less recent evidence; may be underutilized or lower priority

USER RESEARCH & DISCOVERY: ⭐⭐⭐⭐
"Listens to Voice of Customer," "customer obsession" (Multiple)
"Deeply understands user needs" (implied across design partnership mentions)
Source diversity: Manager, Peer, Designer, Customer
Interpretation: Very strong customer focus, but fewer explicit "research/discovery" mentions

DESIGN COLLABORATION: ⭐⭐⭐⭐
"Partners exceptionally well with design" (Designer, 2025)
"Balances user needs, business goals, technical constraints" (Designer, 2025)
Source diversity: Designer (primary), implied in execution stories
Interpretation: Design-focused, but validation mostly from designer perspective

TECHNICAL ACUMEN: ⭐⭐⭐⭐
"Strong application development background" (Manager, 2012)
"Technical understanding of systems" (implied across multiple)
Source diversity: Manager, peers in technical contexts
Interpretation: Solid technical foundation, particularly strong in systems thinking

CROSS-FUNCTIONAL LEADERSHIP: ⭐⭐⭐⭐⭐
"Collaborates effectively across functions" (Multiple)
"Brings together cross-functional teams" (Manager, 2020)
Source diversity: Manager, Peer, Engineer, Designer, Marketer
Interpretation: Exceptional cross-functional credibility across wide range of functions

COMMUNICATION & ARTICULATION: ⭐⭐⭐⭐⭐
"Articulate," "clear communicator" (Multiple)
"Thoughtful, articulate, exceptionally sharp" (Senior peer, 2026)
Source diversity: Manager, Peer, Skip-level
Interpretation: Recognized communicator, can inspire confidence in presentations
```

**C. PM Archetype & Stage Analysis**
- **PM Archetype**: Based on competency balance, identify which type:
  - Strategy PM (Strategy + Vision strong, Data strong, Execution solid) → Good for platform/vision roles
  - Execution PM (Execution + Delivery strong, Data strong) → Good for scaling/optimization roles
  - Design-partnered PM (Design + User Research + Communication strong) → Good for consumer/UX-critical products
  - Technical PM (Technical + Systems thinking strong) → Good for infrastructure/developer platform roles
  - Balanced PM (All competencies solid) → Ready for multiple contexts

- **Career Stage Signal**: 
  - Recent strong evidence across all competencies = Ready for Senior PM / PM Manager roles
  - Older/weaker signals in some areas = May be underdeveloped or less prioritized in recent roles

**D. Role Fit Analysis**
For target PM role, show:
- Which competencies are critical
- Your fit (strong / moderate / gap)
- What to emphasize in interviews
- Potential development areas

Example:
```
VP Product at B2B Marketplace Platform

Critical competencies:
  ✓ Product Strategy & Vision (you're exceptional here)
  ✓ Execution & Delivery (you're strong)
  ✓ Data & Analytics (moderate signal; platform roles need deep metrics thinking)
  ◐ Cross-Functional Leadership (strong, but at VP level needs org design component)
  ? Technical Acumen (solid, platform roles benefit from deeper systems understanding)

Recommendation: You're very well-positioned. Emphasize:
  - Marketplace economics understanding (Strategy)
  - Zero-to-one execution track record (Execution)
  - Cross-functional influence at scale (Leadership)

In interviews, discuss:
  - Specific examples of metrics/data driving decisions (strengthen Data perception)
  - How you'd build the product org/structure (org design is VP-level expectation)
  - Technical architecture decisions in recent roles (depth of systems thinking)
```

**E. Benchmarking (Optional)**
- How does your PM profile compare to typical Senior PM / PM Manager / Director PM profiles?
- Strengths that are exceptional for your level
- Competencies that need development to move to next level

### Step 5: Create Visualization (Optional, Framework-Specific)

**Universal Mode Visualization**: Radial diagram with 7 dimensions radiating from center, sized by frequency/strength

**Executive Mode Visualization**: Three-tier pyramid or concentric circles showing Strategic (outer) → People (middle) → Foundational (core), with heat-map coloring for strength

**Reforge PM Mode Visualization**: Bar chart or radial showing 8 competencies with ratings, or skill matrix showing which recommender types validate each competency

---

## Output Format

**Universal Mode**: Summary → Dimensional breakdown → Synthesis narrative → Strategic positioning → Visual diagram

**Executive Mode**: Summary → Tier scorecard → Executive narrative → Role fit analysis → Tier-level positioning

**Reforge PM Mode**: Summary → PM competency scorecard → PM archetype analysis → Role fit analysis → Benchmarking against stage

## Key Principles

- **Specificity over generic**: "Listens to customers and implements their feedback in complex system designs" beats "good product manager."
- **Show the work**: Always cite evidence. Quote recommenders. Show why you're drawing conclusions.
- **Recommender diversity matters**: A dimension supported by a manager, peer, and direct report is stronger than one supported by three peers.
- **Avoid generic praise**: "Great leader" needs to be reframed as "builds trust through XYZ, which shows in [evidence]."
- **Look for combinations**: Rare strengths are often combinations (e.g., "intellectual depth + execution speed" or "technical mastery + humility").
- **Timescale context**: Earlier recommendations (2008–2012) show foundational work; recent ones (2023–2026) show current capability. Note evolution.

## Example Output: Three Framework Modes

### UNIVERSAL MODE Example

```
## Vijay Madhavan: 360-Degree Strength Profile (Universal Mode)

### Executive Summary
Rare combination of intellectual depth (first-principles thinking) + disciplined execution 
(clarity to delivery) + personal excellence (humility), grounded in system-level understanding 
of complex domains (marketplaces, streaming media, data analytics). 26 recommendations across 
18-year career from 7 recommender types. Strongest differentiator: ability to distill complex 
problems into clear strategy while building and developing teams.

### Dimensions (one detailed section per dimension)

**1. Intellectual Depth** [Frequency: 8/26 recommendations]
- Recommender types: 2 managers, 3 peers, 1 direct report, 2 customers
- Key evidence: [quotes with specific evidence]
- Career arc: [how this evolved from 2008 to 2026]

...continuing for all 7 dimensions
```

### EXECUTIVE MODE Example

```
## Vijay Madhavan: Executive Profile (VP Product / Director Level)

### Executive Summary
Strategic executive with exceptional intellectual rigor and execution discipline. Strongest in 
Vision & Strategy (marketplace economics thinking) and Execution at Scale (shipped complex 
initiatives). People leadership validated by direct report testimonials. Rare combination: 
first-principles strategic thinking + ability to move from ideation to delivery while 
developing talent. Ready for VP/Director scope.

### TIER SCORECARD

STRATEGIC LEADERSHIP: ✓✓✓ (All dimensions strong)
  Vision & Strategy (⭐⭐⭐⭐⭐): "Sophisticated perspective on marketplace economics" (Peer, 2026)
  Execution at Scale (⭐⭐⭐⭐⭐): "Executes from zero to one with speed and precision" (Manager, 2025)
  Customer Insight (⭐⭐⭐⭐): "Advocates for customer needs in complex tradeoffs" (Designer, 2025)

PEOPLE LEADERSHIP: ✓✓✓ (All dimensions strong)
  Team Building (⭐⭐⭐⭐⭐): "Grew 4→10, mentored through career transitions" (Direct reports, multiple)
  Cross-Functional Influence (⭐⭐⭐⭐): "Aligns across all functions" (Multiple peer types, 2013–2025)
  Learning Agility (⭐⭐⭐⭐): "Successfully navigated 5 different companies/domains" (Career trajectory evident)

FOUNDATIONAL EXCELLENCE: ✓✓✓ (All dimensions strong)
  Intellectual Rigor (⭐⭐⭐⭐⭐): "First-principles, analytical, intellectually honest" (Multiple)
  Presence & Communication (⭐⭐⭐⭐⭐): "Articulate, calm, composed, humble" (All levels)
  Integrity & Humility (⭐⭐⭐⭐⭐): "Humble, no ego, listens to feedback" (Multiple)

### Assessment for VP Product Role
You are exceptionally well-positioned for VP Product at a platform or marketplace company. 
All three tiers are strong. Your particular differentiation: deep systems thinking + ability 
to execute at scale + building teams. Recommended emphasis in interviews: specific examples 
of marketplace economics thinking + team development at scale + navigating ambiguity in 
multi-year initiatives.
```

### REFORGE PM MODE Example

```
## Vijay Madhavan: PM Competency Profile (Reforge Framework)

### Executive Summary
Exceptional PM profile across all eight competencies, with particular strength in Strategy, 
Execution, and Cross-Functional Leadership. Archetype: Balanced Strategic-Execution PM (strong 
in both vision and delivery, unusual combination). Validated by diverse recommender types 
(managers, peers, engineers, designers, customers). Ready for Senior PM → PM Manager transition.

### PM COMPETENCY SCORECARD

⭐⭐⭐⭐⭐ PRODUCT STRATEGY & VISION
  Evidence: "Distill complex challenges into clear strategic direction" (Manager, 2025)
           "Sophisticated perspective on marketplace economics" (Peer, 2026)
  Sources: Manager (2 recs), Peer (2 recs), Customer (1 rec)
  Interpretation: Strategic thinking validated across hierarchy and external stakeholders
  Reforge readiness: Advanced (ready to teach/mentor others on strategy)

⭐⭐⭐⭐⭐ EXECUTION & DELIVERY
  Evidence: "Zero to one builder," "delivers with speed and precision" (Multiple)
  Sources: Manager (3×), Peer (2×), Skip-level (1×)
  Interpretation: Consistently strong execution, not a role-specific perception
  Reforge readiness: Advanced

⭐⭐⭐⭐ DATA & ANALYTICS
  Evidence: "Significant depth in data analysis" (Manager, 2013)
           "Analytic sense and attention to detail" (Peer, 2013)
  Sources: Manager (2×), Peer (1×) — mostly older recommendations
  Interpretation: Strong capability, but less salient in recent roles; may be underdeveloped or 
                  lower priority in last 5 years
  Reforge readiness: Intermediate (should refresh/deepen metrics thinking for senior PM roles)

⭐⭐⭐⭐ USER RESEARCH & DISCOVERY
  Evidence: "Voice of Customer," "listens with utmost patience," "customer obsession" (Multiple)
  Sources: Manager (2×), Peer (2×), Customer (2×), Designer (1×)
  Interpretation: Deep customer focus, but fewer explicit "research/discovery methodology" mentions
  Reforge readiness: Intermediate-Advanced (strong customer instinct, could formalize discovery process)

⭐⭐⭐⭐ DESIGN COLLABORATION
  Evidence: "Partners exceptionally well with design," "balances user needs + business + tech" (Designer, 2025)
  Sources: Designer (2×, primary), Manager (implied)
  Interpretation: Design partnership is validated but primarily from design perspective; 
                  could strengthen peer PMs' perception
  Reforge readiness: Intermediate-Advanced (excellent collaboration, consider broader org visibility)

⭐⭐⭐⭐ TECHNICAL ACUMEN & SYSTEMS THINKING
  Evidence: "Strong application development background" (Manager, 2012)
           "Understands systems deeply" (implied across marketplace platform work)
  Sources: Manager (1× explicit), Inferred from role context
  Interpretation: Solid technical foundation, particularly strong in platform/system thinking
  Reforge readiness: Intermediate (can deepen technical depth in next role)

⭐⭐⭐⭐⭐ CROSS-FUNCTIONAL LEADERSHIP & INFLUENCE
  Evidence: "Collaborates across all functions" (Multiple)
           "Brings cross-functional teams together" (Manager, 2020)
           "Partners with engineers, designers, marketers, execs" (Role context)
  Sources: Manager (3×), Peer (4×), Designer (1×), Customer (1×)
  Interpretation: Exceptional cross-functional credibility; unusual breadth of stakeholder validation
  Reforge readiness: Advanced (ready to mentor others on influence/stakeholder management)

⭐⭐⭐⭐⭐ COMMUNICATION & ARTICULATION
  Evidence: "Articulate," "clear communicator," "thoughtful, articulate, exceptionally sharp yet humble" (Multiple)
  Sources: Manager (2×), Peer (2×), Skip-level (1×)
  Interpretation: Recognized as strong communicator; can inspire confidence in executive settings
  Reforge readiness: Advanced (could teach communication/storytelling)

### PM ARCHETYPE: Balanced Strategic-Execution PM
You combine strong strategy (marketplace economics, vision) with strong delivery (zero-to-one, 
shipping). This is rare—many PMs are strong in one or the other. Your archetype: "Strategic 
Operator" who can both define where to go and ensure the org gets there. Best suited for: 
scaling products at critical inflection points, taking new platforms to market, or building 
product orgs in complex domains (marketplaces, B2B platforms).

### Reforge Stage Assessment
Current: Senior PM / PM Manager ready (all competencies at advanced level)
Gap for Director PM: Org design, product leadership at scale, mentoring PM teams
Recommendation: Emphasize breadth of competencies (rare) + depth in strategy/execution (very rare)
```

## Edge Cases & Framework-Specific Notes

**Limited recommendations** (< 5): 
- Universal mode: Note that patterns are less robust. Highlight which dimensions are supported by fewest recommenders.
- Executive mode: Flag which tier has weak support (e.g., "People leadership is underdeveloped relative to Strategic").
- Reforge PM mode: Identify which competencies lack validation (e.g., "Data/Analytics has no explicit mentions; infer from execution track record").

**Time gaps**: 
- If recommendations cluster in certain years with gaps, note whether strengths are recent or historical.
- Executive mode: Recent recommendations carry more weight for current capability assessment.
- Reforge PM mode: Gaps in recent evidence may indicate evolving priorities or role context shifts.

**Recommender conflicts**: 
- If dimension has conflicting signals (some say X, others say opposite), flag explicitly and investigate.
- May indicate role-specific perception vs. genuine strength.

**Generic praise** (vague recommendations):
- If most recommendations are warm but lack specificity, output a note: "Recommendations are warm but lack specificity. Strongest evidence is in: [specific section]."
- All frameworks: Prioritize detailed, example-driven recommendations over generic praise.

**Framework mismatch**:
- If user provides PM recommendations but specifies "Executive" framework: Can still analyze, but flag gaps in executive-specific evidence (e.g., "Org design," "Mentoring" may be absent in PM-focused recs).
- Similarly for vice versa.

**Recommender type imbalance**:
- All managers, no peers: May indicate strong manager perception but unclear peer credibility.
- All peers, no direct reports: Can't assess team building/people leadership capability.
- No customers: Harder to assess customer obsession dimension in concrete terms.
- Skill should flag these gaps in recommender diversity and note what's interpretable vs. uncertain.

## Next Steps After Analysis

Once the 360 profile is complete, user can:
1. **Create positioning narrative** for job search (which dimensions to emphasize for which roles)
2. **Draft interview talking points** (backed by specific recommendation examples)
3. **Identify development areas** (dimensions not mentioned, or weak recommender diversity)
4. **Build one-pager** for portfolio (2-page summary of dimensions + key quotes)
5. **Map to job descriptions** (which role dimensions match their strengths)
