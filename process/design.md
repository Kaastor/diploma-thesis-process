## The design principle: Treat the thesis like a chain of decisions, not a pile of text

A good engineering thesis is a sequence:

1. **Problem framing** → 2) **Scope choices** → 3) **Method choices** → 4) **Implementation & data** → 5) **Analysis** → 6) **Claims**

Your “verification guardlines” should make each link:

* **Explicit** (written down),
* **Justified** (why this, not that),
* **Traceable** (claim → evidence → code/data → assumptions),
* **Reproducible** (someone else can rerun it),
* **Defendable orally** (student can explain without AI).

If you structure the process around those properties, AI becomes fine—because every AI-assisted output must pass the same epistemic tests.

---

## The Thesis Process (Stage-Gate + Audit Trail)

Think of this as an engineering design review pipeline: Concept Review → Plan Review → Implementation Review → Results Review → Defense Readiness.

### Gate 0 — AI Working Agreement (1–2 pages)

**Goal:** Define *allowed use*, *required disclosure*, and *verification expectations*.

**Student delivers:**

* **AI Use Statement**: tools allowed, what for (e.g., grammar, brainstorming, code suggestions), and what is prohibited (e.g., unverified citations, fabricated experiments).
* **Verification pledge**: “I am accountable for correctness. AI outputs are treated as suggestions until verified.”
* **Logging rule** (lightweight): keep a running “AI & Decision Log” (more below).

**Your verification guardline:**

* If it can’t be verified independently, it can’t go into the thesis.

---

### Gate 1 — Thesis Charter (Scope Lock v1)

**Goal:** Force clarity early, before “AI makes everything look easy.”

**Student delivers (2–4 pages):**

1. **Problem statement** in one paragraph (what’s broken / unknown).
2. **Research question(s)**: specific, testable, engineering-relevant.
3. **Minimum Viable Thesis (MVT)**: the smallest version that would still be a thesis.
4. **Scope box**:

   * In-scope items (bulleted, measurable)
   * Out-of-scope items (equally explicit)
   * Constraints (time, compute, data access, ethics)
5. **Success criteria**: what counts as “done” (metrics, accuracy, cost, latency, etc.).
6. **Primary risks**: what could invalidate results.

**Allowed AI use:** brainstorming alternative scopes, rewording, listing risks—fine.

**Verification guardlines (you can check quickly):**

* Can the student explain why the scope is *this size* and not 2× bigger?
* Do success criteria map cleanly to the research question?
* Is there an explicit “out-of-scope” list (this prevents scope creep disguised as productivity)?

**A killer supervisor prompt here:**

> “If you had half the time, what would you cut first—and why is that the least damaging cut scientifically?”

If they can answer crisply, they’re thinking. If they waffle, AI wrote it.

---

### Gate 2 — Literature Map + Claim Taxonomy (Reality Check)

**Goal:** Prevent AI-generated “literature vibes” and force real grounding.

**Student delivers:**

* **Literature map** (1 page): 8–15 key sources, grouped by theme, with 1–2 sentence summaries in the student’s words.
* **Gap statement**: what exactly is missing.
* **Claim taxonomy draft**: what types of claims will the thesis make?

  * Empirical performance claim?
  * Theoretical derivation?
  * System design claim?
  * Usability claim?
  * Cost/efficiency claim?

**Verification guardlines:**

* **Source audit:** pick 2 random papers and ask:

  * “What is the dataset/setup?”
  * “What is the main limitation?”
  * “Which figure matters and why?”
* If they can’t answer without reading, they didn’t digest it.

**AI-specific rule that saves lives:**

* **No citation enters the thesis unless the student opened the PDF and extracted the relevant point.**
  (AI is notoriously good at confident fake citations and mangled attributions.)

---

### Gate 3 — Methodology & Pre-Registration (Plan Lock)

**Goal:** Make methodology a *commitment* before results tempt them to rationalize.

This is the single biggest “scientific approach” upgrade you can make.

**Student delivers (the “protocol”):**

1. **Hypothesis / design objective**
2. **Variables**

   * Inputs, outputs, confounders
3. **Data plan**

   * Data source, inclusion/exclusion, splits, leakage prevention
4. **Baseline(s)**

   * What is the simplest/standard method to beat?
5. **Evaluation metrics**

   * And why they match the real engineering objective
6. **Experimental design**

   * Ablations (remove pieces to see what matters)
   * Sensitivity tests (hyperparameters, noise, environment)
   * Statistical plan (if relevant): repeats, confidence intervals, tests
7. **Stopping rule**

   * When do we conclude it works/doesn’t?
8. **Threats to validity table**

   * Internal / external / construct / conclusion validity (simple table is enough)

**Allowed AI use:** generate candidate ablations or threats-to-validity *lists*—but student must choose and justify.

**Verification guardlines (high signal):**

* Ask the student to predict outcomes *before running anything*:

  > “Which ablation do you think will hurt most, and why?”
* Ask:

  > “What result would *falsify* your hypothesis?”
  > If they can’t articulate falsification, they’re not doing science; they’re doing demo-building.

---

### Gate 4 — Implementation Review (Reproducibility Lock)

**Goal:** Prevent “it worked on my machine” and ensure charts aren’t decorative.

**Student delivers:**

