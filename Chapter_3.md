# Chapter 3: Appraising Sources — Citations and Syntheses

## Introduction

You've asked a clear clinical question (Chapter 1). You understand how infrastructure has changed and what clinical expertise requires (Chapter 2). Now the AI has given you an answer with citations to studies, guidelines, meta-analyses, or its own synthesis.

Here's the critical step: **Before you use this answer clinically, you need to appraise what the AI cites.**

This is not the same as old-fashioned critical appraisal. When you appraise sources in the AI era, you're evaluating:

1. **Individual studies the AI cites** — Was the study well-done? Are the findings accurate? Does it apply to your patient?
    
2. **Meta-analyses the AI cites** — Did they include relevant studies? Were studies weighted appropriately? Is the conclusion supported by the data?
    
3. **Guidelines the AI cites** — Who made it? What's the evidence base? Are there caveats the AI missed?
    
4. **Syntheses the AI creates itself** — Did the AI correctly synthesize the studies it cites? Did it weight them appropriately? Did it miss important disagreement between studies?
    

The last one is crucial: **The AI is making synthesis decisions, and you need to verify those decisions.** The AI might cite five studies correctly but synthesize them poorly—weighting one too heavily or presenting disagreements as consensus.

The AI can be wrong in two ways:

- The sources it cites might be inaccurate or misrepresented
- The synthesis might be wrong even if the individual sources are correct

Both need verification. This chapter teaches you how.

---

## Part 1: Understanding Evidence Quality

Before you can appraise what the AI cites, you need to understand how to evaluate evidence quality. This section covers the fundamental concepts.

### Study Design and Critical Appraisal

When appraising evidence, design matters—but not in the way traditional hierarchies suggest.

Early evidence-based medicine popularized strict hierarchies: RCTs at the top, observational studies below, case reports at the bottom. This was useful historically. It corrected uncritical reliance on pathophysiology and case series. It gave clinicians a simple rule: if an RCT exists, prioritize it.

But hierarchies are too blunt. They treat the label of a study design as if it conveyed credibility. In practice:

**RCTs vary widely**: Some are underpowered, use surrogate outcomes, recruit highly selected patients, or apply interventions that bear little resemblance to routine practice. A poorly executed RCT can be less useful than a carefully designed observational study.

**Observational studies have strengths RCTs don't**: Some observational and quasi-experimental studies use rich data, careful design, and address questions that RCTs cannot feasibly or ethically touch—such as long-term harms, rare adverse events, or system-level effects.

The problem is not that hierarchies recognize the strength of randomization. It's that they encourage thinking to stop too early. Design labels become proxies for validity instead of prompts to ask deeper questions. A trial is treated as "good" because it is randomized; an observational study is treated as "weak" because it is not. This obscures diversity within each category and discourages nuanced appraisal.

**Better approach**: Instead of asking "What box does this study fit into?" ask "Given its design and execution, what can this study credibly tell us, and what can it not?"

RCTs still deserve a privileged role in assessing treatments, but not because hierarchies say so—because of what they tend to achieve in practice: they isolate the causal effect of an intervention by controlling for confounding through randomization.

Observational, economic, and pragmatic studies still deserve scrutiny, but not automatic dismissal. Each study type has strengths and limitations that require careful evaluation, not categorical judgment.

The task in appraisal is not to consult a hierarchy. It's to understand what the study actually did, how well it did it, and what that means for your specific question.

### Randomized Controlled Trials: Evaluating Quality

When the AI cites an RCT, ask these questions to assess if it's a good study:

**1. Was the study question clearly addressed?**

- Is the research question clearly stated?
- Are the population, intervention, comparator, and outcome clearly defined?
- Does the study actually address what the AI claims it does?

**2. Was the assignment to treatment groups truly random?**

- Random assignment minimizes selection bias
- Look for: computer-generated randomization, sequence concealment
- Red flags: "alternating assignment," "by birth date," "by hospital record number"

**3. Were patients and providers blinded?**

- Blinding minimizes performance and detection bias
- Patients don't know if they got treatment or placebo (patient blinding)
- Providers don't know who got treatment (provider blinding)
- For some interventions, blinding is impossible (e.g., surgery) but should still attempt outcome assessment blinding
- Red flags: Open-label studies (no blinding) are more prone to bias

**4. Were groups treated equally apart from the intervention?**

- Everything except the intervention should be the same between groups
- Different care, different monitoring, different follow-up introduces bias
- Red flags: Different hospitals, different providers, different protocols between groups

