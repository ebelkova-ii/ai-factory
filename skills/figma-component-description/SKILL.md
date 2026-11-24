---
name: figma-component-description
description: Create or revise selected Figma component specification blocks in nearby templates using shared analysis, grouped questions and batch approvals. Preserve complete variant, size and layer coverage, real demonstrations and visual verification.
---

# Figma Component Specification

Use connected Figma tools in Codex to document the selected component in nearby specification frames. Questions and approvals belong in Codex. Write questions, specification content and the final report in Russian; preserve exact component, property, variant, token and style names and template section titles. Explicit user instructions take precedence.

## 1. Identify scope and targets once

Discover only needed tool names/schemas; avoid broad searches matching shared description boilerplate or dumping the tool catalogue. Read [canvas-writing.md](references/canvas-writing.md) once before node inspection for API safety, reusing it when writing. Check connection, current file/page and selection. If access is unavailable, explain the limit without claiming inspection or changes. Accept a main component, component set or instance of one component; inspect accessible main definitions and distinguish instance overrides. Resolve empty, unrelated or ambiguous selections before dependent work.

Determine operation (`create` from placeholders or `revise` existing documentation) separately from scope (all, one or several blocks). Derive the selected subset from the request; never silently expand it. Read applicable project `AGENTS.md` and relevant linked requirements narrowly, using the actual project root. Reuse established answers; project rules establish requirements, not editing permission.

Read [block-map.md](references/block-map.md) once. Read only enough nearby frame/checklist structure to locate selected targets and their live grouping/order. Match titles, structure, common container and context as well as proximity. The checklist routes eight blocks; it is not a ninth block. Missing unselected frames do not block targeted work. Do not obtain templates from another file without authorization.

Use live checklist status and actual content together: neither `done` nor `reject` means unfilled even when component-specific examples are present; `reject` means reviewed with findings, not an empty template. The supplied unfilled templates contain a `date-picker` reference. Replace its editable text and demonstrations with source facts while retaining structure and protected fields. Reference values, behaviors and statuses are not product requirements. Do not overwrite genuinely completed documentation as a placeholder; clarify creation versus revision if they conflict.

Present one short onboarding package only for unresolved operation/scope, source library, optional Taiga cross-check, or ambiguous selection/targets. Library and Taiga choices are independent. For an enabled cross-check, read [taiga-ui.md](references/taiga-ui.md) once for release, access and applicability rules. A direct request enables it; refusal introduces no Taiga dependency.

Freeze source and target identities after resolving them; later selection changes do not switch or expand the task. Continue independent preparation while essential onboarding dependencies await answers. Do not repeat onboarding or ask for another confirmation of submitted choices.

## 2. Build one shared dataset

Read [findings.md](references/findings.md) once and only selected block references. Collection may take several bounded requests; it is not a full-page/file JSON dump. Collect the needed source definitions, semantic hierarchy, actual variant combinations/sizes, nested parts, relevant states/prototype links/triggers/transitions/timing, layout, bindings/styles/text runs, and selected template/checklist/palette contracts. Exclude vector paths, image/base64 payloads and unrelated templates. Include required hidden/conditional parts. Extract available prototype facts before behavioral questions; configurations are not approved runtime requirements or playback results.

Keep compact task context, not a mandatory tracking file:

- File/page/source/target IDs, overrides, selected blocks/checks and protected regions.
- Actual source facts and template/tool contracts; reusable font, token and style metadata.
- Coverage of layers, nested occurrences, sizes, combinations, checks and unavailable data.
- Evidence with paths/URLs/sections, release baseline, corporate decisions and exceptions.
- Stable question/change IDs, dependencies, approvals, refusals, deferrals and applied writes.

Reuse these facts across selected blocks. For construction, account for every actual layer, including nested/hidden/conditional layers and relevant mixed text runs. Shared definitions/metadata may be read once, but every occurrence's bindings, overrides, modes and ancestor context still count. For variants and sizes, retain complete inventories for demonstration coverage. Equivalent metadata does not justify representative-only coverage.

