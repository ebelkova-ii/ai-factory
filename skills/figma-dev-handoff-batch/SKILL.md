---
name: figma-dev-handoff-batch
description: Prepare selected Figma designs for development with separate onboarding, one analysis across ten checklist areas, grouped questionnaires and batch edits. Use for optimized handoff with real measurement diagrams; use figma-dev-handoff for sequential stage approvals.
---

# Figma Development Handoff — Batch

Work in Russian through connected Figma tools. This is an independent optimized alternative to `figma-dev-handoff`; do not edit or depend on that skill. Preserve exact technical/library names. Examples supply formatting, not product facts or node identities.

## Project context before onboarding and analysis

Use the current project/workspace as the source of project-specific requirements. Before preparing questions or assessing Figma designs, read applicable `AGENTS.md` instructions and follow their relevant links to Markdown documentation, component contracts and design-system rules. Search the project narrowly for missing topics; do not read every Markdown file or assume that a global skill's directory is the project root. If project files are unavailable, report the limitation and request only essential missing context.

Extract the rules applicable to the selected product, page type and version, retaining source paths/sections and documented exceptions in the shared dataset. Distinguish documented requirements, observed Figma properties and behavior actually exercised. Use established project answers without asking the user to confirm them again. Explicit task decisions take precedence; when applicable project documents conflict with each other or Figma, show the concrete conflict and sources in the decision package rather than silently choosing or inventing a rule. Ask only about genuine gaps or unresolved conflicts.

Project documentation establishes expected behavior, not authorization to change designs, code, tokens or libraries. Preserve the existing scope and approval boundaries. Keep project values in the project documentation rather than hardcoding one project's breakpoints or grid into this reusable skill.

## 1. Separate onboarding

Inspect the connection, current file/page/selection and available capabilities once. Locate the live checklist, prepared `constraction`, construction reference, findings template, Note and measurement palette by structure/context. They can be sections or frames. Do not scan the whole file to find optional materials.

Present one short onboarding questionnaire for facts that are not already established:

- Scope: selected screens/flows/components and responsive counterparts; choose applicable review areas through the interactive checklist below, rather than asking the user to type the steps to skip. Reading a counterpart does not authorize a full review or edits outside scope.
- Text source of truth: desktop, mobile, a supplied approved source, or no single source. Clarify which screens/scenarios the choice covers; never silently default to desktop. If no source is chosen, semantic differences require decisions later.
- Working targets: confirm only ambiguous or missing construction/checklist/template targets; reuse clearly identified existing targets without another question. Ask before using another file or creating a missing output container.
- Essential supplied context, if absent: flow boundaries or access to required counterparts. Defer behavior/breakpoint questions not answered by applicable project documentation to the consolidated analysis package.

Choose review areas with an interactive onboarding form, separate from the read-only text of the Figma checklist. Read the live checklist order and use it for the onboarding form, mapping rows by meaning without rewriting, renaming or reordering the Figma checklist. The supplied checklist places images/assets before the last two areas, accessibility and motion. When no live order is available, use: flow/navigation; assembly/layer naming; components; construction; states/behavior; responsiveness/edge cases; proofreading/typography; images/assets; accessibility; motion. If the actual input tool supports independent checkboxes or multi-select, initialize all areas as selected and ask the user to uncheck those not needed for this run. Preserve any explicit choices already given instead of resetting them or asking again.

If the native form supports only single-choice questions, use one independent question per undecided area with `Проверить` / `Пропустить`, grouped into one form where tool limits allow (otherwise the minimum required batches). This fallback must still let the user select scope without typing step names. Do not describe single-choice controls as checkboxes or invent unsupported form fields. If no interactive input is available, disclose that limitation and use a compact numbered checklist in chat as a fallback. This is one scope-selection step, not ten sequential approval gates. Only submitted answers establish scope; preselected controls, unsubmitted forms and silence are not consent. Once submitted, summarize included/skipped areas and continue without a second confirmation. These choices apply to this run and do not become permanent exclusions.

State the located scope and output targets briefly. Preserve explicit prior answers; do not repeat the onboarding after interruptions. Resolve essential scope/source questions before dependent edits, while continuing independent preparation. Freeze source/target identities; later selection changes do not silently expand scope. Do not re-ask permission for the autonomous edits authorized below.

## 2. Shared data and ten-area analysis

Read [references/checks.md](references/checks.md) once for the applicable areas, [references/figma-output.md](references/figma-output.md) before canvas writing, and [references/text-review.md](references/text-review.md) for proofreading. Read the bundled policy only for relevant rules.

Collect one compact dataset in bounded requests: scoped semantic hierarchy, actual UI strings, layout properties, component families, relevant states/prototype links, assets and output-template contracts. One collection may require multiple calls; it is not a full-file JSON dump. Stop traversal at ready-made global components such as Header/Footer; inspect their internals only for a specific relevant issue or overridden content. Exclude vector paths and unused hidden drafts. Include meaningful hidden states and product content.

Reuse this dataset across all ten areas: flow, assembly/naming, component inventory, construction, states, responsiveness, proofreading, assets, accessibility, motion. These are coverage categories, not ten approval gates. Inspect one representative per equivalent rule group and record meaningful differences/coverage. Never infer unknown behavior, breakpoints, limits or animation from appearance.

Refresh only objects changed by the user, genuinely missing data or a narrow failed-write target. Update cached facts from successful own writes; do not reread them routinely. If there is evidence of concurrent edits, refresh the affected objects before overwriting. Keep compact scope, object IDs, decisions, coverage, sources, pending questions and applied edits in task context, without mandatory tracking artifacts.

## 3. Autonomous changes

Within the agreed scope, apply without permission questions or proposed mappings:

- Meaningful English kebab-case names for ordinary semantic containers, UI text layers and page-owned elements. Preserve library names, component properties, tokens, styles and technical identifiers. Skip individual vector paths and unused hidden drafts.
- Unambiguous nonbreaking-space corrections under the text-review rules, preserving content, protected strings and intentional formatting.
- Exact text parity between corresponding desktop, mobile and theme variants in the same scenario/state/data, including identical explicit line breaks, nonbreaking spaces binding prepositions and other word groups, and nonbreaking hyphens (U+2011), using the onboarding source of truth and approved exceptions. Do not propagate a suspected grammar error silently: propose its correction in the proofreading group. If the source is absent, ambiguous or itself conflicting, leave the semantic difference for a decision. NBSP normalization can still proceed where unambiguous.

Do not silently rebuild layouts: Auto Layout, hierarchy, Hug/Fill, constraints, responsive rules, duplication removal and composition changes require concrete approval. Do not automatically round or correct fractional geometry/layout values; record them as construction findings with location links under [references/checks.md](references/checks.md). Changing them requires approval of the exact proposed values; general handoff-output approval does not authorize rounding. Autonomous naming is not permission to alter layout, product behavior, masters/tokens or component contracts. Never detach instances. Grammar, spelling and punctuation replacements require approval of exact text; text-source selection does not approve further editorial changes.

## 4. One decision package in meaningful groups

After shared analysis, present the completed autonomous edits separately from decisions. Use a native multi-question input tool when available, with a separate answer for each independent decision and native free text. Otherwise use a compact numbered questionnaire in chat. Respect actual tool limits; do not invent multi-select or arbitrary form fields.

Group the package by meaning, for example:

1. Product rules and unknowns: behavior, states, breakpoints. Offer concrete supported alternatives or free input; never invent a requirement as a default.
2. Layout corrections and findings: location, brief evidence, exact proposed change; choices such as apply / record finding / skip / free input.
3. Proofreading: numbered `Место → Было → Станет → Причина` replacements, grouped by equivalent correction. Offer yes/no/free input and exclusions.
4. Handoff output: compact construction coverage/placement, brief Notes, component lists, assets and checklist findings/statuses. Keep measurements on canvas rather than pasting inventories into the questionnaire.

Combine homogeneous items with explicit scope and allow `Применить всё, кроме №…`. Keep stable IDs so exceptions identify exact changes. Do not collapse unrelated consequences into one ambiguous yes/no. Essential dependent unknowns may require a focused follow-up; do not restart ten sequential gates. Unanswered, preselected and silent options are not consent. Apply decided independent items while leaving unanswered dependencies pending. Report explicit skips/deferrals honestly.

Review copy only for spelling, grammar, punctuation and typography; do not propose new formulations, shortening, tone changes or stylistic alternatives. Do not post editorial comments in Figma. Missing error copy is an open requirement, not permission to write a new message. Necessary developer Notes may explain confirmed behavior without changing UI copy.

## 5. Batch writing and finish

Approval permits the concrete approved changes and corresponding output/status updates without a second approval per category. Apply dependent operations sequentially, and independent changes in bounded batches. Reuse real Note, measurement and checklist components from the user's reference. Preserve prepared work and do not overwrite reference examples.

The designer owns the contents of the prepared construction container (`constraction`, `constractions`, or another identified name). Annotate only the screens, product components and images the designer has placed there. Do not add, copy, move, import or instantiate product content into it, or propose automatic population as part of the handoff package. General approval of handoff output does not authorize filling the container. Documentation instances (measurements, Notes and checklist tools) and component-list text may be added around the prepared objects. Record missing coverage and the objects the designer needs to supply in findings; continue work on available objects without filling gaps yourself. Preserve existing placement unless a concrete rearrangement is approved.

High-quality measurement diagrams remain required for the prepared objects: follow the placement and tool-selection contract in [references/figma-output.md](references/figma-output.md). Show dimensions, spacing, padding, radii, confirmed sizing rules and constraints in real measurement tools. Where width is a confirmed percentage, identify both the percentage and whether it refers to the viewport or a particular container; do not replace that rule with a fixed pixel value. Omit the overall height of complete screens/pages and measure individual-element heights instead. Measure repeated constructions once with explicit coverage; annotate meaningful differences. Keep readable placement and necessary nested-part measurements. Do not replace diagrams with prose or remove coverage for speed. Notes contain brief construction/grid explanations and non-obvious rules, not numeric inventories.

After successful writes, the user reviews the output. Do not add routine readbacks, screenshots, temporary QA copies, tests, repeated inventories or a separate validation stage. Recover narrowly from actual tool errors; do not retry inaccessible component sources. Do not claim unperformed checks or erase retained findings.

The live checklist is status-only: preserve all existing text exactly, including headings, item wording, labels and descriptions. Do not rewrite, proofread, normalize spaces/line breaks, rename rows or append explanations or summaries inside the checklist. This restriction overrides the autonomous naming and text-correction rules for checklist content. Match existing rows by meaning/order and change only their check/cross status properties. For `done` / `reject`: true/false = reviewed and completed without unresolved findings (check); false/true = reviewed with retained findings or deferrals (cross); false/false = unfinished or explicitly skipped/non-applicable (unmarked). Never set both true or mark an unreviewed item complete. Record findings, skips/non-applicability and reasons separately outside the checklist, in the agreed findings area or final report. Read status properties only to identify the target, not after writing.

Finish briefly with scope, automatic/approved changes, unresolved findings, skipped areas and checks not performed. Distinguish static design inspection, prototype playback, export settings, actual exports and runtime tests. Static designs do not certify implementation accessibility or product readiness.