**5. Were all patients accounted for?**

- What percentage completed the study?
- Did some drop out? Were they accounted for in analysis?
- How many were lost to follow-up?
- Rule of thumb: >80% follow-up is generally acceptable; <70% raises concerns
- Intention-to-treat analysis: Did they analyze patients in the group they were randomized to, even if they didn't complete the intervention?

**6. Were the groups similar at the start?**

- Baseline characteristics should be balanced between groups
- If they're not balanced, ask: Did the study control for differences statistically?
- Table 1 in most papers shows baseline characteristics

**7. Was the sample size adequate?**

- Was the study large enough to detect a clinically meaningful difference?
- Small studies can miss real effects (underpowered)
- Very large studies can show statistical significance for clinically small effects
- Look for: sample size calculation, power statement

**8. What was the magnitude of effect?**

- How big was the difference between groups?
- Small effects in large studies may not be clinically meaningful
- This is where NNT and confidence intervals matter (see below)

### Cohort and Case-Control Studies

When the AI cites an observational study, remember: **These studies are prone to confounding.** An observed association might be caused by a third variable, not the exposure itself.

**Example**: Studies show hormone therapy users have lower heart disease risk. But users were healthier, more educated, higher socioeconomic status to begin with. When you adjust for these confounders, the benefit disappears.

**Questions to ask:**

- What confounders were identified?
- Were confounders measured?
- Were confounders controlled for in the analysis?
- Are there unmeasured confounders that could explain the results?
- How was the study population selected? Could selection bias explain results?

### Systematic Reviews and Meta-analyses

When the AI cites a meta-analysis or systematic review, different questions apply:

**1. Was the search comprehensive?**

- Did they search multiple databases (PubMed, Cochrane, Embase)?
- Did they search for unpublished studies?
- Did they have clear inclusion/exclusion criteria?
- Red flags: Single database only, no mention of search strategy, vague inclusion criteria

**2. Were studies of adequate quality included?**

- Did they assess quality of included studies?
- Did they exclude low-quality studies, or include everything?
- Look for: quality assessment tool used (GRADE, Cochrane Risk of Bias tool)

**3. Is the pooling appropriate?**

- Were studies similar enough to combine?
- If they differ in population, intervention, or outcome, combining may not make sense
- Look for: heterogeneity assessment (I² statistic)

**4. Was heterogeneity addressed?**

- Heterogeneity means studies don't all point in the same direction
- High heterogeneity (I² >50%) means results vary substantially
- When heterogeneity is high, pooling all studies may hide important differences
- Red flags: High I² with no discussion, pooling despite high heterogeneity

**5. What does the forest plot show?**

- Look at the actual data visualization
- Do confidence intervals overlap? Do they all point the same direction?
- One large study vs. many small studies can affect interpretation
- Red flags: Studies pointing different directions but conclusion is definitive

**6. Is publication bias assessed?**

- Published studies tend to show positive results (publication bias)
- Small studies with negative results often aren't published
- Funnel plots can show publication bias
- Red flags: Clear funnel plot asymmetry not discussed, no discussion of publication bias

**7. Does the conclusion match the data?**

- Does what they concluded actually match what the forest plot shows?
- Red flags: "Evidence supports X" when studies are mixed, "clear benefit" when heterogeneity is high

---

## Part 2: Understanding Effect Size and Statistical Precision

When you appraise evidence, you need to understand what the numbers actually mean. The AI might cite a study showing a "significant" effect, but that might not mean the effect is clinically meaningful.

### Relative Risk and Absolute Risk

These are two different ways to describe the same effect, and they can look very different.

**Relative Risk (RR)**: How much does the risk change compared to the baseline?

Example: A study shows treatment reduces disease risk from 4% to 2%. That's a 50% relative risk reduction (4% down to 2% is half, so 50% reduction).

But the absolute risk reduction is only 2% (4% - 2% = 2%).

**This matters**: A 50% relative risk reduction sounds impressive. But a 2% absolute risk reduction might not be clinically meaningful.

**Rule of thumb**: Always ask for absolute risk reduction, not just relative risk.

**NNT (Number Needed to Treat)**: How many patients do you need to treat to prevent one bad outcome?

NNT = 1 / Absolute Risk Reduction

If absolute risk reduction is 2%, then NNT = 1/0.02 = 50. You need to treat 50 patients to prevent 1 case of disease.

Is an NNT of 50 good? That depends on:

