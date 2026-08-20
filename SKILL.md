---
name: cms-debate-kit
description: Create or review excerpt-grounded classroom debate kits, including propositions, evidence cards, worksheets, rubrics, and quote-validation reports. Use when adapting the same debate workflow to a different book or numbered excerpt; do not use outside knowledge as textual evidence.
---

# CMS Debate Kit

Turn a supplied excerpt into a traceable debate kit whose claims and quotations can be checked against that excerpt.

## Non-negotiable rules

- Treat the supplied excerpt as the only evidence source. Never introduce facts, plot details, authorial intent, historical context, or statistics that are absent from it as evidence.
- When the excerpt does not support a requested claim, write exactly `발췌문에서 확인 불가`. Do not fill the gap with a plausible inference.
- Copy quotations verbatim and attach the correct paragraph number. Preserve wording, spelling, punctuation, and meaningful spacing; do not silently paraphrase, correct, combine, or add ellipses inside quotation marks.
- Distinguish interpretation from textual fact. A debatable interpretation is allowed only when its quoted evidence is present and the connection is explained.
- Preserve every source file. Do not edit, rename, move, or delete excerpts, rules, forms, or prior outputs.
- Save new artifacts under `<project root>/결과물`. Before writing, inspect the current state, show the planned work, exact file list, and absolute save paths, then wait for explicit approval. One approval may cover all files already listed; additions require new approval.
- Stay within the user-approved project and file scope. Mark uncertain facts or numerical judgments as `확인 필요`.

## Prepare the source

1. Identify the excerpt file and read any local project instructions or debate rules.
2. Confirm that paragraphs have stable labels such as `[1]`, `[2]`, and record the total count. Verify a sample paragraph directly before drafting.
3. If labels are missing or ambiguous, do not alter the source. Explain that paragraph-level citation is blocked and propose a numbered working copy under `결과물`; create it only after approval.
4. If multiple excerpts could be the source and the choice cannot be inferred safely, ask which one governs the kit.

## Build the kit

Follow the user's requested quantities, audience, and formats. When unspecified, draft three proposition candidates and keep document output in Markdown.

### 1. Proposition candidates

- Form propositions that permit meaningful support and opposition from the excerpt.
- For each candidate, include at least one exact quotation with its paragraph number and briefly state the opposing tension.
- Do not claim that a side is supported when its case depends only on information outside the excerpt. Label any such limitation `발췌문에서 확인 불가`.
- Present candidates for selection before building evidence cards unless the user already selected a proposition.

Default output: `결과물/논제후보.md`.

### 2. Evidence cards

Create cards for both sides of the selected proposition. Each card contains:

1. one-sentence claim;
2. a verbatim quotation and paragraph number;
3. a connection between quotation and claim, normally no more than two sentences.

State whether evidence is direct or indirect when that distinction affects strength. If a requested side or card lacks support, keep the card visible and mark it `발췌문에서 확인 불가` instead of inventing evidence.

Default output: `결과물/근거카드.md`.

### 3. Worksheet and rubric

Base both artifacts on the selected proposition and validated evidence cards.

- The worksheet includes proposition, side selection, claim, verbatim quotation, paragraph number, claim-evidence connection, anticipated opposing claim, and rebuttal preparation fields. Remind learners to use `발췌문에서 확인 불가` when necessary.
- The rubric uses observable, audience-appropriate criteria. At minimum assess accurate excerpt evidence with paragraph numbers, listening and rebuttal, and respectful participation. Keep each criterion concise and internally consistent with the worksheet.
- Create DOCX only when requested. Preserve the Markdown source and visually verify any rendered document before delivery.

Default outputs: `결과물/활동지.md` and `결과물/루브릭.md`.

### 4. Quote validation

Validate every quotation used in propositions, evidence cards, worksheets, debate logs, and related outputs:

1. locate the cited paragraph in the excerpt;
2. compare the quoted content directly with that paragraph;
3. confirm the paragraph number;
4. classify it as exact match, mismatch, or absent;
5. for a mismatch, show the differing portion and the correct source text without silently editing the artifact;
6. for an absent quotation, report `발췌문에서 확인 불가` and flag it for removal or replacement.

Use an existing local validation tool when it supports the current input format, but do not modify the tool without approval. If no tool exists, perform direct exact-text searches and produce the same audit trail. Similarity is only a diagnostic aid; it does not count as a verbatim match. Report tool limitations and any result requiring manual confirmation.

Default output: `결과물/검증리포트.md`.

## Cross-check and handoff

Before completion, confirm that:

- the selected proposition is identical across all artifacts;
- every evidence-card quotation exists verbatim in the cited paragraph;
- worksheet and rubric terminology agree;
- no external knowledge is presented as excerpt evidence;
- all approved files are under `결과물` and all originals remain unchanged.

Report completion with a table listing each created file, its absolute path, its purpose, and the items the user should review. Include the file count and identify every `확인 필요` or `발췌문에서 확인 불가` entry.
