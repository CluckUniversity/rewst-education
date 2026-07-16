# Quiz question quality standards

## What types of questions to avoid

The problem isn't whether someone has to reference the lesson. The problem is testing things that are either self-evident or don't affect their ability to do the work.

**Avoid trivial recall questions:**

- Vocabulary that's obvious from naming (What does an "always" transition do? What is a "create ticket" action?)
- UI details they can find in the moment (What button opens the execution summary? Where in the menu is X setting?)
- Steps that don't require judgment (What's the first question RoboRewsty asks? What color indicates success?)
- Definitions where the answer is self-contained in the question stem

**Keep questions that test:**

- Conceptual understanding that shapes how they approach work (What is the blueprint designed to do? Why have a conversation before building?)
- Application and judgment (Which revision instruction is most useful? How do you describe a problem when you don't know the fix?)
- Patterns that prevent common mistakes (What causes workflows to need more revision? What's the weakest part of a vague blueprint?)

## Two-question test

Before including any question, apply both tests:

1. Would answering this question wrong cause them to do the work poorly, or would it just mean they didn't memorize a detail? If it's just a detail, cut it.
2. If this course uses an example workflow: Can someone who built a completely different automation still answer this question? If no, it's too tied to the example. Rewrite or cut.

## Answer choice rules

- One clearly best answer — flag if multiple answers could be reasonably defended
- Plausible distractors — each should reflect a real misconception; flag any obvious throwaway
- No "all of these" or "none of these"
- Similar answer length — a noticeably longer/shorter correct answer is a giveaway
- **No explicit negations in distractors.** Never write "X, but not Y" or "everything except Z." These are implausible because no one would deliberately omit critical information. Write distractors that reflect real mistakes: including wrong information, using the wrong tool, or solving the wrong problem.
- **Distractors must reflect real mistakes.** Ask: "Would a confused learner actually choose this?" If no, rewrite it.

## Question stem rules

- Must be a complete, unambiguous question on its own
- Avoid negative stems ("which is NOT...") — rewrite as positive where possible
- Should present a scenario or problem, not ask for a definition

## Feedback rules

- Correct feedback must explain *why* the answer is right, not just confirm it
- Incorrect feedback addresses the most likely reasoning error — one collective field covers all wrong answers (Skilljar constraint)

**Weak:** "Incorrect. The correct answer is B."
**Strong:** "Not quite. Waiting until the end of the shift to report the error means it stays live in the workflow. Catch it at the source — check the execution log immediately."

Strong feedback explains why the correct answer is right (reasoning, not just the label), addresses the most likely reasoning error behind wrong answers, shows real consequences rather than lecturing, and is one to two sentences. Skilljar has two feedback fields per question — one for correct, one collective for all incorrect answers.

**Rubric for AI-generated feedback:**
- [ ] Explains why the correct answer is right
- [ ] Addresses the most likely reasoning error behind wrong answers (collective — not per-distractor)
- [ ] Avoids condescending or punishing tone
- [ ] Concise — one to two sentences
- [ ] Connects to real job consequences

## Bloom's level reference

Match question type to Bloom's level:
- **Remember/Understand** → recognition-based questions (definition, identification)
- **Apply/Analyze** → scenario-based questions ("given this workflow, what happens when...")
- **Evaluate** → judgment questions with competing valid considerations

Bias toward Apply/Analyze and Evaluate. Remember/Understand questions are acceptable only when the concept is foundational and genuinely non-obvious.

---

## The telegraphed answer problem

AI defaults to one thorough correct option and two shorter, extreme distractors — making the right answer obvious before anyone reads the question. Fix:
- Require similar length across all answer options
- Each distractor should reflect a coherent but flawed mental model, not an obvious throwaway
- Rotate correct answer position (don't always put it first)

---

## Redundancy check

Review all questions together. If two questions test the same knowledge or have the same correct answer pattern, flag one for removal.

Example of redundancy:
- Q1: "Jinja error occurred, what's your next step?" → Answer: Use Live Editor
- Q5: "Want to test a Jinja fix, what should you do?" → Answer: Use Live Editor

These are testing the same concept. Keep only one.

## Examples of bad questions to avoid

**Too obvious (answer in stem):**
- Bad: You see "Result: published as" in the execution. What does this mean?
- Good: An action succeeded but the next action can't find the data it needs. Where should you check first?

**Implausible distractor:**
- Bad: Include the execution link, screenshots, and what you tried, but not the org name since Support can find it
- Good: Include a detailed description of the workflow's purpose and the expected outcome

**Recall vs. application:**
- Bad: What does a 404 error mean? (definition)
- Good: A workflow shows a 404 error on an RMM action that worked yesterday. What's the most likely cause? (diagnosis)
