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

<img width="978" height="429" alt="Screenshot 2026-09-04 at 6 58 55 PM" src="https://github.com/user-attachments/assets/b4c581e4-c299-4bd8-ad1b-0d2a4ad3e7d8" />
<img width="982" height="342" alt="Screenshot 2026-09-04 at 6 59 10 PM" src="https://github.com/user-attachments/assets/1efdac46-cc4f-40ea-b789-144ff723ebe6" />
<img width="995" height="410" alt="Screenshot 2026-09-04 at 6 59 17 PM" src="https://github.com/user-attachments/assets/9a9f6b33-adbc-4495-9c9e-e1196c977e93" />
<img width="989" height="626" alt="Screenshot 2026-09-04 at 6 58 05 PM" src="https://github.com/user-attachments/assets/9e7dc757-0e07-4b93-9577-068e3f8b6b70" />
<img width="991" height="639" alt="Screenshot 2026-09-04 at 6 58 18 PM" src="https://github.com/user-attachments/assets/50443992-99c9-4bd3-92db-ecac0027e5d2" />
<img width="1014" height="625" alt="Screenshot 2026-09-04 at 6 58 27 PM" src="https://github.com/user-attachments/assets/49c37631-e5e6-45e7-b34e-19d15cdbb22f" />
<img width="1000" height="638" alt="Screenshot 2026-09-04 at 6 58 39 PM" src="https://github.com/user-attachments/assets/1e82b14c-e9f2-43b6-b784-90c07c55933b" />
<img width="989" height="418" alt="Screenshot 2026-09-04 at 6 59 33 PM" src="https://github.com/user-attachments/assets/8d9705e5-412f-4baa-8ab8-5f4be33cc113" />
<img width="1005" height="612" alt="Screenshot 2026-09-04 at 6 59 44 PM" src="https://github.com/user-attachments/assets/913a5dd8-becd-40e8-b915-9f73732ec08b" />
<img width="993" height="716" alt="Screenshot 2026-09-04 at 7 00 13 PM" src="https://github.com/user-attachments/assets/c9b7c942-e743-4d62-afa2-adc7be076355" />
<img width="1000" height="750" alt="Screenshot 2026-09-04 at 7 00 38 PM" src="https://github.com/user-attachments/assets/b7308975-7a61-4b20-855b-8ad5c60dd012" />
<img width="986" height="744" alt="Screenshot 2026-09-04 at 7 01 04 PM" src="https://github.com/user-attachments/assets/d6d8ad60-b7ed-4045-bb72-5b9696085a88" />
<img width="987" height="766" alt="Screenshot 2026-09-04 at 7 01 26 PM" src="https://github.com/user-attachments/assets/7f4a8600-8e8e-476a-9722-7e3c47779532" />
<img width="1222" height="643" alt="Screenshot 2026-09-04 at 7 23 07 PM" src="https://github.com/user-attachments/assets/a2e656b0-3a12-4462-89a2-a47ea0bdfa88" />
<img width="1433" height="686" alt="Screenshot 2026-09-04 at 7 22 55 PM" src="https://github.com/user-attachments/assets/64bf18ba-9303-43a8-85b0-b00b39ae7ced" />