Refresh only missing evidence, externally changed objects, failed-write targets or facts needed to verify changed results. Update cached facts from successful own writes. Before overwriting, narrowly guard the affected target and approved before-state; do not routinely reread the source or all templates for each question/block. Resolve evidence conflicts explicitly.

## 3. Analyze and clarify in meaningful groups

Analyze selected blocks in relative live checklist order using the shared dataset. These are coverage groups, not separate approval gates. Investigate accessible Figma, project and enabled library sources before requesting extractable facts. Distinguish observed Figma properties, documented library capabilities, confirmed corporate requirements, proposals and behavior actually tested. Do not infer runtime behavior from appearance, token currency from binding presence, or accessibility from static designs.

Collect genuine gaps into a compact thematic questionnaire: for example purpose/content, behavior/states, responsive/edge limits, accessibility/motion. For onboarding and later decisions, prefer an available native form with ready options and free input for each independent decision, within actual tool limits. Do not invent controls. An accepted tool call proves neither a visible form nor submitted answers. Keep required forms open and use available bounded waits until answers arrive; do not send a final that closes a pending form. If closed/invisible, resend only unanswered questions, preserving submitted decisions. Use a chat questionnaire only when native forms are unavailable. Preselection and silence are not answers or consent.

Reuse confirmed answers; ask a focused follow-up only when a new dependency needs it. Distinguish a proven defect, unknown requirement and suggestion; establish the requirement before calling uncertainty a defect. A component problem blocks dependent changes, not independent read-only analysis. Do not introduce unsolicited redesign.

Essential unknowns need an answer or explicit agreed deferral; never silently substitute “нет данных”. A request to record a described gap in remarks authorizes that entry, not behavior, a source fix or a passed check. Follow the findings rules for unresolved impact/status. Do not re-ask explicitly deferred questions. If even a safe limited description is impossible, agree the limited record/scope. Confirm non-applicability before presenting it as established.

Carry corporate departures, refusals and decisions across blocks. If new evidence conflicts with earlier content, locate the exact affected text, reading another block narrowly only as needed. Propose the concrete correction in the decision package. Editing an unselected block first requires scope authorization. Honor refusal; do not repeat the proposal without materially new evidence or a new request. Retained inconsistencies remain visible.

## 4. Approve a concrete package

Prepare concise drafts and demonstrations using the contracts below. Inspect both text and associated demos for unrelated template material before presenting changes. Group independent decisions without hiding their consequences; use stable IDs and allow explicit exclusions such as “Применить всё, кроме D03”. Split only for real dependencies or interface limits, not into mandatory per-block gates.

| Change type | Show before approval |
| --- | --- |
| Create | Each selected block's concrete content, full demonstration/measurement coverage, replaceable template material, relevant layout changes, remarks and intended checklist results |
| Revise | Change ID, exact frame/element, current → proposed text/demo/layout/status and reason; include related local reflow explicitly |
| Source fix | A separate ID/decision: evidence, exact source/variants/properties, concrete proposed fix/values and known dependent documentation/demonstrations |
| Findings/checklist | Concrete entries, removals or results tied to selected blocks/checks; not blanket permission to rewrite the checklist |

Requirement answers do not approve a later draft. Approval covers the described text, instances, annotations, layout and corresponding listed results without a second permission per category or transition. A revise package may approve several individually specified changes together; an overall vague instruction does not approve undisclosed changes. Documentation approval alone does not authorize separately listed source fixes; explicit approval of a package that includes named source changes can authorize them without a duplicate question.

Apply only decided items and their authorized dependencies. Unanswered or ambiguous items remain pending; continue approved independent work. Rejected changes are skipped, not treated as accepted. A changed approved proposal needs renewed approval only for its changed part. Do not ask “перейти к следующему блоку?” after a package approval. If a required capability is unavailable, explain the limit and ask for the necessary action rather than claiming success.

## 5. Route content without losing coverage

Follow live checklist order, not the table's text order if the live grouping differs. Detailed block contracts live in the linked references; they use the shared interaction rules above.

