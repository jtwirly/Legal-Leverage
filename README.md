# Legal-Leverage
Explore where legal systems can change - and why.

**Explore where legal systems can change — and why.**

Legal Leverage is a computational law tool that applies system dynamics modeling
to Canadian law, helping users identify high-leverage points for legal or
policy intervention on a topic of their choosing. Built in Google AI Studio.

This is a prototype that uses AI and AI can make mistakes. This is not legal advice. All sources should be verified independently.

https://ai.studio/apps/159b4463-1e34-4471-aba5-b12df38483a9

## Video

https://www.loom.com/share/a73a278159034f27993765ae2f7f445f

## What it does

A user enters any Canadian policy topic (e.g. "AI regulation," "housing
zoning," "climate change causing emissions") and the application:

1. **Builds a causal loop diagram** — a system dynamics model showing the
   reinforcing (R) and balancing (B) feedback loops driving the issue, with
   labeled polarities (+/-) and institutional delays (||).
2. **Identifies ranked leverage points** — using a leverage points hierarchy
   to locate where a legal or policy intervention would most efficiently shift 
   the system from a reinforcing lock-in toward a balancing equilibrium.
4. **Grounds each leverage point in real legal sources** — relevant statutes,
   case law, and active federal bills, each with an outbound link to the
   original source.
5. **Produces a "Theory of Change"** for the top leverage point — a 6-step
   causal interrogation chain (Systemic Friction → Observed Canadian Law →
   Causal Feedback Loop → Target Leverage Point → Actionable Legal Step →
   Expected Systemic Shift) explaining the hypothesis end to end.
6. **Recommends concrete next actions** — e.g. filing a specific application,
   submitting a committee brief, or intervening in a named proceeding.

## Key features

- **Interactive causal loop diagram** — every node, link, and loop is
  clickable, opening a plain-language explanation of what the variable
  means, why a link has the polarity it does, and why a loop reinforces or
  balances the system.
- **Systemic Impact vs. Evidence Confidence scoring** — each leverage point
  is scored on two separate axes rather than one conflated score: Impact
  (theoretical system elasticity) and Confidence (empirical Canadian legal
  precedent support). The UI explicitly warns that a high-leverage point is
  not necessarily a high-confidence one.
- **"Challenge This Recommendation"** — an expandable control for
  interrogating a given leverage point rather than taking the ranking at
  face value.
- **Active federal bills panel** — pulls currently-before-Parliament bills
  relevant to the topic (via OpenParliament.ca and LEGISinfo), each flagged
  with its current stage (e.g. "Second Reading," "In House of Commons") and
  a one-line note on how it bears on the recommendation.
- **Built-in methodology guides** — in-app explainers for "What is System
  Dynamics in Law?", "How to Create the System Dynamics Model" (a 4-step
  protocol: define system boundaries → map causal influences and polarities
  → trace closed feedback loops and delays → identify and rank leverage
  points), and "What is a Legal Theory of Change?"
- **Exportable models** — the causal loop diagram can be exported as
  SD-JSON for use in dedicated system dynamics software (CoModel.io,
  Stella).

## Data sources

The application states every variable, causal link, and statutory lever is
grounded in:

- **Access to Algorithmic Justice (A2AJ)** — Access to Algorithmic
  Justice jurisprudence, covering the Supreme Court of Canada, Federal Court
  of Appeal, and provincial courts.
- **OpenParliament.ca** — active federal legislation, House of
  Commons and Senate bills, committee testimony, second-reading statuses,
  and statutory amendment records.
- **Doctrinal frameworks & systems theory** — Donella Meadows' Twelve
  Leverage Points hierarchy, *Vavilov* administrative-law standards, and
  Charter ss. 1/7/8 frameworks.

Also used in development: **tldraw** for whiteboarding, and **SD-AI**, a
collection of open-source system dynamics modeling tools.

## Known limitations

- **Citation accuracy needs independent verification.** Every citation should be
  spot-checked before this is treated as a research-grade tool rather than a demo.
- **The confidence-score feature is a good mitigation, not a full fix.**
  A confidence score doesn't catch a citation that's simply wrong. The two should be 
  treated as complementary, not substitutes for each other.
- **Onboarding gap for novice users.** The diagram itself doesn't explain
  its own elements without the user actively clicking through — a first-time
  user could view the model without realizing an explanation is available
  per node.

## Future directions

- Expand the databases the application scans — broader web search, official
  government sites (the Canadian analogue to congress.gov), news
  publications, and other media.
- Build out systematic "gut checking" / citation verification as a formal
  pipeline step.
- Improve developmental transparency so the architectural theory behind
  each leverage point is more clearly evidence-based and auditable by a
  user who isn't already familiar with system dynamics.