* **Repo with version control** (Git).
* **Reproducible run script**: one command to regenerate key results (or as close as practical).
* **Environment spec**: requirements file / container / lockfile.
* **Data provenance**: where data came from, hashes/checksums if possible.
* **Unit tests or sanity checks** appropriate to the domain:

  * Basic invariants, boundary conditions, known-case tests.
* **Figure provenance** for every plot:

  * Script path + commit hash + data version + parameters.

**Verification guardlines:**

* Do a **live rerun** of one figure in a meeting (even a small one).
* Do a **code walkthrough** where they explain:

  * inputs/outputs,
  * key functions,
  * where randomness enters,
  * how evaluation is computed.
    If they can’t narrate the pipeline, they don’t own it.

**AI use note:** AI-written code is fine **if the student can explain every part that matters** and can diagnose bugs. Engineers ship systems; they don’t ship vibes.

---

### Gate 5 — Results Review (Claim-to-Evidence Audit)

**Goal:** Turn results into defensible knowledge, not a chart gallery.

**Student delivers:**

* A **Claim–Evidence–Reasoning (CER) table** (this is pure gold for supervision):

For each major claim:

* **Claim:** one sentence
* **Evidence:** which experiments/figures/tables support it
* **Reasoning:** why that evidence supports the claim (assumptions explicit)
* **Uncertainty:** limitations, error bars, sensitivity
* **Alternative explanations:** at least one plausible rival
* **What would change my mind:** the falsifier

**Verification guardlines:**

* Pick one claim and ask them to trace it end-to-end:

  > “Show me the raw measurement → transformation → metric → plot → conclusion.”
* Ask for **negative results**:

  > “What didn’t work, and what did you learn from it?”
  > If everything worked, something is fishy—or the thesis is too shallow.

**AI as a tool here (great use):**

* Have the student ask AI to generate the **strongest critique** of their own results.
  Then the student must write a rebuttal with actual evidence.
  This trains scientific toughness.

---

### Gate 6 — Writing & Defense Readiness (Oral Ownership)

**Goal:** Ensure the student owns the thesis intellectually.

**Student delivers:**

* Final thesis with:

  * **Methods written like a recipe** someone else could follow
  * **Limitations section** that doesn’t read like legal boilerplate
  * **AI disclosure appendix**: tools used + where + how verified

**Verification guardlines:**

* **Micro-vivas** (short oral defenses) at each chapter boundary:

  * “Explain this figure without reading.”
  * “Define the metric and why it matters.”
  * “What assumption is most fragile?”
  * “If I change X, what happens to Y?”

This is not adversarial; it’s the educational equivalent of a wind tunnel.

---

## The “AI & Decision Log” (lightweight, but powerful)

Make students maintain a single living document with two columns:

1. **Decision / Output**
2. **Justification & Verification**

Examples:

* “Chose train/test split method” → cite reason + leakage check performed
* “Used AI-generated code for preprocessing” → what tests confirmed correctness
* “AI suggested metric F1; chose AUROC instead” → why

This is your window into their thinking without micromanaging.

---

## Weekly cadence that trains scientific thinking (without drowning you)

Have the student send a **1-page Weekly Scientific Memo** before each meeting:

* This week’s question
* What I did (max 5 bullets)
* What I observed (with 1 key figure/table)
* Interpretation (what I think it means)
* What I will do next week
* Top risk / uncertainty
* AI use summary: where it helped + what was verified

**Your meeting becomes a review of reasoning**, not a tour of outputs.

---

## Practical “verification guardlines” you can apply anytime

These are the supervisor’s equivalent of unit tests.

### 1) The “Explain it on a whiteboard” rule

If they can’t explain:

* the method,
* the metric,
* the pipeline,
* the source of improvement,
  then AI did the work and they didn’t learn.

### 2) The “Two baselines minimum” rule

Every performance claim must beat:

* a naive baseline (simple heuristic),
* a standard baseline (common method).
  Otherwise, improvement is meaningless.

### 3) The “Ablation or it didn’t happen” rule

If a system has multiple parts, require:

* remove one part at a time,
* quantify impact.
  This prevents “complexity cosplay.”

### 4) The “One figure, one command” rule

Every key figure must be reproducible from code with documented inputs.

### 5) The “Rival hypothesis” rule

For each conclusion, student must name:

* at least one alternative explanation,
* one test that would distinguish them.

### 6) The “Citations are hand-carried” rule

No AI-invented citations. Student must open sources.

---

## How AI fits, explicitly: the “Junior Engineer” model

I’d teach students to treat AI like a very fast junior engineer:

* Great at drafts, boilerplate, suggesting options.
* Terrible at truth, careful methodology, and knowing what matters.
* Needs supervision, tests, and code review.

So your process should reward:

* asking better questions,
* designing better tests,
* interpreting results honestly,
* documenting assumptions,
  not producing more pages.

---

## What you’ll get if you run this process

* Students still use AI (because of course they will).
* But they learn the real skill: **epistemic engineering**—building systems of belief that resist self-deception.
* You can verify thinking via:

  * stage-gates,
  * CER tables,
  * live reruns,
  * oral ownership checks,
  * decision logs.

And the thesis becomes what it should be: not a fancy document, but a **compressed record of good judgment under constraints**.

---

If you want to push this even further, the next upgrade is to formalize a **replication check**: another student (or you, briefly) reruns one key result from scratch using the repo and protocol. In engineering terms: the thesis passes CI. Debugging reality is the curriculum.