| Block | Read when selected | Required output |
| --- | --- | --- |
| Passport | [passport.md](references/passport.md) | Name/Level/purpose/usage/content rules. Design and development readiness each need an independent answer from exactly `to do`, `in progrees`, `ready`; they may share one questionnaire. Owner, Last change and the entire history remain untouched, including sample/empty contents. |
| Construction | [construction.md](references/construction.md); [measurement-tools.md](references/measurement-tools.md) for annotations | All sizes and necessary nested-part dimension demonstrations with real tools. Full internal color/typography/size-binding audit; publish only grouped attention findings, not correctly bound-layer inventories. Preserve size/anatomy layouts and Tools for spech palette. |
| Variants | [variants.md](references/variants.md) | Every existing variant combination: real instance plus individual purpose/use description. Do not invent combinations or reduce them to representative examples. |
| States | [states.md](references/states.md) | Parent/nested ownership, confirmed conditions/behavior, valid combinations, named groups and comparable baseline/target pairs. Preserve captions, token-range treatment and the live grid; describe visible changes rather than raw diffs. |
| Responsive | [responsive.md](references/responsive.md) | Actual sizing/overflow/wrapping and confirmed contexts/limits, demonstrated with real instances and actual measurements. Do not invent breakpoints or alter the source to force a demonstration. |
| Edge cases | [edge-cases.md](references/edge-cases.md) | Applicable confirmed boundary inputs and expected outcomes with consistent demonstrations. Keep preliminary presentation decisions explicit. |
| Accessibility | [accessibility.md](references/accessibility.md) | Component-specific source-backed practices, user impact and tradeoffs. Distinguish recommendations, implementation requirements and tested results. |
| Animation | This paragraph; animation research in [taiga-ui.md](references/taiga-ui.md) only when enabled | Confirmed triggers, transitions, affected properties, timing/duration/easing, interruption and reduced-motion behavior where relevant. Investigate extractable source facts before questions; agree non-applicability. Preserve the existing description/demo structure. |

Preserve headings, subtitles and the supplied visual system. Expand heading-only Responsive/Edge cases with compatible descriptions/cards. Real examples and confirmed overrides replace unrelated placeholders; static demonstrations are not working prototypes. Do not delete a required section just because applicability is unresolved. Keep contradictory source variants in inventory/findings, not as supported states.

## 6. Write, verify and finalize

Apply the already-read [canvas-writing.md](references/canvas-writing.md). Write independent approved changes in bounded batches; execute dependent operations sequentially. Guard targets against external changes; preserve fonts, rich text, links, range bindings, protected content and instance relationships. Never detach instances. Change source components/tokens only with concrete approval.

After a source fix, immediately verify affected variants, nested instances, demonstrations and intentional overrides before dependent output; consult the propagation guidance in states when needed without starting a full unrelated states review. Do not claim propagation from approval alone. Material changes to the approved draft require a focused new decision.

Use one consolidated coverage/text/instance/link and visual pass over changed frames, with bounded views as needed. Actual errors, suspicious geometry and propagation failures require immediate narrow inspection/recovery. Retain real visual verification and disclose unavailable checks; do not repeat inventories, source reads or unchanged-frame screenshots.

Finalize only selected block checks after approved content and verification. Preserve checklist title, order, grouping and annotations; keep wording except concrete approved edits/pointers. Map evidence/dependencies to each check; do not reject independent checks because another part of the block has findings. Use the template statuses, distinguishing reviewed findings/deferrals from unfinished checks. Missing runtime testing is a limitation, not by itself a proven defect. Keep labels compact and details in the block. Revise checklist content/status changes belong in the approval package. Never mark unreviewed, unresolved or unselected checks complete. If checks do not support an approved planned status, leave it pending unless the concrete unresolved result was also authorized; propose only the affected correction.

Resume after interruption from recorded IDs, scope, decisions, coverage, applied writes and pending dependencies. Keep skipped blocks and submitted onboarding decisions.

Finish briefly in Russian: processed blocks and approved documentation/source changes; confirmed corporate differences; retained findings, explicit deferrals/skips and checks not performed. Distinguish completed review from complete requirements/readiness, and static design/source inspection, prototype playback and runtime testing. For a skill trial, distinguish skill execution evidence from product implementation evidence. If essential unknowns were not explicitly deferred, request the focused remaining answers instead of claiming completion. Do not present unselected blocks as mandatory unfinished work.
