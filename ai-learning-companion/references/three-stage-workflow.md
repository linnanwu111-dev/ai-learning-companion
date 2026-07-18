# Three-stage learning workflow

## Contents

1. Knowledge Map
2. Unified-Scenario Analogy
3. Feynman Check
4. Stage handoff format

## 1. Knowledge Map

Use this module for large, scattered, or unfamiliar source material.

Confirm the field, accessible sources, learning goal, and filtering priorities before starting.

### Stage 1: Build a source index

1. Inspect the table of contents, bookmarks, page ranges, headings, and extractable text.
2. Build a lightweight index of sections, core themes, important source locations, and priority.
3. Separate source-backed findings from hypotheses that still require checking.
4. Do not load or summarize the entire source at once when staged reading is possible.

Deliver:

- source inventory and access status;
- lightweight index;
- priority reading plan;
- missing or unreadable sections.

### Stage 2: Create a traceable structure draft

1. Read the high-priority sections selected from the index.
2. Produce a Markdown hierarchy with no more than four levels.
3. Preserve page, section, heading, or quotation anchors for important claims whenever available.
4. Mark uncertain or conflicting information instead of resolving it silently.

Deliver:

- traceable Markdown structure;
- source anchors for key nodes;
- unresolved questions and conflicts.

### Stage 3: Produce the high-density map

1. Derive one complete 16:9 map from the confirmed structure draft.
2. Emphasize module relationships, the learning path, concept boundaries, and decision chains.
3. Avoid filling the map with disconnected sentences.
4. If image generation is unavailable, produce a structured visual specification instead.
5. Maintain one canonical complete map. Zoom into that same map for details rather than inventing separate local maps.

Deliver:

- complete map or render-ready visual specification;
- mapping from visual nodes to the structure draft;
- items that still require human verification.

### Stage 4: Check usability

Verify titles, hierarchy, page numbers, numbers, Chinese text, source anchors, and mobile readability. State explicitly that a finished map is a navigation aid, not proof of understanding.

## 2. Unified-Scenario Analogy

Use this module when abstract or neighboring concepts are difficult to distinguish.

Confirm the field, target topic, concept list, source material or confirmed structure draft, and any preferred everyday scenario.

1. If no scenario is provided, choose one familiar scenario capable of containing every target concept.
2. Use one shared scenario. Do not invent unrelated stories for individual concepts.
3. Explain what happens in the scenario before mapping terminology.
4. Compare concepts in a table with these fields:
   - scenario event or object;
   - professional concept;
   - why the mapping works;
   - difference from neighboring concepts;
   - limitation of the analogy.
5. Return to the source-backed professional definitions.
6. Summarize practical decision rules, positive examples, and counterexamples.
7. If the materials cannot support the definitions, request more evidence rather than forcing a conclusion from general knowledge.

Deliver:

- shared scenario;
- comparison table;
- analogy limits;
- source-backed decision rules.

## 3. Feynman Check

Use this module after the learner has studied a topic. Confirm the topic, source material or confirmed structure draft, and question count. Default to five rounds only when the user does not specify a count.

1. Ask the learner to explain the topic completely in their own words without copying the source.
2. Do not provide the explanation before the learner answers.
3. In each round, ask one question based on the learner's latest answer and target the most important gap.
4. Prioritize:
   - definition accuracy;
   - concept boundaries;
   - examples and counterexamples;
   - transfer to a new situation;
   - verifiable conditions;
   - trade-offs and constraints.
5. When an answer is wrong, identify the concrete contradiction or missing condition, then invite correction. Cite the source location when available.
6. Do not reveal the final score before the agreed rounds are complete.

Final feedback must include:

- a score out of 100 with explicit evidence-based criteria;
- what the learner demonstrated correctly;
- errors, omissions, and confused neighboring concepts;
- source locations to revisit;
- the smallest next learning action.

Describe the score as a feedback interface for locating gaps, never as an exam result, certification, or objective measure of ability.

## 4. Stage handoff format

At the end of each stage, use this compact structure:

```markdown
## 本阶段产物

[output]

## 依据

- [source and location]

## 待核对

- [uncertainty or missing evidence]

## 建议下一步

[one proposed action]
```

Do not advance automatically if the next stage requires a new source, a changed scope, or user confirmation.
