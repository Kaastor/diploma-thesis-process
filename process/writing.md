# A Practical and Philosophical Guide to Writing a Thesis or Scientific Paper  
*Version 1.0 — “Bootstrap file” for first-time authors and experienced researchers*

---

## How to use this document
This file is designed as both:
1) **A pedagogical guide** (it explains the *why* behind good scientific writing), and  
2) **A reference manual** (it provides actionable *how-to* steps, checklists, and templates).

Scientific writing is not merely “writing down what happened.” It is **the construction of a transparent, testable argument** that connects a question to evidence to inference—so that a skeptical, intelligent reader can decide whether to believe you, reproduce you, or build upon you.

Use it in three ways:
- **Before you write:** to design your argument and structure.
- **While you write:** to draft each section with correct purpose and content.
- **Before you submit:** to audit clarity, rigor, ethics, reproducibility, and presentation.

---

## Table of contents
1. [The philosophy of scientific writing](#the-philosophy-of-scientific-writing)  
2. [Core principles (the “laws of the land”)](#core-principles-the-laws-of-the-land)  
3. [From idea to paper: the research-to-writing pipeline](#from-idea-to-paper-the-research-to-writing-pipeline)  
4. [Planning the document: audience, contribution, and story](#planning-the-document-audience-contribution-and-story)  
5. [Standard structures (paper vs. thesis)](#standard-structures-paper-vs-thesis)  
6. [Section-by-section guide (with why + how)](#section-by-section-guide-with-why--how)  
7. [Figures, tables, and visual evidence](#figures-tables-and-visual-evidence)  
8. [Citations, scholarship, and intellectual honesty](#citations-scholarship-and-intellectual-honesty)  
9. [Methods, statistics, and reproducibility](#methods-statistics-and-reproducibility)  
10. [Style, clarity, and scientific tone](#style-clarity-and-scientific-tone)  
11. [Revision, feedback, and quality control](#revision-feedback-and-quality-control)  
12. [Ethics, authorship, and responsible research](#ethics-authorship-and-responsible-research)  
13. [Submission, peer review, and responding to reviewers](#submission-peer-review-and-responding-to-reviewers)  
14. [Thesis-specific guidance](#thesis-specific-guidance)  
15. [Common failure modes (and how to avoid them)](#common-failure-modes-and-how-to-avoid-them)  
16. [Practical checklists](#practical-checklists)  
17. [Mini-templates and phrase banks (use judiciously)](#mini-templates-and-phrase-banks-use-judiciously)  
18. [Annex A — Deep Learning: Truthful Experiments and Reproducible Systems](#annex-a--deep-learning-truthful-experiments-and-reproducible-systems)  
19. [Annex B — Agentic AI: Evaluating Systems Without Fooling Yourself](#annex-b--agentic-ai-evaluating-systems-without-fooling-yourself)  

---

# The philosophy of scientific writing

## Writing is part of the scientific method
Scientific knowledge is *public* knowledge. A result that cannot be understood, evaluated, or reproduced is not yet fully scientific. Writing is therefore not a cosmetic step after “real work” is done; it is a **core instrument of science**, comparable to measurement and analysis.

### The central philosophical commitment
Scientific writing should let a reader answer, with minimal guesswork:
- **What was asked?**  
- **What was done?**  
- **What was found?**  
- **Why should we believe it?**  
- **What does it mean—and what does it not mean?**

## The goal of good science: reliable knowledge that resists self-deception
If scientific writing is the public interface of science, then the goal of good science can be stated plainly:

**To produce reliable knowledge about the world, under uncertainty, in a way that other minds can audit.**

"Truth" in science is rarely a dramatic absolute. More often it is:
- a measurement with uncertainty,
- a model that predicts within a known regime,
- an explanation that survives attempts to falsify it,
- a result that remains stable when reasonable alternatives are tried.

Good science therefore aims to **minimize avoidable error** (bias, leakage, confounding, measurement artifacts, overfitting, cherry-picking) and to **maximize inspectability** (clear methods, transparent assumptions, complete reporting).

A practical test of whether you are doing good science is not "Does this sound convincing?" but:

- **Would I still believe this if I were trying to prove it wrong?**
- **Could a competent skeptic reproduce the result from my description?**
- **If the result is wrong, can the reader see where it might have gone wrong?**

Scientific writing operationalizes this goal by turning private work into a public, checkable chain of reasoning.

## The paper/thesis is an argument, not a diary
A scientific document is not a chronological record of your activities. It is a **structured argument** where every part serves a function in the reader’s reasoning.

A useful mental model:
- **Claim**: What you assert.
- **Evidence**: What you observed/measured/derived.
- **Warrant**: Why that evidence supports the claim (assumptions, theory, logic, statistics).
- **Scope**: Where it applies, and where it might not.

## Clarity is a form of ethics
Ambiguity wastes time, hides errors, and can mislead. In science, confusing writing is not harmless: it can distort interpretation and impair replication. Strive for writing that is **precise, modest in claims, and explicit about uncertainty**.

---

# Core principles (the “laws of the land”)

These principles apply across disciplines. Conventions differ, but the underlying logic is stable.

## 1) Reader-first design
**Why:** Your reader does not share your context. Your job is to reconstruct it efficiently.  
**How:** State the question early, define terms, and maintain a consistent thread from motivation → method → results → meaning.

## 2) One main contribution per paper (usually)
**Why:** A paper is evaluated as an integrated unit; too many contributions dilute the message and confuse reviewers.  
**How:** Write a one-sentence “contribution statement” and ensure every section supports it.

## 3) Reproducibility is not a slogan; it is documentation
**Why:** Science advances through verification and extension.  
**How:** Record data provenance, parameter choices, exclusions, preprocessing, and analysis decisions. Make the “path from raw to result” inspectable.

## 4) Truthfulness over persuasion (calibration as a virtue)
**Why:** Scientific documents can accidentally become sales pitches. Persuasion is not the purpose; accurate belief is.  
**How:** Make claims proportional to evidence, report uncertainty, disclose negative results when relevant, and separate measurement from interpretation. Prefer being correct and reproducible over being impressive and fragile.

## 5) Separate observation from interpretation
**Why:** Readers must distinguish what *happened* from what you *think it means*.  
**How:** In Results, describe; in Discussion, interpret. When you interpret, label it as interpretation and specify assumptions.

## 6) Precision beats grandeur
**Why:** Overclaiming is punished by reality (and reviewers).  
**How:** Prefer bounded statements (“in this dataset…”, “under these conditions…”, “suggests”) to universal proclamations.

## 7) Every number needs context
**Why:** Numbers are meaningless without units, uncertainty, and conditions.  
**How:** Provide units, sample sizes, variability/uncertainty (SD/SE/CI), and definitions of metrics.

## 8) Writing is iterative engineering
**Why:** Good papers are not written; they are rewritten.  
**How:** Draft quickly, revise structurally, then refine sentences. Do not attempt perfection in the first pass.

---

# From idea to paper: the research-to-writing pipeline

A robust pipeline reduces both errors and anxiety.

## Step A — Define the research question
A good question is:
- **Specific** (not “about X,” but “does X affect Y under conditions Z?”)
- **Answerable** with available methods and resources
- **Interesting** to a defined community
- **Situated** in existing work (you know what would count as “new”)

Deliverable: a 2–5 sentence statement:
1. Problem background  
2. Gap in knowledge  
3. Your question/hypothesis  
4. Your approach  
5. Your expected contribution

## Step B — Decide what counts as evidence
**Why:** Many projects fail at writing time because “evidence” was never defined.  
**How:** Decide:
- Primary outcome(s)
- Secondary outcome(s)
- Inclusion/exclusion criteria
- Baselines and comparisons
- Failure conditions (what would falsify your hypothesis?)

## Step C — Keep a research log that can become Methods
Maintain a living record:
- Instruments, software versions, parameters
- Data collection conditions
- Deviations from plan and why
- Cleaning steps
- Analysis scripts or workflows

This is not bureaucracy; it is future Methods text.

## Step D — Write earlier than you think
Drafting early reveals:
- missing controls
- unclear definitions
- weak measurements
- logic gaps

Writing is a diagnostic tool.

---

# Planning the document: audience, contribution, and story

## Identify your primary reader
Common “primary readers” include:
- A skeptical reviewer in your subfield
- A committee member outside your niche (thesis)
- An applied practitioner (engineering/clinical)
- A methods specialist (statistics/ML)

**How:** Write a 3-line “reader profile”:
- What they already know
- What they doubt
- What they need to see to be convinced

## Define your contribution in one sentence
Examples (generic forms):
- “We propose a method that ___ and demonstrate ___ on ___.”
- “We provide evidence that ___ by measuring ___ under ___.”
- “We resolve ___ by proving/deriving ___.”
- “We curate a dataset/tool that enables ___ and validate it by ___.”

If you cannot write this sentence, the paper is not ready to outline.

## Treat the document as a guided tour of reasoning
A scientific document answers a sequence of reader questions. If you satisfy these in order, the paper becomes easy to follow:
1. Why does this matter?
2. What exactly is unknown?
3. What is your approach?
4. What did you find?
5. Why should I believe it?
6. What does it imply?
7. What are the limits and next steps?

---

# Standard structures (paper vs. thesis)

## Typical scientific paper (IMRaD + framing)
- Title
- Abstract
- Introduction
- Methods
- Results
- Discussion
- Conclusion (sometimes merged with Discussion)
- References
- Appendices / Supplementary material

## Typical thesis (modular and explicit)
Two common thesis patterns:

### A) Monograph thesis
- Introduction / Background
- Literature Review (sometimes separate)
- Methods / Materials
- Results chapters
- Discussion
- Conclusion + Future Work
- Appendices (detailed methods, extra analyses, code/data notes)

### B) Paper-based thesis (thesis by publication)
- General introduction
- 2–4 manuscript-style chapters (published/submitted papers)
- Integrative discussion/conclusion tying them together
- Appendices

**Key difference:** A thesis must demonstrate *mastery, independence, and breadth*; a paper must demonstrate *a focused contribution*.

---

# Section-by-section guide (with why + how)

## Title
### Why it exists
The title is an indexing device and a promise: it tells readers whether this is relevant.

### How to write it
- Include the **core object** (method/system/phenomenon)
- Include the **action** (predicting, measuring, analyzing, improving)
- Include the **domain** (dataset, population, setting) when necessary

Avoid:
- vague words (“novel,” “improved,” “new”) without specifics
- unnecessary cleverness (memorable is good; ambiguous is not)

---

## Abstract
### Why it exists
The abstract is often the only part many readers will read. It must enable accurate triage and correct interpretation.

### How to write it (structured logic)
A strong abstract usually contains:
1. **Context** (1–2 sentences): the problem space  
2. **Gap** (1 sentence): what is missing/unknown  
3. **Approach** (1–2 sentences): what you did  
4. **Results** (1–3 sentences): key quantitative/qualitative findings  
5. **Meaning** (1 sentence): implications and scope  
6. **Limits** (optional, 1 sentence): important constraints

Common mistake: describing what you did but not what you found.

---

## Introduction
### Why it exists
The Introduction constructs the rationale and positions your work in the literature, culminating in a precise question and contribution.

### How to write it (a reliable arc)
A useful structure:
1. **Broad context:** why the area matters  
2. **Narrowed context:** what is specifically challenging/unknown  
3. **Literature map:** what has been tried and what remains unresolved  
4. **Gap statement:** the exact missing piece  
5. **Your approach:** what you do differently  
6. **Contributions:** explicit list or paragraph  
7. **Paper roadmap:** a short guide to the rest

A test of success:
- After reading the Introduction, a reader should be able to predict what Methods and Results will contain.

---

## Related Work / Literature Review
*(Sometimes part of Introduction; often its own chapter in a thesis.)*

### Why it exists
Science is cumulative. You must show:
- you understand the field
- you respect prior work
- your contribution is distinct
- your methods are appropriate

### How to do it well
Do not write a shopping list of citations. Instead:
- Organize by **ideas, approaches, or debates**, not by author chronology.
- Compare studies by: question, data, method, assumptions, findings, limitations.
- Highlight *why* existing results do not settle your question.

Include:
- foundational works (conceptual anchors)
- best current methods/results (state-of-the-art)
- closely adjacent approaches (to prevent “you missed X” reviews)

Thesis-specific guidance: the literature review often doubles as a *tutorial*. Teach the landscape, then locate your work.

---

## Methods (or Materials and Methods)
### Why it exists
Methods are the contract that enables reproduction and valid interpretation. They explain *how your evidence was produced*.

### How to write it
A Methods section should allow a competent researcher to:
- replicate your procedure, or
- implement an equivalent procedure, and
- understand why your choices are reasonable

Include, as applicable:
- Study design (experimental/observational/simulation/theoretical)
- Data sources and collection protocol
- Participants/samples/materials and inclusion/exclusion criteria
- Variables/features and operational definitions
- Instruments and calibration
- Preprocessing and quality control
- Statistical analysis plan (tests/models, assumptions, corrections)
- Software, versions, hardware (for computational work)
- Hyperparameters, training protocol, validation strategy (ML)
- Ethical approvals and consent (human/animal/field work)

#### Methods philosophy: expose degrees of freedom
Readers should see where choices could have been made differently:
- alternative preprocessing
- alternative model specifications
- selection criteria
- stopping rules
- outlier handling

When you made choices, state:
- what you did
- why you did it
- what sensitivity checks you performed (if any)

---

## Results
### Why it exists
Results deliver the evidence, clearly and without rhetorical inflation.

### How to write it
- Present results in the same order as your questions/hypotheses.
- For each result: **what was measured, in whom/what, under what conditions, with what uncertainty**.
- Prefer effect sizes and intervals over only “significance.”
- Use figures/tables for dense information; use text to guide interpretation of what the reader should notice.

Avoid:
- re-explaining Methods
- interpreting deeply (save for Discussion)
- selective reporting (“cherry-picking”)

A strong Results section is a well-lit room: nothing important is hidden in shadows.

---

## Discussion
### Why it exists
Discussion answers: “So what?” and “Why should we believe this?” while honestly stating limitations.

### How to write it (a productive sequence)
1. **Summary of key findings** (not a copy of Results)  
2. **Interpretation:** mechanisms, explanations, theory alignment  
3. **Comparison to prior work:** agreements, disagreements, reasons  
4. **Robustness:** sensitivity checks, assumptions, threats to validity  
5. **Limitations:** what you cannot claim and why  
6. **Implications:** for theory, practice, or future research  
7. **Next steps:** concrete and realistic directions

A hallmark of maturity is a Discussion that is both confident and careful:
- confident about what your evidence supports
- careful about what it does not

---

## Conclusion
### Why it exists
The Conclusion compresses the contribution into a durable form.

### How to write it
- Restate the contribution and main findings in plain terms.
- Emphasize scope (where it applies) and limits (where it might not).
- End with a forward-looking but grounded statement (future work, applications, open questions).

Avoid introducing new results.

---

## Acknowledgements, funding, and disclosures
### Why it exists
Research is social and financial. Transparency reduces hidden influence.

### How to write it
- Acknowledge technical help, feedback, resources.
- List funding sources.
- Declare conflicts of interest (financial, personal, institutional).

---

# Figures, tables, and visual evidence

## Philosophy: figures are arguments made visible
A good figure is not decoration. It is **compressed evidence**.

## General rules
- Every figure must answer a question: *What is the reader supposed to learn?*
- Make figures interpretable without the main text:
  - labeled axes with units
  - clear legends
  - defined abbreviations
  - captions that explain what, how, and key takeaway

## Captions: a useful structure
A strong caption often includes:
1. What is shown (data/model/conditions)
2. How it was produced (brief)
3. What the reader should notice (main pattern)

## Tables: when exact values matter
Use tables for:
- parameter values
- ablation results
- demographic breakdowns
- statistical model coefficients

Avoid tables for patterns better seen as plots.

## Integrity rules
- Do not manipulate axes or scales to mislead.
- Report exclusions and transformations.
- Maintain consistent scales across comparable plots when feasible.

---

# Citations, scholarship, and intellectual honesty

## Why we cite
Citations serve at least four functions:
1. **Credit** (intellectual honesty)
2. **Support** (evidence for claims)
3. **Context** (placing work in a lineage)
4. **Navigation** (helping readers find details)

## What to cite
Cite when you:
- use an idea, method, dataset, or tool not originally yours
- state a nontrivial fact not common knowledge in your audience
- compare to prior results
- use a specific definition or theoretical claim

## Good citation practice
- Prefer primary sources (original papers) when possible.
- Cite reviews for broad overviews, but do not replace primary citations with reviews.
- Avoid citation chains (“I cited a paper that cited the original”).
- Ensure citations actually support the claim you attach them to.

## Avoid “citation plagiarism”
Paraphrasing an author’s idea still requires citation. Changing wording does not change ownership of an idea.

---

# Methods, statistics, and reproducibility

## Reproducibility components
Depending on the field, reproducibility may require:
- data availability (or access procedure)
- code availability (or detailed pseudo-code)
- parameter/hyperparameter documentation
- random seeds and environment details
- full model specification
- preregistration (where appropriate)
- complete reporting of exclusions and missing data handling

## Statistics: reporting principles
- Report **effect sizes** and **uncertainty** (confidence/credible intervals where appropriate).
- Report **sample sizes** and how they were chosen (power analysis or rationale).
- Address **multiple comparisons** if you test many hypotheses.
- Distinguish **confirmatory** (hypothesis-driven) from **exploratory** analyses.
- Be explicit about **assumptions** (normality, independence, model fit).

## Robustness and sensitivity
Strong work often includes:
- alternative plausible model specifications
- ablation studies (what happens if you remove components?)
- checks for data leakage (ML)
- outlier and missingness sensitivity
- subgroup analyses (with caution and transparency)

---

# Style, clarity, and scientific tone

## The goal: precision with readability
Scientific prose should be:
- accurate
- explicit about uncertainty
- concise but not cryptic

## Preferred habits
- Define terms on first use.
- Use consistent terminology (do not rename the same concept repeatedly).
- Prefer active voice when it clarifies responsibility (“We measured…”).
- Use passive voice when the actor is irrelevant and method matters (“Samples were incubated…”).
- Keep sentences short when describing procedures or results.
- Put the main point early in the sentence; put details later.

## Hedging: the disciplined kind
Hedging is not weakness; it is accuracy calibration.
- Use “suggests” when evidence is indirect.
- Use “demonstrates” when evidence directly supports a claim under stated assumptions.
- Use “may” only when you can explain the mechanism or uncertainty.

## Numbers and symbols
- Define all symbols and variables.
- Provide units.
- Use consistent significant figures (reflecting measurement precision).

---

# Revision, feedback, and quality control

## Revision is not proofreading
There are different levels of revision:
1. **Argument revision:** Are you answering the right question with the right evidence?
2. **Structure revision:** Does the order match the reader’s logic?
3. **Paragraph revision:** Does each paragraph have one purpose?
4. **Sentence revision:** Are sentences clear and correct?
5. **Proofreading:** Typos, formatting, consistency

Do not start at level 5.

## Practical revision techniques
- **Reverse outline:** After drafting, write one sentence per paragraph describing its role. Remove or move paragraphs that do not serve the argument.
- **Reader simulation:** Give the paper to a colleague and ask them to summarize your contribution and main evidence. If they cannot, the paper is not yet clear.
- **Figure-first checking:** Can someone understand your results from figures and captions alone?

## Feedback etiquette (and effectiveness)
- Ask for specific feedback: “Is the contribution clear?” “Is the Methods replicable?” “Does Figure 2 support Claim A?”
- Accept that criticism is about the artifact, not your worth.

---

# Ethics, authorship, and responsible research

## Ethics is broader than approvals
Ethics includes:
- honest reporting
- respect for participants and communities
- avoidance of harm
- transparency about uncertainty and limitations
- proper attribution

## Authorship (general principles)
Authorship standards vary by field, but common expectations include:
- meaningful contribution to conception/design, execution, or interpretation
- participation in drafting or critical revision
- responsibility for integrity of the work

Discuss authorship early, revise as roles evolve, and document decisions.

## Data ethics
- Protect privacy and sensitive information.
- Follow institutional and legal requirements.
- Avoid “de-identification theater” (assuming removal of names is enough).
- Document consent and data governance rules.

---

# Submission, peer review, and responding to reviewers

## Submission strategy
- Match your paper to a venue’s scope and standards.
- Follow formatting and reporting requirements.
- Ensure figures, references, and supplemental materials meet specifications.

## Peer review: the correct mindset
Reviewers are not omniscient; they are constrained, skeptical readers.
Treat reviews as:
- a test of clarity
- a test of rigor
- a test of novelty and positioning

## Writing the response to reviewers
A strong response is:
- polite and concrete
- structured (point-by-point)
- transparent about changes (with locations)
- willing to concede and improve, but not to surrender logic

When you disagree:
- restate the reviewer’s concern fairly
- provide evidence or reasoning
- clarify the manuscript accordingly (often you can improve clarity even if the reviewer is “wrong”)

---

# Thesis-specific guidance

## The thesis is an apprenticeship certificate
A thesis demonstrates:
- technical competence
- independent thinking
- command of literature
- ability to plan and execute research
- ability to communicate it responsibly

## Thesis structure choices
If your thesis is long, it must be:
- navigable (clear chapter purposes, consistent notation)
- internally consistent (same definitions and assumptions)
- honest about what is original vs. background

## Working with a supervisor and committee
- Align expectations early: scope, chapter count, contribution level, deadlines.
- Treat meetings as design reviews: bring outlines, decisions, and open questions.
- Keep a “decision log” (methods choices, changes, rationales).

## The defense (where applicable)
A defense is an oral test of:
- your model of the problem
- your evidence and reasoning
- your awareness of limitations
- your ability to respond thoughtfully under pressure

Build a talk around:
- the question
- your approach
- 2–4 key results
- implications and limits

---

# Common failure modes and how to avoid them

## 1) “Everything is important”
**Symptom:** bloated introduction, unfocused results.  
**Fix:** choose one main contribution and subordinate everything else.

## 2) Methods too vague to reproduce
**Symptom:** missing parameter choices, unclear sampling, unknown preprocessing.  
**Fix:** write Methods as if a rival lab will try to replicate and critique it.

## 3) Results without uncertainty
**Symptom:** only point estimates and p-values.  
**Fix:** include uncertainty, effect sizes, and assumptions.

## 4) Discussion that overclaims
**Symptom:** causal language without causal design, generalization beyond data.  
**Fix:** explicitly state scope conditions and threats to validity.

## 5) Literature review as a list
**Symptom:** “Author A did X. Author B did Y.”  
**Fix:** organize by themes, debates, methods; compare and synthesize.

## 6) Figures that do not carry their weight
**Symptom:** unclear axes, missing units, captions that say nothing.  
**Fix:** treat each figure as a self-contained argument.

---

# Practical checklists

## Pre-writing checklist
- [ ] I can state the research question in one sentence.
- [ ] I can state the main contribution in one sentence.
- [ ] I know the target audience/venue.
- [ ] I have defined what counts as evidence and success.
- [ ] I have a minimal set of figures/tables that will carry the Results.

## Introduction checklist
- [ ] I explain why the topic matters (for this audience).
- [ ] I state the specific gap my work addresses.
- [ ] I position my work relative to key prior approaches.
- [ ] I state contributions explicitly.
- [ ] I provide a roadmap of the document.

## Methods checklist
- [ ] Design, data sources, and sample selection are explicit.
- [ ] All variables/metrics are operationally defined.
- [ ] Preprocessing and exclusions are documented.
- [ ] Statistical/modeling choices are justified and reproducible.
- [ ] Tools, versions, and key parameters are recorded.
- [ ] Ethical approvals/consent are stated if applicable.

## Results checklist
- [ ] Results correspond to the stated questions/hypotheses.
- [ ] Sample sizes are reported.
- [ ] Uncertainty is reported appropriately.
- [ ] Figures and tables are interpretable and referenced in text.
- [ ] Negative/null results are reported when relevant.

## Discussion checklist
- [ ] I summarize key findings accurately.
- [ ] I interpret results with appropriate caution.
- [ ] I compare to prior work fairly.
- [ ] I state limitations and threats to validity.
- [ ] I avoid claims that exceed my design/data.

## Final polish checklist
- [ ] Terminology is consistent.
- [ ] All symbols/abbreviations are defined.
- [ ] All claims that need citations have citations.
- [ ] References are complete and correctly formatted.
- [ ] Figures have units, readable text, and informative captions.
- [ ] The abstract reflects the actual findings.

---

# Mini-templates and phrase banks (use judiciously)

These are scaffolds, not substitutes for thinking.

## Contribution statements
- “This work makes three contributions: (1) ___, (2) ___, and (3) ___.”
- “We introduce ___ and show that it ___ compared with ___ on ___.”
- “We provide evidence that ___ by measuring ___ under ___.”

## Gap statements
- “However, existing studies have not resolved ___ because ___.”
- “Prior approaches are limited by ___, motivating ___.”

## Limitations
- “Our findings are limited to ___ because ___.”
- “A key assumption in our analysis is ___; violations of this assumption may lead to ___.”

## Responsible interpretation
- “These results suggest ___ under the conditions tested.”
- “An alternative explanation is ___; future work could distinguish these by ___.”

---

## Closing note: the quiet virtue of scientific writing
Scientific writing is an unusual craft because it demands two virtues at once:
- **Ambition** (to say something new and useful), and
- **Humility** (to say no more than the evidence warrants).

When those are in balance, the document becomes more than a report: it becomes a trustworthy piece of the shared machinery of knowledge.

---

# A Practical and Philosophical Guide to Writing a Thesis or Scientific Paper  
*Version 1.1 — Includes Deep Learning + Agentic AI annexes*

---

## How to use this document
This file is designed as both:
1) **A pedagogical guide** (it explains the *why* behind good scientific writing), and  
2) **A reference manual** (it provides actionable *how-to* steps, checklists, and templates).

Scientific writing is not merely “writing down what happened.” It is **the construction of a transparent, testable argument** that connects a question to evidence to inference—so that a skeptical, intelligent reader can decide whether to believe you, reproduce you, or build upon you.

Use it in three ways:
- **Before you write:** to design your argument and structure.
- **While you write:** to draft each section with correct purpose and content.
- **Before you submit:** to audit clarity, rigor, ethics, reproducibility, and presentation.

---

## Table of contents
1. [The philosophy of scientific writing](#the-philosophy-of-scientific-writing)  
2. [Core principles (the “laws of the land”)](#core-principles-the-laws-of-the-land)  
3. [From idea to paper: the research-to-writing pipeline](#from-idea-to-paper-the-research-to-writing-pipeline)  
4. [Planning the document: audience, contribution, and story](#planning-the-document-audience-contribution-and-story)  
5. [Standard structures (paper vs. thesis)](#standard-structures-paper-vs-thesis)  
6. [Section-by-section guide (with why + how)](#section-by-section-guide-with-why--how)  
7. [Figures, tables, and visual evidence](#figures-tables-and-visual-evidence)  
8. [Citations, scholarship, and intellectual honesty](#citations-scholarship-and-intellectual-honesty)  
9. [Methods, statistics, and reproducibility](#methods-statistics-and-reproducibility)  
10. [Style, clarity, and scientific tone](#style-clarity-and-scientific-tone)  
11. [Revision, feedback, and quality control](#revision-feedback-and-quality-control)  
12. [Ethics, authorship, and responsible research](#ethics-authorship-and-responsible-research)  
13. [Submission, peer review, and responding to reviewers](#submission-peer-review-and-responding-to-reviewers)  
14. [Thesis-specific guidance](#thesis-specific-guidance)  
15. [Common failure modes (and how to avoid them)](#common-failure-modes-and-how-to-avoid-them)  
16. [Practical checklists](#practical-checklists)  
17. [Mini-templates and phrase banks (use judiciously)](#mini-templates-and-phrase-banks-use-judiciously)  
18. [Annex A — Deep Learning: Truthful Experiments and Reproducible Systems](#annex-a--deep-learning-truthful-experiments-and-reproducible-systems)  
19. [Annex B — Agentic AI: Evaluating Systems Without Fooling Yourself](#annex-b--agentic-ai-evaluating-systems-without-fooling-yourself)  

---

# The philosophy of scientific writing

## Writing is part of the scientific method
Scientific knowledge is *public* knowledge. A result that cannot be understood, evaluated, or reproduced is not yet fully scientific. Writing is therefore not a cosmetic step after “real work” is done; it is a **core instrument of science**, comparable to measurement and analysis.

### The central philosophical commitment
Scientific writing should let a reader answer, with minimal guesswork:
- **What was asked?**  
- **What was done?**  
- **What was found?**  
- **Why should we believe it?**  
- **What does it mean—and what does it not mean?**

## The goal of good science: reliable knowledge that resists self-deception
If scientific writing is the public interface of science, then the goal of good science can be stated plainly:

**To produce reliable knowledge about the world, under uncertainty, in a way that other minds can audit.**

“Truth” in science is rarely a dramatic absolute. More often it is:
- a measurement with uncertainty,
- a model that predicts within a known regime,
- an explanation that survives attempts to falsify it,
- a result that remains stable when reasonable alternatives are tried.

Good science therefore aims to **minimize avoidable error** (bias, leakage, confounding, measurement artifacts, overfitting, cherry-picking) and to **maximize inspectability** (clear methods, transparent assumptions, complete reporting).

A practical test of whether you are doing good science is not “Does this sound convincing?” but:

- **Would I still believe this if I were trying to prove it wrong?**
- **Could a competent skeptic reproduce the result from my description?**
- **If the result is wrong, can the reader see where it might have gone wrong?**

Scientific writing operationalizes this goal by turning private work into a public, checkable chain of reasoning.

## The paper/thesis is an argument, not a diary
A scientific document is not a chronological record of your activities. It is a **structured argument** where every part serves a function in the reader’s reasoning.

A useful mental model:
- **Claim**: What you assert.
- **Evidence**: What you observed/measured/derived.
- **Warrant**: Why that evidence supports the claim (assumptions, theory, logic, statistics).
- **Scope**: Where it applies, and where it might not.

## Clarity is a form of ethics
Ambiguity wastes time, hides errors, and can mislead. In science, confusing writing is not harmless: it can distort interpretation and impair replication. Strive for writing that is **precise, modest in claims, and explicit about uncertainty**.

---

# Core principles (the “laws of the land”)

These principles apply across disciplines. Conventions differ, but the underlying logic is stable.

## 1) Reader-first design
**Why:** Your reader does not share your context. Your job is to reconstruct it efficiently.  
**How:** State the question early, define terms, and maintain a consistent thread from motivation → method → results → meaning.

## 2) One main contribution per paper (usually)
**Why:** A paper is evaluated as an integrated unit; too many contributions dilute the message and confuse reviewers.  
**How:** Write a one-sentence “contribution statement” and ensure every section supports it.

## 3) Reproducibility is not a slogan; it is documentation
**Why:** Science advances through verification and extension.  
**How:** Record data provenance, parameter choices, exclusions, preprocessing, and analysis decisions. Make the “path from raw to result” inspectable.

## 4) Truthfulness over persuasion (calibration as a virtue)
**Why:** Scientific documents can accidentally become sales pitches. Persuasion is not the purpose; accurate belief is.  
**How:** Make claims proportional to evidence, report uncertainty, disclose negative results when relevant, and separate measurement from interpretation. Prefer being correct and reproducible over being impressive and fragile.

## 5) Separate observation from interpretation
**Why:** Readers must distinguish what *happened* from what you *think it means*.  
**How:** In Results, describe; in Discussion, interpret. When you interpret, label it as interpretation and specify assumptions.

## 6) Precision beats grandeur
**Why:** Overclaiming is punished by reality (and reviewers).  
**How:** Prefer bounded statements (“in this dataset…”, “under these conditions…”, “suggests”) to universal proclamations.

## 7) Every number needs context
**Why:** Numbers are meaningless without units, uncertainty, and conditions.  
**How:** Provide units, sample sizes, variability/uncertainty (SD/SE/CI), and definitions of metrics.

## 8) Writing is iterative engineering
**Why:** Good papers are not written; they are rewritten.  
**How:** Draft quickly, revise structurally, then refine sentences. Do not attempt perfection in the first pass.

---

# From idea to paper: the research-to-writing pipeline

A robust pipeline reduces both errors and anxiety.

## Step A — Define the research question
A good question is:
- **Specific** (not “about X,” but “does X affect Y under conditions Z?”)
- **Answerable** with available methods and resources
- **Interesting** to a defined community
- **Situated** in existing work (you know what would count as “new”)

Deliverable: a 2–5 sentence statement:
1. Problem background  
2. Gap in knowledge  
3. Your question/hypothesis  
4. Your approach  
5. Your expected contribution

## Step B — Decide what counts as evidence
**Why:** Many projects fail at writing time because “evidence” was never defined.  
**How:** Decide:
- Primary outcome(s)
- Secondary outcome(s)
- Inclusion/exclusion criteria
- Baselines and comparisons
- Failure conditions (what would falsify your hypothesis?)

## Step C — Keep a research log that can become Methods
Maintain a living record:
- Instruments, software versions, parameters
- Data collection conditions
- Deviations from plan and why
- Cleaning steps
- Analysis scripts or workflows

This is not bureaucracy; it is future Methods text.

## Step D — Write earlier than you think
Drafting early reveals:
- missing controls
- unclear definitions
- weak measurements
- logic gaps

Writing is a diagnostic tool.

---

# Planning the document: audience, contribution, and story

## Identify your primary reader
Common “primary readers” include:
- A skeptical reviewer in your subfield
- A committee member outside your niche (thesis)
- An applied practitioner (engineering/clinical)
- A methods specialist (statistics/ML)

**How:** Write a 3-line “reader profile”:
- What they already know
- What they doubt
- What they need to see to be convinced

## Define your contribution in one sentence
Examples (generic forms):
- “We propose a method that ___ and demonstrate ___ on ___.”
- “We provide evidence that ___ by measuring ___ under ___.”
- “We resolve ___ by proving/deriving ___.”
- “We curate a dataset/tool that enables ___ and validate it by ___.”

If you cannot write this sentence, the paper is not ready to outline.

## Treat the document as a guided tour of reasoning
A scientific document answers a sequence of reader questions. If you satisfy these in order, the paper becomes easy to follow:
1. Why does this matter?
2. What exactly is unknown?
3. What is your approach?
4. What did you find?
5. Why should I believe it?
6. What does it imply?
7. What are the limits and next steps?

---

# Standard structures (paper vs. thesis)

## Typical scientific paper (IMRaD + framing)
- Title
- Abstract
- Introduction
- Methods
- Results
- Discussion
- Conclusion (sometimes merged with Discussion)
- References
- Appendices / Supplementary material

## Typical thesis (modular and explicit)
Two common thesis patterns:

### A) Monograph thesis
- Introduction / Background
- Literature Review (sometimes separate)
- Methods / Materials
- Results chapters
- Discussion
- Conclusion + Future Work
- Appendices (detailed methods, extra analyses, code/data notes)

### B) Paper-based thesis (thesis by publication)
- General introduction
- 2–4 manuscript-style chapters (published/submitted papers)
- Integrative discussion/conclusion tying them together
- Appendices

**Key difference:** A thesis must demonstrate *mastery, independence, and breadth*; a paper must demonstrate *a focused contribution*.

---

# Section-by-section guide (with why + how)

## Title
### Why it exists
The title is an indexing device and a promise: it tells readers whether this is relevant.

### How to write it
- Include the **core object** (method/system/phenomenon)
- Include the **action** (predicting, measuring, analyzing, improving)
- Include the **domain** (dataset, population, setting) when necessary

Avoid:
- vague words (“novel,” “improved,” “new”) without specifics
- unnecessary cleverness (memorable is good; ambiguous is not)

---

## Abstract
### Why it exists
The abstract is often the only part many readers will read. It must enable accurate triage and correct interpretation.

### How to write it (structured logic)
A strong abstract usually contains:
1. **Context** (1–2 sentences): the problem space  
2. **Gap** (1 sentence): what is missing/unknown  
3. **Approach** (1–2 sentences): what you did  
4. **Results** (1–3 sentences): key quantitative/qualitative findings  
5. **Meaning** (1 sentence): implications and scope  
6. **Limits** (optional, 1 sentence): important constraints

Common mistake: describing what you did but not what you found.

---

## Introduction
### Why it exists
The Introduction constructs the rationale and positions your work in the literature, culminating in a precise question and contribution.

### How to write it (a reliable arc)
A useful structure:
1. **Broad context:** why the area matters  
2. **Narrowed context:** what is specifically challenging/unknown  
3. **Literature map:** what has been tried and what remains unresolved  
4. **Gap statement:** the exact missing piece  
5. **Your approach:** what you do differently  
6. **Contributions:** explicit list or paragraph  
7. **Paper roadmap:** a short guide to the rest

A test of success:
- After reading the Introduction, a reader should be able to predict what Methods and Results will contain.

---

## Related Work / Literature Review
*(Sometimes part of Introduction; often its own chapter in a thesis.)*

### Why it exists
Science is cumulative. You must show:
- you understand the field
- you respect prior work
- your contribution is distinct
- your methods are appropriate

### How to do it well
Do not write a shopping list of citations. Instead:
- Organize by **ideas, approaches, or debates**, not by author chronology.
- Compare studies by: question, data, method, assumptions, findings, limitations.
- Highlight *why* existing results do not settle your question.

Include:
- foundational works (conceptual anchors)
- best current methods/results (state-of-the-art)
- closely adjacent approaches (to prevent “you missed X” reviews)

Thesis-specific guidance: the literature review often doubles as a *tutorial*. Teach the landscape, then locate your work.

---

## Methods (or Materials and Methods)
### Why it exists
Methods are the contract that enables reproduction and valid interpretation. They explain *how your evidence was produced*.

### How to write it
A Methods section should allow a competent researcher to:
- replicate your procedure, or
- implement an equivalent procedure, and
- understand why your choices are reasonable

Include, as applicable:
- Study design (experimental/observational/simulation/theoretical)
- Data sources and collection protocol
- Participants/samples/materials and inclusion/exclusion criteria
- Variables/features and operational definitions
- Instruments and calibration
- Preprocessing and quality control
- Statistical analysis plan (tests/models, assumptions, corrections)
- Software, versions, hardware (for computational work)
- Hyperparameters, training protocol, validation strategy (ML)
- Ethical approvals and consent (human/animal/field work)

#### Methods philosophy: expose degrees of freedom
Readers should see where choices could have been made differently:
- alternative preprocessing
- alternative model specifications
- selection criteria
- stopping rules
- outlier handling

When you made choices, state:
- what you did
- why you did it
- what sensitivity checks you performed (if any)

---

## Results
### Why it exists
Results deliver the evidence, clearly and without rhetorical inflation.

### How to write it
- Present results in the same order as your questions/hypotheses.
- For each result: **what was measured, in whom/what, under what conditions, with what uncertainty**.
- Prefer effect sizes and intervals over only “significance.”
- Use figures/tables for dense information; use text to guide interpretation of what the reader should notice.

Avoid:
- re-explaining Methods
- interpreting deeply (save for Discussion)
- selective reporting (“cherry-picking”)

A strong Results section is a well-lit room: nothing important is hidden in shadows.

---

## Discussion
### Why it exists
Discussion answers: “So what?” and “Why should we believe this?” while honestly stating limitations.

### How to write it (a productive sequence)
1. **Summary of key findings** (not a copy of Results)  
2. **Interpretation:** mechanisms, explanations, theory alignment  
3. **Comparison to prior work:** agreements, disagreements, reasons  
4. **Robustness:** sensitivity checks, assumptions, threats to validity  
5. **Limitations:** what you cannot claim and why  
6. **Implications:** for theory, practice, or future research  
7. **Next steps:** concrete and realistic directions

A hallmark of maturity is a Discussion that is both confident and careful:
- confident about what your evidence supports
- careful about what it does not

---

## Conclusion
### Why it exists
The Conclusion compresses the contribution into a durable form.

### How to write it
- Restate the contribution and main findings in plain terms.
- Emphasize scope (where it applies) and limits (where it might not).
- End with a forward-looking but grounded statement (future work, applications, open questions).

Avoid introducing new results.

---

## Acknowledgements, funding, and disclosures
### Why it exists
Research is social and financial. Transparency reduces hidden influence.

### How to write it
- Acknowledge technical help, feedback, resources.
- List funding sources.
- Declare conflicts of interest (financial, personal, institutional).

---

# Figures, tables, and visual evidence

## Philosophy: figures are arguments made visible
A good figure is not decoration. It is **compressed evidence**.

## General rules
- Every figure must answer a question: *What is the reader supposed to learn?*
- Make figures interpretable without the main text:
  - labeled axes with units
  - clear legends
  - defined abbreviations
  - captions that explain what, how, and key takeaway

## Captions: a useful structure
A strong caption often includes:
1. What is shown (data/model/conditions)
2. How it was produced (brief)
3. What the reader should notice (main pattern)

## Tables: when exact values matter
Use tables for:
- parameter values
- ablation results
- demographic breakdowns
- statistical model coefficients

Avoid tables for patterns better seen as plots.

## Integrity rules
- Do not manipulate axes or scales to mislead.
- Report exclusions and transformations.
- Maintain consistent scales across comparable plots when feasible.

---

# Citations, scholarship, and intellectual honesty

## Why we cite
Citations serve at least four functions:
1. **Credit** (intellectual honesty)
2. **Support** (evidence for claims)
3. **Context** (placing work in a lineage)
4. **Navigation** (helping readers find details)

## What to cite
Cite when you:
- use an idea, method, dataset, or tool not originally yours
- state a nontrivial fact not common knowledge in your audience
- compare to prior results
- use a specific definition or theoretical claim

## Good citation practice
- Prefer primary sources (original papers) when possible.
- Cite reviews for broad overviews, but do not replace primary citations with reviews.
- Avoid citation chains (“I cited a paper that cited the original”).
- Ensure citations actually support the claim you attach them to.

## Avoid “citation plagiarism”
Paraphrasing an author’s idea still requires citation. Changing wording does not change ownership of an idea.

---

# Methods, statistics, and reproducibility

## Reproducibility components
Depending on the field, reproducibility may require:
- data availability (or access procedure)
- code availability (or detailed pseudo-code)
- parameter/hyperparameter documentation
- random seeds and environment details
- full model specification
- preregistration (where appropriate)
- complete reporting of exclusions and missing data handling

## Statistics: reporting principles
- Report **effect sizes** and **uncertainty** (confidence/credible intervals where appropriate).
- Report **sample sizes** and how they were chosen (power analysis or rationale).
- Address **multiple comparisons** if you test many hypotheses.
- Distinguish **confirmatory** (hypothesis-driven) from **exploratory** analyses.
- Be explicit about **assumptions** (normality, independence, model fit).

## Robustness and sensitivity
Strong work often includes:
- alternative plausible model specifications
- ablation studies (what happens if you remove components?)
- checks for data leakage (ML)
- outlier and missingness sensitivity
- subgroup analyses (with caution and transparency)

---

# Style, clarity, and scientific tone

## The goal: precision with readability
Scientific prose should be:
- accurate
- explicit about uncertainty
- concise but not cryptic

## Preferred habits
- Define terms on first use.
- Use consistent terminology (do not rename the same concept repeatedly).
- Prefer active voice when it clarifies responsibility (“We measured…”).
- Use passive voice when the actor is irrelevant and method matters (“Samples were incubated…”).
- Keep sentences short when describing procedures or results.
- Put the main point early in the sentence; put details later.

## Hedging: the disciplined kind
Hedging is not weakness; it is accuracy calibration.
- Use “suggests” when evidence is indirect.
- Use “demonstrates” when evidence directly supports a claim under stated assumptions.
- Use “may” only when you can explain the mechanism or uncertainty.

## Numbers and symbols
- Define all symbols and variables.
- Provide units.
- Use consistent significant figures (reflecting measurement precision).

---

# Revision, feedback, and quality control

## Revision is not proofreading
There are different levels of revision:
1. **Argument revision:** Are you answering the right question with the right evidence?
2. **Structure revision:** Does the order match the reader’s logic?
3. **Paragraph revision:** Does each paragraph have one purpose?
4. **Sentence revision:** Are sentences clear and correct?
5. **Proofreading:** Typos, formatting, consistency

Do not start at level 5.

## Practical revision techniques
- **Reverse outline:** After drafting, write one sentence per paragraph describing its role. Remove or move paragraphs that do not serve the argument.
- **Reader simulation:** Give the paper to a colleague and ask them to summarize your contribution and main evidence. If they cannot, the paper is not yet clear.
- **Figure-first checking:** Can someone understand your results from figures and captions alone?

## Feedback etiquette (and effectiveness)
- Ask for specific feedback: “Is the contribution clear?” “Is the Methods replicable?” “Does Figure 2 support Claim A?”
- Accept that criticism is about the artifact, not your worth.

---

# Ethics, authorship, and responsible research

## Ethics is broader than approvals
Ethics includes:
- honest reporting
- respect for participants and communities
- avoidance of harm
- transparency about uncertainty and limitations
- proper attribution

## Authorship (general principles)
Authorship standards vary by field, but common expectations include:
- meaningful contribution to conception/design, execution, or interpretation
- participation in drafting or critical revision
- responsibility for integrity of the work

Discuss authorship early, revise as roles evolve, and document decisions.

## Data ethics
- Protect privacy and sensitive information.
- Follow institutional and legal requirements.
- Avoid “de-identification theater” (assuming removal of names is enough).
- Document consent and data governance rules.

---

# Submission, peer review, and responding to reviewers

## Submission strategy
- Match your paper to a venue’s scope and standards.
- Follow formatting and reporting requirements.
- Ensure figures, references, and supplemental materials meet specifications.

## Peer review: the correct mindset
Reviewers are not omniscient; they are constrained, skeptical readers.
Treat reviews as:
- a test of clarity
- a test of rigor
- a test of novelty and positioning

## Writing the response to reviewers
A strong response is:
- polite and concrete
- structured (point-by-point)
- transparent about changes (with locations)
- willing to concede and improve, but not to surrender logic

When you disagree:
- restate the reviewer’s concern fairly
- provide evidence or reasoning
- clarify the manuscript accordingly (often you can improve clarity even if the reviewer is “wrong”)

---

# Thesis-specific guidance

## The thesis is an apprenticeship certificate
A thesis demonstrates:
- technical competence
- independent thinking
- command of literature
- ability to plan and execute research
- ability to communicate it responsibly

## Thesis structure choices
If your thesis is long, it must be:
- navigable (clear chapter purposes, consistent notation)
- internally consistent (same definitions and assumptions)
- honest about what is original vs. background

## Working with a supervisor and committee
- Align expectations early: scope, chapter count, contribution level, deadlines.
- Treat meetings as design reviews: bring outlines, decisions, and open questions.
- Keep a “decision log” (methods choices, changes, rationales).

## The defense (where applicable)
A defense is an oral test of:
- your model of the problem
- your evidence and reasoning
- your awareness of limitations
- your ability to respond thoughtfully under pressure

Build a talk around:
- the question
- your approach
- 2–4 key results
- implications and limits

---

# Common failure modes and how to avoid them

## 1) “Everything is important”
**Symptom:** bloated introduction, unfocused results.  
**Fix:** choose one main contribution and subordinate everything else.

## 2) Methods too vague to reproduce
**Symptom:** missing parameter choices, unclear sampling, unknown preprocessing.  
**Fix:** write Methods as if a rival lab will try to replicate and critique it.

## 3) Results without uncertainty
**Symptom:** only point estimates and p-values.  
**Fix:** include uncertainty, effect sizes, and assumptions.

## 4) Discussion that overclaims
**Symptom:** causal language without causal design, generalization beyond data.  
**Fix:** explicitly state scope conditions and threats to validity.

## 5) Literature review as a list
**Symptom:** “Author A did X. Author B did Y.”  
**Fix:** organize by themes, debates, methods; compare and synthesize.

## 6) Figures that do not carry their weight
**Symptom:** unclear axes, missing units, captions that say nothing.  
**Fix:** treat each figure as a self-contained argument.

---

# Practical checklists

## Pre-writing checklist
- [ ] I can state the research question in one sentence.
- [ ] I can state the main contribution in one sentence.
- [ ] I know the target audience/venue.
- [ ] I have defined what counts as evidence and success.
- [ ] I have a minimal set of figures/tables that will carry the Results.

## Introduction checklist
- [ ] I explain why the topic matters (for this audience).
- [ ] I state the specific gap my work addresses.
- [ ] I position my work relative to key prior approaches.
- [ ] I state contributions explicitly.
- [ ] I provide a roadmap of the document.

## Methods checklist
- [ ] Design, data sources, and sample selection are explicit.
- [ ] All variables/metrics are operationally defined.
- [ ] Preprocessing and exclusions are documented.
- [ ] Statistical/modeling choices are justified and reproducible.
- [ ] Tools, versions, and key parameters are recorded.
- [ ] Ethical approvals/consent are stated if applicable.

## Results checklist
- [ ] Results correspond to the stated questions/hypotheses.
- [ ] Sample sizes are reported.
- [ ] Uncertainty is reported appropriately.
- [ ] Figures and tables are interpretable and referenced in text.
- [ ] Negative/null results are reported when relevant.

## Discussion checklist
- [ ] I summarize key findings accurately.
- [ ] I interpret results with appropriate caution.
- [ ] I compare to prior work fairly.
- [ ] I state limitations and threats to validity.
- [ ] I avoid claims that exceed my design/data.

## Final polish checklist
- [ ] Terminology is consistent.
- [ ] All symbols/abbreviations are defined.
- [ ] All claims that need citations have citations.
- [ ] References are complete and correctly formatted.
- [ ] Figures have units, readable text, and informative captions.
- [ ] The abstract reflects the actual findings.

---

# Mini-templates and phrase banks (use judiciously)

These are scaffolds, not substitutes for thinking.

## Contribution statements
- “This work makes three contributions: (1) ___, (2) ___, and (3) ___.”
- “We introduce ___ and show that it ___ compared with ___ on ___.”
- “We provide evidence that ___ by measuring ___ under ___.”

## Gap statements
- “However, existing studies have not resolved ___ because ___.”
- “Prior approaches are limited by ___, motivating ___.”

## Limitations
- “Our findings are limited to ___ because ___.”
- “A key assumption in our analysis is ___; violations of this assumption may lead to ___.”

## Responsible interpretation
- “These results suggest ___ under the conditions tested.”
- “An alternative explanation is ___; future work could distinguish these by ___.”

---

## Closing note: the quiet virtue of scientific writing
Scientific writing is an unusual craft because it demands two virtues at once:
- **Ambition** (to say something new and useful), and
- **Humility** (to say no more than the evidence warrants).

When those are in balance, the document becomes more than a report: it becomes a trustworthy piece of the shared machinery of knowledge.

---

# Annex A — Deep Learning: Truthful Experiments and Reproducible Systems

## A.0 Purpose and scope
This annex is for the moment when you are thinking:

> “I am implementing a deep learning system. How do I ensure my results are *truthful*—that they reflect real performance, not experimental accidents?”

Deep learning experiments are unusually prone to **self-deception by degrees of freedom**:
- data pipelines with hidden leakage,
- stochastic training and fragile improvements,
- hyperparameter tuning that quietly uses the test set,
- comparisons made unfair by mismatched compute or tuning effort,
- evaluation that differs subtly from real deployment.

The aim is not perfection. The aim is **honest, stable conclusions** that survive skepticism.

---

## A.1 State the claim you actually want to make (capability vs. system result)
Before you run anything, write one sentence:

- **Claim type 1 — Algorithmic/capability claim:**  
  “Under controlled conditions, method X improves metric Y relative to baseline B.”

- **Claim type 2 — System claim:**  
  “A complete pipeline (data + training + inference constraints) achieves Y in setting Z.”

These are different. If you do not separate them, you will misinterpret your own results.

---

## A.2 Experimental design: controls, baselines, and fairness
### A.2.1 Choose baselines you can defend
Your baseline should be:
- **competitive** (not a strawman),
- **properly tuned** (similar tuning budget),
- **documented** (exact configuration, versions).

A common methodological error is a “baseline that was not allowed to try.”

### A.2.2 Match budgets when comparing methods
Deep learning performance often scales strongly with:
- training steps,
- dataset size,
- augmentation strength,
- model size,
- compute.

Therefore, when you compare A vs. B, specify what is held constant:
- **fixed compute** (same FLOPs/steps/wall-clock), or
- **fixed model size**, or
- **fixed data**, or
- **fixed performance target** (and compare cost).

If you do not define the budget, “better” is ambiguous.

### A.2.3 Predefine your selection rule
Decide *before* running:
- What metric determines “best checkpoint”?
- On which split is that metric computed?
- What is the stopping rule (epochs, steps, early stopping)?
- How many runs will you do?

This prevents accidental “researcher degrees of freedom” from dominating conclusions.

---

## A.3 Data hygiene: leakage is the most common invalidator
Treat leakage as an adversary.

### A.3.1 Split at the correct unit
In many domains, naïve random splits leak identity or context:
- medical: split by **patient**, not image
- recommender systems: split by **user** (and often by time)
- time series: split by **time**, not random shuffle
- web data: de-duplicate across splits aggressively (near-duplicates matter)

### A.3.2 Keep the test set “dead”
A dead test set is:
- never used for model selection,
- never used for early stopping,
- never used to decide preprocessing variants,
- never used for threshold tuning.

If you look repeatedly at test performance while iterating, you are training on it—just slowly.

### A.3.3 Compute preprocessing statistics on train only
Common leakage pattern:
- normalization mean/std computed on full dataset,
- vocabulary/tokenizer built using test text,
- feature selection done using labels from all splits.

Rule: **fit transforms on train, apply to val/test.**

### A.3.4 Beware label leakage in feature engineering
If a feature is derived from anything correlated with labels due to collection procedures, you may be learning the procedure, not the phenomenon.

Ask: “Could the model succeed without learning the intended signal?”

---

## A.4 Training protocol: document the real procedure, not the idealized one
A deep learning Methods section should allow reproduction of the training run, not merely its general idea.

Minimum items to record:
- model architecture and initialization details
- optimizer + hyperparameters (including defaults you did not touch)
- learning rate schedule (exact form + warmup)
- batch size (global and per device)
- number of steps/epochs, gradient accumulation
- regularization: weight decay, dropout, label smoothing, augmentations
- mixed precision settings (if any)
- gradient clipping
- checkpoint selection rule
- random seeds (and what they seed)
- hardware and distributed settings (number of GPUs, strategy)
- library versions (framework, CUDA/cuDNN) where relevant

### A.4.1 Evaluation mode matters (a subtle but frequent bug)
When evaluating:
- ensure dropout is disabled,
- batch normalization uses appropriate running statistics,
- augmentations are disabled unless you explicitly do test-time augmentation,
- data shuffling is controlled.

Incorrect training/eval modes can silently invalidate comparisons.

---

## A.5 Hyperparameter tuning without contaminating conclusions
### A.5.1 Tuning budget should be described
Report:
- which hyperparameters were tuned,
- the search method (grid, random, Bayesian),
- the budget (trials, compute),
- the selection metric and split.

A paper that says “we tuned hyperparameters” without the budget is missing a methodological variable.

### A.5.2 Avoid “test-set tuning by impatience”
If you tried 20 variants and only report the one that does best on test, you have performed implicit multiple testing.

Safer patterns:
- use validation for all decisions,
- keep a final test evaluation for the end,
- consider a second validation set for late-stage iteration (especially in thesis-scale work).

---

## A.6 Stochasticity: you must measure it, not assume it away
Deep learning is noisy. A single run is often an anecdote.

### A.6.1 Minimum practice
- run multiple seeds (often ≥3; more if variance is high),
- report mean ± variability (and/or confidence intervals),
- state whether the reported number is mean, median, or best-of-k.

### A.6.2 Seed selection is a known pitfall
Anti-pattern:
- run many seeds silently and report the best.

If you do explore many seeds (for debugging or research), be explicit:
- how many seeds were run,
- what was reported and why.

---

## A.7 Ablations: attribute improvements correctly
Ablations answer: “Which component caused the gain?”

Good ablations:
- remove one component at a time,
- keep training budget fixed,
- re-tune minimally and symmetrically if necessary,
- report whether the component interacts with others.

Ablations that change multiple things at once are stories, not evidence.

---

## A.8 Evaluation: metrics, calibration, and robustness
### A.8.1 Use metrics aligned with the real objective
Accuracy is not always relevant. Consider:
- class imbalance (use F1, AUROC, AUPRC, balanced accuracy)
- ranking problems (NDCG, MAP)
- calibration (ECE, Brier score, reliability diagrams)
- cost-sensitive errors (weighted metrics)

### A.8.2 Thresholds must be chosen properly
If a classifier threshold is selected using test labels, the test set is no longer a test set.

Rule: choose thresholds on validation, then apply to test.

### A.8.3 Robustness checks (often cheap, highly informative)
- perturbation tests (noise, blur, compression)
- subgroup analyses (if ethically and statistically appropriate)
- out-of-distribution probes (clearly labeled as such)
- sanity checks (below)

---

## A.9 Sanity checks that catch surprising numbers of bugs
These are “truthfulness probes,” not optional niceties.

- **Overfit a tiny subset:** can the model reach near-perfect training performance on ~50–200 examples? If not, something is broken.
- **Label-shuffle test:** if you shuffle labels, performance should drop to chance.
- **Input ablation:** remove the signal you claim matters; performance should degrade.
- **Train/val agreement check:** if training improves but validation does not, investigate leakage, overfitting, or metric mismatch.
- **Baseline reproduction:** can you reproduce a known baseline number from literature or your own prior run?

---

## A.10 Reproducibility package: what “complete” looks like in practice
A strong reproducibility bundle often includes:
- a single command to run training (or a clear script pipeline)
- environment file/container specification
- fixed dataset versioning (hashes, manifest)
- config files for all experiments
- logs (including failed runs where relevant)
- evaluation scripts that regenerate tables/figures from checkpoints

Principle: a result is not fully scientific until the path from raw inputs to reported numbers is auditable.

---

## A.11 Common deep learning methodological failure modes (diagnostic list)
If any item below is true, treat results as provisional until fixed:

- Test set used for early stopping or model selection  
- Data preprocessing fitted on full dataset (including test)  
- Split performed at the wrong unit (identity/time leakage)  
- Baseline under-tuned relative to proposed method  
- Only best seed reported without disclosure  
- Hyperparameter search space not reported (or effectively unlimited)  
- Code changes mid-experiment without version control / run identifiers  
- Evaluation performed with augmentations enabled unintentionally  
- Model evaluated in training mode (dropout/BN issues)  
- Dataset contains duplicates across splits (exact or near-duplicate)  
- Metric chosen after looking at results (“metric shopping”)

---

## A.12 A minimal “truthful result” checklist (printable)
Before you believe your own number, verify:

- [ ] The claim is clearly stated and matches the metric  
- [ ] The test set was not used for any decision  
- [ ] Splits prevent identity/time leakage  
- [ ] Preprocessing was fit on train only  
- [ ] Baselines were tuned with comparable effort  
- [ ] Multiple seeds were run (or variance is otherwise justified)  
- [ ] Sanity checks pass (tiny overfit, label shuffle)  
- [ ] Exact configs, versions, and budgets are recorded  
- [ ] Figures/tables can be regenerated from logs/checkpoints  

---

# Annex B — Agentic AI: Evaluating Systems Without Fooling Yourself

## B.0 Why agentic AI is methodologically tricky
“Agentic AI” systems—LLMs or other policies that plan, use tools, call APIs, write code, browse, store memory, and act across multiple steps—introduce failure modes that standard model evaluation does not cover.

In agentic work, it is remarkably easy to:
- mistake *a demo* for *a result*,
- let the agent accidentally access the answer key,
- tune on the benchmark through prompt iteration,
- report non-reproducible success because the environment changed,
- use subjective LLM judges without reliability controls,
- create impressive behavior that is actually brittle or unsafe.

This annex provides pragmatic methodology to keep results truthful.

---

## B.1 Define the object of study: model vs. agent vs. system
Be explicit whether you are evaluating:
- **Base model capability:** what the model can do given a prompt.
- **Agent policy:** the decision logic across steps (planning, tool calls, memory usage).
- **Full system:** policy + tools + retrieval + environment + guardrails + budget constraints.

A system result (“works end-to-end”) cannot be attributed to a new planning algorithm unless you show ablations.

---

## B.2 Specify the environment as part of the Methods
Agent performance depends critically on environment details:
- tool set and tool interfaces (versions matter)
- availability of internet access (or sandboxed corpora)
- latency, timeouts, rate limits
- error handling
- reset behavior between episodes
- hidden state (caches, persistent files, memory store)

**Rule:** If the environment can change, your evaluation can drift. Document the environment like lab equipment.

---

## B.3 The “answer key” problem: prevent unintended information access
Agentic systems are uniquely prone to cheating (often unintentionally).

### B.3.1 Common leakage paths
- Retrieval corpus contains solutions or benchmark explanations  
- Tools allow searching within the benchmark repository  
- Internet access allows finding benchmark answers online  
- Memory stores accumulate test solutions across runs  
- Logs from previous runs are visible to the agent  
- Evaluation harness includes hints or ground truth in tool outputs  
- Prompt includes examples that overlap test tasks

### B.3.2 Practical containment rules
- Separate **development tasks** from **test tasks** strictly.
- Run evaluation in a sandbox where the agent cannot read:
  - test labels,
  - hidden unit tests (for coding tasks),
  - benchmark solution files,
  - grading scripts.
- Clear or version memory stores; do not let them silently persist across evaluation episodes unless that is explicitly the experimental condition.

---

## B.4 Success metrics must include cost and reliability
Agent evaluation should usually report at least:
- **Task success rate** (with clear success criteria)
- **Cost** (tokens, tool calls, wall-clock time, compute)
- **Reliability** (variance across runs/seeds)
- **Failure modes** (categories: tool error, planning error, hallucination, safety refusal, etc.)

A system that succeeds once but fails unpredictably is not robust. Treat reliability as a primary metric, not an afterthought.

---

## B.5 Non-determinism: evaluate over runs, not anecdotes
Agents are stochastic in multiple places:
- model sampling (temperature, top-p)
- tool/API nondeterminism (search results, web content changes)
- concurrency and timeouts

Minimum practice:
- fix seeds where possible (and state what is and is not seed-controlled)
- run multiple trials per task
- report distributions (not only best-case outcomes)

If the system is designed to be stochastic (e.g., exploration), your evaluation must measure expected performance and variance.

---

## B.6 Benchmark and task suite design: avoid building a “benchmark-shaped key”
### B.6.1 Dev/test separation is non-negotiable
Prompt iteration on a benchmark is training. It may be legitimate engineering, but it is not a clean scientific test unless you preserve an untouched test set.

Practical pattern:
- **Dev set:** used for prompt/system iteration  
- **Validation set:** used for choosing variants  
- **Test set:** used once for final reporting  

If you cannot afford three splits, at least enforce: *dev ≠ test*.

### B.6.2 Control difficulty and ambiguity
Agents often appear good on tasks that are underspecified. Define:
- what counts as success,
- what constitutes partial credit (if any),
- time/cost limits per episode,
- allowed tool usage.

Ambiguity is not inherently bad, but it must be acknowledged and handled consistently.

---

## B.7 Baselines for agentic systems (and how to make them fair)
Agent improvements are easy to exaggerate because you can compare to weak baselines.

Recommended baseline set (adapt to domain):
- **Direct LLM (no tools):** single-shot or few-shot prompt baseline  
- **LLM + retrieval (no multi-step planning):** isolates value of retrieval  
- **Tool-use without planning (fixed script):** isolates planning value  
- **Strong public agent baseline:** if available, configured fairly  
- **Oracle tools (optional, clearly labeled):** estimates upper bound

Fairness rules:
- similar budget constraints,
- similar tool access,
- comparable prompt tuning effort (or report tuning budgets explicitly).

---

## B.8 Ablations: treat prompts and scaffolding as code
In agentic systems, “prompt” is not just text; it is part of the algorithm.

Therefore:
- version control prompts and system messages
- ablate planning modules, memory, retrieval, tool subsets
- test sensitivity to prompt wording (robustness)
- report the exact prompt used (or a principled redaction if sensitive)

A system that only works with one magical incantation is fragile; fragility is a result, but it must be reported honestly.

---

## B.9 LLM-as-judge evaluation: use carefully or regret later
LLM judges can be useful, but they introduce bias and non-reproducibility.

If you use an LLM judge:
- define the rubric precisely (what counts as correct)
- keep judge prompts fixed and versioned
- assess judge reliability (agreement with humans on a subset)
- consider multiple judges or majority vote for stability
- avoid judging with the same model family you evaluate (conflict of interest in the measurement device)

When objective evaluation is possible (unit tests, exact matches, structured outputs), prefer it.

---

## B.10 Environment drift: “live web” is not a stable benchmark
If your agent uses the open internet:
- pages change,
- search rankings change,
- APIs change,
- content disappears.

That can be acceptable for a *system demonstration*, but it is unstable for scientific claims unless you:
- snapshot content,
- restrict to a fixed corpus,
- or treat the evaluation as time-stamped and non-comparable across dates.

Be explicit: *Is this a benchmark or a demo?* Both can be valuable, but they are different epistemic objects.

---

## B.11 Safety and security are part of methodological correctness
Agentic systems interact with tools and environments that can be adversarial.

### B.11.1 Prompt injection and tool-output attacks
Web pages or tool outputs can contain instructions that hijack behavior.
Methodological implication: an agent that “succeeds” by following malicious instructions may appear capable while being unsafe.

Mitigations (report them):
- tool output sanitization
- instruction hierarchy rules (system > developer > user > tool)
- restricted tool permissions
- sandboxing
- explicit refusal policies for unsafe actions

### B.11.2 Privilege boundaries
Do not evaluate agents in a way that grants them privileges a real deployment would not have (filesystem access, private keys, unrestricted network). That can inflate performance and mask risk.

---

## B.12 Logging and traceability: transcripts are your Methods section
For agentic systems, the experiment record is not only code and configs. It is also:
- full prompts
- action traces (tool calls, arguments, outputs)
- intermediate thoughts *if you log them* (optional; treat privacy carefully)
- final outputs
- evaluator outputs and scores

A result without traces is hard to audit. A trace without versioned configs is hard to reproduce. You want both.

---

## B.13 Common ways agentic experiments become invalid (a blunt list)
Treat your evaluation as compromised if any of the following occurred without disclosure and correction:

- Agent can access benchmark answers via retrieval or web  
- Prompt/examples overlap with test tasks  
- Test set used repeatedly during iteration (“prompt tuning on test”)  
- Memory persists across test episodes unintentionally  
- Evaluation environment not reset properly between runs  
- Tool behavior changes across runs (API versions, content drift)  
- Success criteria are vague or inconsistently applied  
- LLM judge used without reliability checks  
- Only cherry-picked demos shown while failure rate is hidden  
- Budget constraints not enforced (unbounded retries/tool calls)  
- Human interventions occur mid-run and are not reported  

---

## B.14 A minimal “truthful agent evaluation” checklist (printable)
Before you trust your agent results:

- [ ] The evaluated object is defined (model vs agent vs system)  
- [ ] Tools, environment, and budgets are documented and versioned  
- [ ] Dev/val/test separation is enforced  
- [ ] The agent cannot access answers (no leakage paths)  
- [ ] Evaluation includes success + cost + reliability  
- [ ] Multiple trials per task are run (stochasticity measured)  
- [ ] Baselines are competitive and tuned fairly  
- [ ] Ablations isolate which components matter  
- [ ] Judging is objective when possible; LLM judges are validated if used  
- [ ] Full traces are logged for auditability  

---