- How bad is the outcome? (preventing death is worth higher NNT than preventing mild headache)
- What are the harms of treatment? (if treatment is safe, higher NNT is acceptable)
- What are the costs? (if treatment is cheap, higher NNT is acceptable)

**The AI might cite a study and conclude "treatment is effective."** You need to ask: "What's the NNT? Is that clinically meaningful?"

### Confidence Intervals

A confidence interval (CI) shows the range of uncertainty around the estimate. Per Doug Altman,
	A strictly correct definition of a 95% CI is, somewhat opaquely, that 95% of such intervals will contain the true population value. Little is lost by the less pure interpretation of the CI as the range of values within which we can be 95% sure that the population value lies.

If a study shows NNT = 50 with a 95% CI of 25 to 200, that means:

- The true value could reasonably be anywhere from 25 to 200

**What this means**:

- Narrow CI = precise estimate, probably reliable
- Wide CI = imprecise estimate, less reliable
- CI crossing 1.0 (for risk ratios) or 0 (for differences) = result not statistically significant

**Red flags when appraising**:

- Study shows a "significant" effect, but confidence interval is very wide
- Small study with small numbers → wide confidence interval → imprecise estimate
- Study shows effect, but confidence interval includes the null value

### P-values and Statistical Significance

A p-value tells you the probability of seeing the result (or more extreme) if there's actually no effect.

- p < 0.05 usually means "statistically significant" (less than 5% chance of seeing this by random variation)
- But "statistically significant" ≠ "clinically important"

**Example**: A huge study of a tiny effect might show p < 0.05, but the effect size is so small it doesn't matter clinically.

**Red flag**: AI cites a study as "showing effect" based on p < 0.05, but effect size is tiny or confidence interval is wide.

### Absolute vs. Relative Numbers

Always convert to absolute numbers to understand clinical importance.

**Example from AI**: "Treatment reduces risk by 50%"

**What you should ask**:

- Risk of what? (outcome)
- Reduced from what baseline? (2%? 50%?)
- What's the absolute reduction? (Is it 1% or 30%?)
- What's the NNT?

---

## Part 3: Citation Appraisal — Verifying Individual Sources

Now that you understand how to evaluate evidence quality, let's apply the three approaches from Chapter 2.

### Step 1: Verify the Citation Exists

The first defense against AI hallucination is simple: **Try to find the source.**

**For a journal article:**

- Author names
- Year of publication
- Journal name
- Title (if you can remember it)
- PubMed ID if available

Go to PubMed, Google Scholar, or your institutional library and search for it.

**Red flags that a citation might be hallucinated:**

- You can't find it despite a thorough search
- The journal exists, but the article doesn't
- The authors are real, but they didn't publish on this topic
- The year seems off (published before the topic existed, or after the author died)
- The citation format is wrong (impossible page numbers, wrong journal for that time period)

**Real example of AI hallucination:** An AI suggested a specific meta-analysis titled "SGLT2 Inhibitors and CKD Progression: A Systematic Review." The citation looked real. But when searched, it didn't exist. The AI had invented it, though it cited real authors and a real journal.

**How to search effectively:**

- Start with author + year (most specific)
- If that fails, try title keywords + author
- If that fails, try journal + year + keywords
- If it still doesn't exist, it's probably hallucinated

**What to do if you can't find it:**

- Ask the AI: "I can't find this citation. Can you double-check?" (AI may "hallucinate" a correction)
- Ask a colleague
- Contact your medical librarian
- Mark it as unverified and look for alternative evidence

### Step 2: Read the Actual Source

Once you've confirmed the source exists, you need to read it. Not the abstract. Not the AI's summary. **Read the actual thing.**

For a journal article, read at least:

- The methods (how was this study done?)
- The results (what did they actually find?)
- The discussion (what do the authors think it means?)
- The limitations (what does the study acknowledge it didn't address?)

For a guideline, read:

- The recommendation itself
- The evidence base cited
- Any caveats or exceptions
- When it was published (is it current?)

For a meta-analysis, read:

- Which studies were included
- How were they weighted
- Was there heterogeneity (did studies disagree?)
- What does the forest plot show
- Did authors address quality and publication bias

### Step 3: Assess Study Quality

Using the frameworks from Part 1, evaluate:

**For an RCT:**

- Was randomization adequate?
- Were patients and providers blinded?
- How many completed the study?
- Were groups similar at baseline?
- Was sample size adequate?
- What was the magnitude of effect and confidence interval?

**For an observational study:**

- What confounders were measured?
- Were confounders controlled for?
- What unmeasured confounders might explain the results?
- How was the study population selected?

**For a systematic review:**

- Was search comprehensive?
- Were included studies of adequate quality?
- Is heterogeneity present and explained?
- Does conclusion match the data?

### Step 4: Evaluate Applicability to Your Patient

Even a high-quality study might not apply to your patient.

**Questions to ask:**

- What population was studied? How similar is your patient?
- What was the follow-up time? Is your patient's timeframe similar?
- What was the baseline risk? Is your patient at similar risk?
- What intervention was tested? Is it the same as what you're considering?
- What outcome was measured? Is it the one you care about?

**Example:** A trial of SGLT2i in CKD studied patients with eGFR 20-90. Your patient has eGFR 15. The study population doesn't include patients with eGFR <20, so the evidence may not directly apply.

### Step 5: Compare What You Read to What the AI Said

Now compare the actual source to what the AI claimed:

**Did the AI represent it accurately?**

- Does the claim match what the paper actually found?
- Did the AI leave out important limitations?
- Did the AI leave out important qualifications in a guideline?
- Did the AI misrepresent the effect size?
- Did the AI oversimplify nuance?

**Real example of AI misrepresentation:** An AI recommended "SGLT2i for all CKD patients with diabetes" based on a guideline it cited. When you read the actual guideline, it said: "Consider SGLT2i for CKD stage 3-4 with T2DM, especially if albuminuria present. Use caution in stage 3a. Not recommended for ESRD."

The AI's claim was much broader than what the guideline actually said. It left out the stages, the qualifications, and the caution. The guideline's recommendation was nuanced; the AI's was absolute.

**Red flags that the AI misrepresented a source:**

- The AI says "Studies show X works" but the paper says "In this population, X had modest benefits"
- The AI says a guideline "recommends X" but the guideline says "Consider X"
- The AI cites a meta-analysis but the forest plot shows high heterogeneity that the AI didn't mention
- The AI cites a small study as if it's definitive
- The AI cites a study in a different population than your patient and doesn't acknowledge the difference

### Step 6: Form Your Own Judgment

Based on reading the source, do you agree with how the AI used it?

- Is this good evidence for the recommendation?
- Is this evidence strong enough to change practice for this patient?
- Are there reasons to weight this evidence differently than the AI did?
- What would you do if this source didn't exist?

---

## Part 4: Synthesis Appraisal — Verifying How Sources Are Combined

The second major source of error is **incorrect synthesis of correct sources.** An AI (or guideline, or meta-analysis) might cite all the right studies but synthesize them wrong.

Examples:

- Including all five relevant studies but weighting one too heavily
- Presenting contradictions between studies as consensus
- Generalizing from one population to others
- Missing important heterogeneity
- Drawing a conclusion that goes beyond what the evidence supports

### Appraising Meta-analyses

When the AI cites a meta-analysis, you need to evaluate:

**Comprehensiveness**: Did they find all relevant studies?

- Look at: Search strategy, databases searched, unpublished studies sought
- Red flags: Single database only, no unpublished studies, vague search strategy

**Quality**: Did they assess study quality and weight appropriately?

- Look at: Quality assessment method, whether low-quality studies included/excluded
- Red flags: No quality assessment, equal weighting of high and low-quality studies

**Heterogeneity**: Do the studies point in the same direction, or do they disagree?

- Look at: I² statistic (0% = no heterogeneity, 100% = complete heterogeneity)
- Rule of thumb: I² > 50% suggests substantial heterogeneity
- Red flags: High heterogeneity (I² > 50%) but conclusion stated as definitive

**Data presentation**: Does the forest plot show what the conclusion claims?

- Look at: Confidence intervals, direction of effect, size of effect
- Red flags: Some studies disagree but conclusion is presented as certain

**Publication bias**: Is there evidence of publication bias?

- Look at: Funnel plot, discussion of publication bias
- Red flags: Obvious funnel plot asymmetry not addressed

**Conclusion matching**: Does the conclusion match what the forest plot shows?

- Red flags: "Evidence supports X" when studies are mixed, "clear benefit" when heterogeneity is high

**Real example of problematic meta-analysis:**

A meta-analysis on "Antibiotics for common cold" included 10 studies. The forest plot showed:

- 3 studies showed antibiotics helped (but small effect)
- 4 studies showed no difference
- 3 studies showed harm

The I² was 72% (high heterogeneity). But the conclusion stated: "Antibiotics show modest benefit for common cold."

This is synthesis gone wrong. The studies disagreed substantially. The conclusion should have been: "Evidence is mixed, with no clear consensus." Instead, they pooled disagreeing studies and drew a favorable conclusion.

An AI citing this meta-analysis would be citing a flawed synthesis.

### Appraising Narrative Syntheses (Guidelines)

Many guidelines use narrative synthesis: They review evidence and summarize it conceptually rather than statistically.

Evaluate by asking:

**Coverage**: Did they include all major studies?

- Look at: Citation list, whether major trials are cited
- Red flags: Missing large or recent studies

**Balance**: Did they present both supporting and contradicting evidence?

- Look at: Whether they discuss contrary findings
- Red flags: Only cites supportive studies, ignores contradictory findings

**Interpretation**: Did they accurately represent what each study found?

- Look at: Whether citations match the text description
- Red flags: Selective quoting, changing meaning

**Weighting**: Did they weight high-quality studies more heavily than low-quality ones?

- Look at: Whether study design and quality are discussed
- Red flags: Treating all studies as equal

**Conclusion match**: Does the recommendation match the evidence presented?

- Red flags: "Strongly recommend X" when evidence is mixed, leaving out important exceptions

**Real example:**

A guideline recommends "Hormone therapy for all postmenopausal women with vasomotor symptoms" based on a narrative synthesis. But when you read the evidence they cite, it's mostly from older studies before the Women's Health Initiative. They cite some newer studies showing increased cardiovascular risk but dismiss them as "outliers."

The synthesis itself is biased—it emphasizes older, favorable evidence and downplays newer, contradicting evidence.

### Appraising AI's Own Synthesis

This is the new problem: The AI synthesizes studies, and you need to verify the synthesis.

**Citation matching**: Does the AI cite the studies it claims?

- Ask the AI for a list of sources
- Spot-check if they exist

**Representation matching**: Does it represent each study correctly?

- Read a key study
- Compare to how AI described it
- Does the characterization match?

**Weighting**: Does it weight high-quality studies more than low-quality ones?

- Ask the AI: "Which study was most influential?"
- Does it acknowledge quality differences?

**Heterogeneity**: Does it acknowledge when studies disagree?

- Ask the AI: "Did any studies show opposite findings?"
- If yes to opposite findings, does it address the disagreement?

**Conclusion match**: Does the conclusion match the evidence presented?

- Take the studies it cited
- Do they support the conclusion?
- Or did the AI go beyond what they showed?

**Practical approach to AI synthesis verification:**

1. Ask the AI to list its sources clearly: "List all studies you're basing this on"
2. Spot-check the most important ones (largest study, most recent guideline)
3. Verify they exist and say what AI claims
4. Look for contradictory evidence: "Were there studies showing X?"
5. Ask about weighting: "Why did you emphasize this study over that one?"
6. Check for overgeneralization: "Does this apply to [specific population]?"

### Red Flags in Any Synthesis

Regardless of type, watch for:

**1. Certainty without acknowledgment of uncertainty**

- "This treatment works" (instead of "may work")
- "Guidelines recommend" (instead of "conditionally recommend")
- No discussion of when evidence is weak

**2. Missing contradictory evidence**

- Only cites supporting studies
- Doesn't acknowledge studies that point opposite direction
- Doesn't explain why contradictory evidence is dismissed

**3. Overgeneralization**

- Studies done in one population applied to others
- Recommendations stated absolutely when evidence is conditional
- Time-sensitive recommendations treated as permanent

**4. Insufficient detail about evidence quality**

- Doesn't distinguish between RCTs and observational studies
- Doesn't mention study size or risk of bias
- Treats weak evidence the same as strong evidence

**5. Vague citations**

- "Research shows..." without specific citations
- "Studies suggest..." without naming them
- "Guidelines recommend..." without specifying which guideline

**6. Conclusion-creep**

- Evidence shows "may help" but synthesis concludes "does help"
- Evidence shows "in some populations" but synthesis generalizes to all
- Evidence shows "moderate benefit" but synthesis markets as "effective"

---

## The Protocol: Citation and Synthesis Appraisal in Practice

Here's a practical protocol for appraising sources when an AI gives you a recommendation:

### For Routine Decisions (Low-Stakes)

**Quick check the citations:**

- Do the citations look real? (Author + year + journal)
- Can you spot-check one major citation quickly?
- Does the AI acknowledge limitations or uncertainty?

**If red flags**: Do more thorough appraisal (below)

**If looks reasonable**: Proceed, but note you didn't fully verify

### For High-Stakes Decisions (High-Risk Changes, Major Interventions, Rare Scenarios)

**Step 1: Use one of the three appraisal approaches from Chapter 2**

- Clinical judgment: Does this match your experience? (if in your expertise)
- Source appraisal: Read the actual sources cited
- Systematic verification: What's missing? What aren't they saying?

**Step 2: Identify the key citations**

- What evidence is the AI relying on most heavily?
- Usually: the largest studies, most recent guidelines, or meta-analyses

**Step 3: Verify key citations exist**

- Search PubMed or Google Scholar
- If citation doesn't exist, note it as unverified

**Step 4: Read the key citations**

- At least methods, results, and limitations
- For meta-analyses: look at the forest plot and heterogeneity
- For guidelines: look at evidence base and caveats

**Step 5: Assess quality using frameworks from Part 1**

- For studies: randomization, blinding, follow-up, baseline characteristics, sample size
- For meta-analyses: search comprehensiveness, quality assessment, heterogeneity, publication bias
- For guidelines: evidence base, currency, acknowledgment of limitations

**Step 6: Evaluate effect size and applicability**

- What was the magnitude of effect? (NNT, relative risk, absolute risk reduction)
- Are confidence intervals wide or narrow?
- Is the population similar to your patient?
- Is the outcome clinically relevant?

**Step 7: Compare what you read to what the AI said**

- Did the AI represent the source accurately?
- Did the AI leave out important caveats or qualifications?
- Did the AI weight the source appropriately?

**Step 8: Evaluate synthesis**

- Do the sources the AI cites actually support its conclusion?
- Did it acknowledge studies that point different directions?
- Did it appropriately weight high-quality vs. low-quality evidence?

**Step 9: Form your judgment**

- Based on your reading, do you agree with the recommendation?
- What would you do differently, if anything?
- What's your confidence in the recommendation?

---

## Common Pitfalls in Source Appraisal

### Pitfall 1: Trusting the Citation Format

**"If it looks like a real citation, it must be real."**

Not true. Hallucinated citations often look perfect:

- Correct author names
- Real journal
- Plausible year
- Reasonable title

But the actual combination doesn't exist. Check by searching, not by trusting format.

### Pitfall 2: Assuming the AI Read the Source Carefully

**"The AI cited it, so it must have understood what it says."**

No. The AI may have skimmed multiple papers, combined information from different sources incorrectly, or misremembered details.

Always read important sources yourself.

### Pitfall 3: Assuming a Guideline Accurately Synthesized Its Evidence

**"It's a guideline from a reputable organization, so the synthesis must be good."**

Guidelines vary in quality. A prestigious organization can still create a biased synthesis.

Spot-check the evidence the guideline cites. Does the recommendation match?

### Pitfall 4: Not Noticing Conditional vs. Absolute Recommendations

Many guidelines use careful language:

- "Consider X" (conditional, weak evidence)
- "X is recommended" (stronger)
- "X is not recommended" (against it)

The AI might collapse these distinctions and present a conditional recommendation as absolute. Read the actual guideline to preserve these nuances.

### Pitfall 5: Ignoring Publication Bias

Meta-analyses often have publication bias: Small studies with positive results get published; small studies with negative results don't. The funnel plot may show this.

If a meta-analysis shows publication bias, the true effect is probably smaller than the pooled estimate.

The AI might cite the pooled estimate without acknowledging the bias.

---

## Summary

Citation and synthesis appraisal in the AI era requires verifying two things:

**Citation appraisal**: Is each individual source accurate and reliable?

- Does the citation exist?
- Does it say what the AI claims?
- Is it good quality evidence?

**Synthesis appraisal**: Did the AI (or guideline, or meta-analysis) correctly synthesize multiple sources?

- Were all relevant sources included?
- Were they weighted appropriately?
- Was contradiction acknowledged?
- Does the conclusion match the evidence?

Both are essential. A perfect meta-analysis misrepresented is still wrong. Individual studies synthesized poorly still lead to bad conclusions.

Use the three approaches from Chapter 2:

- **Clinical judgment** when you have expertise
- **Source appraisal** when you need to verify thoroughly
- **Systematic verification** to catch gaps and omissions

The protocol is:

1. For routine decisions, do quick citation checks
2. For high-stakes decisions, do full appraisal of key citations and synthesis
3. Always read important sources yourself
4. Always compare what you read to what the AI claimed
5. Form your own judgment before acting

This is the critical skill for practicing safe EBM in the AI era.

---

## References



---

## Further Reading

