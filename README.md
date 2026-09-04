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
- **Legislation and Statutory levers panel** — pulls relevant legislation
- **Case law** — pulls relevant case law
- **Built-in methodology guides** — in-app explainers for "What is System
  Dynamics in Law?", "How to Create the System Dynamics Model" (a 4-step
  protocol: define system boundaries → map causal influences and polarities
  → trace closed feedback loops and delays → identify and rank leverage
  points), and "What is a Legal Theory of Change?"
- **Exportable models** — the causal loop diagram can be exported as
  SD-JSON for use in dedicated system dynamics software (CoModel.io,
  Stella).

## Data sources

The application leverages the following data sources:

- **Access to Algorithmic Justice (A2AJ)** — Access to Algorithmic
  Justice jurisprudence, covering the Supreme Court of Canada, Federal Court
  of Appeal, and provincial courts. https://a2aj.ca/data/
- **OpenParliament.ca** — active federal legislation, House of
  Commons and Senate bills, committee testimony, second-reading statuses,
  and statutory amendment records. http://openparliament.ca/
- **SD-AI**, a collection of open-source system dynamics modeling tools. https://ub-iad.github.io/sd-ai/#/
- **tldraw** for whiteboarding. https://www.tldraw.com/

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

## Screenshots

<img width="987" height="766" alt="Screenshot 2026-09-04 at 7 01 26 PM" src="https://github.com/user-attachments/assets/cff82eeb-133f-41ed-b4f6-f67df6a05526" />
<img width="986" height="744" alt="Screenshot 2026-09-04 at 7 01 04 PM" src="https://github.com/user-attachments/assets/343be9d3-f541-4e89-8894-8bdc6e329e9f" />
<img width="1000" height="750" alt="Screenshot 2026-09-04 at 7 00 38 PM" src="https://github.com/user-attachments/assets/39c3e7a4-447c-4a1f-ac81-642b43cdcc9a" />
<img width="993" height="716" alt="Screenshot 2026-09-04 at 7 00 13 PM" src="https://github.com/user-attachments/assets/dabaa866-f005-4899-ac05-332c1786a5f0" />
<img width="1005" height="612" alt="Screenshot 2026-09-04 at 6 59 44 PM" src="https://github.com/user-attachments/assets/e928684a-5007-46ab-95ea-6e24261b0f78" />
<img width="989" height="418" alt="Screenshot 2026-09-04 at 6 59 33 PM" src="https://github.com/user-attachments/assets/61f0f8b3-08d2-43cc-aafb-afa26e3428f8" />
<img width="995" height="410" alt="Screenshot 2026-09-04 at 6 59 17 PM" src="https://github.com/user-attachments/assets/0e921bd0-d969-4e05-b9e2-69f8888653c6" />
<img width="982" height="342" alt="Screenshot 2026-09-04 at 6 59 10 PM" src="https://github.com/user-attachments/assets/5d6e67fb-aec9-4ad8-b22d-2935859d17ba" />
<img width="978" height="429" alt="Screenshot 2026-09-04 at 6 58 55 PM" src="https://github.com/user-attachments/assets/04e50e5f-ea30-4a18-a976-9f89db7cb938" />
<img width="1000" height="638" alt="Screenshot 2026-09-04 at 6 58 39 PM" src="https://github.com/user-attachments/assets/a540ccbd-abd6-4a9a-8c00-926a896eb02f" />
<img width="1014" height="625" alt="Screenshot 2026-09-04 at 6 58 27 PM" src="https://github.com/user-attachments/assets/57ee0150-5fd0-4e66-a423-92f2a73cf520" />
<img width="991" height="639" alt="Screenshot 2026-09-04 at 6 58 18 PM" src="https://github.com/user-attachments/assets/115e6f8c-07b8-4bc5-8036-c40af0e56afc" />
<img width="989" height="626" alt="Screenshot 2026-09-04 at 6 58 05 PM" src="https://github.com/user-attachments/assets/b85eca80-b7e3-45da-b75a-6d8d00426c0e" />

