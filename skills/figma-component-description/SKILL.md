---
name: figma-component-description
description: Use Codex with Figma MCP to create or revise a selected component's specification in nearby template frames. Work on all or selected blocks in checklist order, clarifying and approving each block before proceeding.
---

# Figma Component Specification

Work in Codex using the connected Figma MCP tools to read the selected component and edit nearby specification frames. Ask questions and obtain approvals in Codex, not the Figma agent. Check the connected file and selection before starting. If the connection is unavailable, explain what is needed rather than claiming access. Explicit user instructions take precedence over these guidelines.

Write questions and specification content in Russian. Preserve exact technical names of components, properties, variants, tokens, and styles. Preserve the template's section titles unless the user requests a change.

For every processed block, read [references/findings.md](references/findings.md) and include a bottom subsection «Замечания и спорные моменты» only when there are actual findings, required improvements, or material open questions. Do not create an empty subsection or a no-findings message. Use compact attention cards matching the construction token-findings treatment. Put only findings/open points there, grouping repeats; do not duplicate correct-layer inventories or rewrite unselected blocks.

## Interaction and authorization

- Ask exactly one question at a time and wait for the answer. Do not combine several information requests into one question. Use facts already available from the component or previous answers.
- Clarify every required fact you cannot establish from the component or supplied context. Do not invent behavior, owners, implementation status, dates, rules, token currency, accessibility results, or missing states. Do not silently replace clarification with “нет данных”. If the user explicitly cannot provide a fact, agree how to represent that gap before finalizing the affected content. An explicit request to record it in remarks authorizes that described entry under references/findings.md, not an invented answer or a source fix. Continue with confirmed information and keep the unresolved requirement visible; do not mark it passed.
- When you identify a component problem, pause before further edits. Explain the evidence and a concrete proposed fix, then ask whether to apply it. Wait. Apply only the approved fix and verify it; if declined, leave the component unchanged, retain the finding, and continue with confirmed information.
- Distinguish a proven defect from an unknown requirement or a suggestion. Ask about the requirement before calling uncertainty a defect. Do not introduce an unsolicited redesign.
- For a new specification, prepare and agree one block at a time before filling its supplied placeholder frame. Block approval authorizes its described text, demonstration instances, and layout adjustments; it does not authorize changing the source component or another block. After writing and checking the block, ask before starting the next one.
- A request to update an existing specification requires approval for each concrete change. Show the frame/element, current and proposed content or layout, and the reason; ask one permission question. Apply only that approved change. A refusal skips it. One approval does not authorize later changes.
- Reuse confirmed decisions and corporate departures from library defaults across blocks. Keep a compact record in task context or existing task notes of decisions, sources, deferred questions, and declined changes; do not require a new local record file to run this skill. When a new fact conflicts with relevant previously read content, identify the exact affected text. Read another block only as needed to verify that conflict, without starting an unrelated full review. Propose each correction separately under the existing approval rules; obtain scope authorization before editing an unselected block. Honor a refusal and do not repeat the same proposal without materially new evidence or a new user request. Never present a retained inconsistency as fixed.
- If a proposed fix requires an unavailable capability, explain the limit and ask for the necessary action; never claim it was performed. Visual examples of transitions are not working prototypes.

## 1. Identify the component and target frames

Determine two independent choices from the user's request: operation (create from placeholders or revise existing documentation) and scope (all blocks, one block, or several named blocks). Creating a specification does not require completing every block in the same run. If scope is unclear, ask one scope question before substantive analysis or edits; never silently expand a targeted request to the whole specification.

Examples: “Создай спецификацию с нуля” selects all blocks; “Заполни только passport и construction” selects those two; “Доработай states” revises only states. Follow the live checklist's order within the selected subset. Do not reset or complete skipped blocks. If a selected block needs a fact from another block, reuse available confirmed information or ask one question; do not start editing that other block without authorization.

After resolving operation and scope, establish the source library if it is not already known, then separately ask whether to cross-check against Taiga UI. Ask one question at a time and reuse explicit choices already supplied. A direct request for the cross-check is sufficient authorization to read its public sources. When enabled, read [references/taiga-ui.md](references/taiga-ui.md): resolve the latest stable release at task start, match the component, and apply its source and conflict rules. Do not ask for the company's installed version. When declined, continue the existing workflow without Taiga dependencies. This source choice does not authorize edits or change the selected block scope.

Use the current canvas selection. The user selects only the component, not the templates. Accept a main component, a component set, or an instance belonging to one component. For an instance, inspect the accessible main component and variants, distinguishing instance overrides from general component facts. If selection is empty, ambiguous, or includes unrelated components, ask one question before editing.

Find nearby specification frames on the same page. Match their names, visible titles, internal structure, shared section/container, and proximity. Read [references/block-map.md](references/block-map.md) when resolving scope and identifying frames: it is the shared map of the eight blocks, aliases, roles, and associated checklist items. Check-list is the review/routing frame, not an additional specification block.

Proximity alone is insufficient. If several sets fit, a frame needed for the selected scope is absent, or placeholder status is unclear, ask which frames to use before affected edits. Missing frames outside scope do not block targeted work. Use the live checklist to identify whether a block was populated: an item with neither `done` nor `reject` marked means its block has not yet been filled, even if the frame contains component-specific text and examples. A `reject` status means the block was reviewed with a finding; it is not an empty template. The supplied specification templates use a filled `date-picker` specification as a reference for content and visual structure. Treat reference content in an unfilled block as replaceable template material, whether documenting `date-picker` or another selected component. Replace its component-specific text and demonstrations within the selected scope while preserving the template structure and protected designer-owned fields. Do not treat reference behavior, values, or statuses as confirmed facts without checking the selected component and user requirements. For genuinely completed documentation of the selected component, do not overwrite it as a placeholder; clarify the intended action if the user requested creation.

Keep the identified source and target frames fixed throughout the task. A later selection change does not automatically switch the task. Do not fetch templates from another file unless the user supplies or authorizes that source.

## 2. Inspect, review, and clarify

First read only enough of the checklist and nearby frame names to identify the block mapping and selected scope. For the current block, inspect the relevant layer structure, properties, variants, layout, styles, bindings, and behavior. Do not load the whole page, all templates, or unrelated component data for each question. Reuse confirmed facts while checking that the source has not changed before an affected edit. Do not infer runtime interactions solely from appearance. Ask about information unavailable in the design when the current block requires it.

Use the live checklist's block annotations and order as the workflow, not an independent sequence of individual checklist rows. Use the grouping in the block map; do not maintain a second independent order here.

Read annotations with their grouping/brackets, not just text traversal order. If the supplied checklist has changed, follow its unambiguous mapping; ask about conflicting or missing annotations instead of guessing. Work only on selected blocks, preserving this relative order.

For each block:

1. Identify the current block and its associated checks. Read only its required source and template data. When Taiga cross-checking is enabled, also consult the relevant evidence for this block under [references/taiga-ui.md](references/taiga-ui.md), keeping Figma observations, Taiga facts, and confirmed corporate requirements distinct. Include compact source attribution in the block draft; the existing approvals and checks still apply.
2. Clarify missing information, one question at a time, waiting after each answer. Respect explicit deferrals under references/findings.md instead of repeating the deferred question. Handle component problems through separate fix approval.
3. Assemble a concise draft of this block's content, relevant demonstrations, its bottom «Замечания и спорные моменты» subsection when needed under the findings rules, and checklist findings. Show it in Codex and ask for approval before writing it to Figma. Do not begin other blocks while waiting.
4. In create mode, write only the agreed block. In revise mode, retain the per-change approval rule: describe and obtain permission for each concrete change; an overall draft approval does not waive it. If a draft explicitly presents one concrete change, its approval can authorize that change without a duplicate question.
5. Verify the changed frame and associated checks. Update only this block's checklist entries; in revise mode, checklist changes need approval too. Preserve the remaining blocks, their content, and their statuses.
6. Report the block's result and ask one explicit question about moving to the next selected block. Wait. Approval of a draft is not approval to advance. If no selected blocks remain, finish the requested scope without offering the unselected remainder as unfinished mandatory work.

If the user pauses or changes scope, keep the current block's status and approvals clear; resume at the last unfinished step. A change affecting an approved draft requires renewed approval for the changed content.

Use the component's confirmed requirements to judge applicability and completeness. An example component's state list or token values are not universal requirements. Confirm a token's currency against the supplied or accessible source of truth; binding to a variable alone does not prove currency. Separate design inspection from implementation testing: do not certify screen-reader support, keyboard execution, or production behavior from a static mockup.

Record verified compliance, findings, and unresolved checks using the template's available status treatment. Do not mark an item passed before it is checked. Unknown essential information triggers one clarification question. Confirm non-applicability before marking a section or check “Не применимо”.

Pause for approval whenever a problem is found, following the authorization rules above. After an approved fix, inspect the changed result and update only facts actually established.

## 3. Fill the specification

The descriptions below define block content, not a second execution order. Execute only selected blocks in the checklist mapping above and use the approval cycle for each one. Replace placeholder facts and demonstration content with facts about the selected component. Preserve references' visual structure, not their example behavior.

### Passport

Read [references/passport.md](references/passport.md) for field-specific rules when working on this block. Preserve the passport heading, General info fields, Guides, and the history region. Draft clear values independently; ask or propose uncertain values for agreement. Name comes from the component; determine Level as element/component/pattern. For design and development readiness, separately ask the user to choose one of exactly `to do`, `in progrees`, or `ready`; preserve these labels and do not infer a mapping from other answers. The designer owns Owner, Last change, and change history: leave all three untouched, including sample or empty values. Do not treat them as unfinished placeholder cleanup.

### Anatomy / Construction

Read [references/construction.md](references/construction.md) for this block and its linked measurement-tool guidance when placing annotations. Preserve the supplied size/anatomy layouts and Tools for spech palette. Show all existing component sizes and extract nested components for dimension demonstrations. Check every layer's color, font/typography, and size bindings internally; in anatomy publish only attention findings, grouping identical repeated issues. Do not print correctly bound layers or a complete layer/token registry. Replace sample content with real component data; use the palette's annotation instances with real measurements. Do not change source components or token bindings without the separate required approval.

### States

Read [references/states.md](references/states.md) for this block. Cover states of the selected component and its nested components, clearly identifying which part owns each state. Group related demonstrations into named state blocks using the live template. Describe conditions, visible changes, and behavior in plain language; do not publish token-to-token comparisons or raw parameter diffs.

Inspect layer roles and hierarchy before comparing parameters; do not confuse internal-wrapper padding with the component frame's padding. If only internal elements change state, use a short general description of that fact and keep their details in their own sections.

Preserve the States heading, subtitle, and the user's current grouping and grid layout. Each state block contains a title, a concise description of conditions/behavior, and paired demonstrations in a shared card. Show the relevant baseline and target side by side, with clear labels and consistent configuration/content apart from the documented state change. Exclude impossible combinations even when source variants exist; record conflicting source definitions in the bottom findings subsection without changing them automatically.

Describe actual and agreed states. Normal, Focus, Hover, Pressed, Loading, and Disabled are template examples, not mandatory for every component. Do not copy sample focus thickness, opacity, tokens, desktop restrictions, or button behavior. Clarify unknown triggers, keyboard behavior, transitions, and limits. Use real states or confirmed examples; do not fabricate a missing state by changing the source without approval.

### Variants

Read [references/variants.md](references/variants.md) for this block. Preserve the Variants heading, subtitle, and repeated description-and-demonstration blocks. Show every existing combination of variant properties using a real variant instance and describe its purpose and conditions of use individually; do not reduce coverage to representative examples. A separate differences section is not required. Use source facts and confirmed answers. Do not invent absent combinations or confuse instance overrides with variant axes. Replace copied placeholder state descriptions with relevant variant documentation.

### Responsive

Read [references/responsive.md](references/responsive.md) for this block. Preserve the Responsive heading. When the supplied frame has only a heading, extend the visual system of neighboring specification frames with rule descriptions and demonstration cards.

Describe actual auto layout, resizing, minimum/maximum dimensions, wrapping, overflow, and supported contexts. Ask about unknown rules and relevant demonstration widths. Do not invent breakpoints. Resize demonstration instances or their containers within supported behavior; do not alter the main component to make a demonstration work.

### Edge cases

Read [references/edge-cases.md](references/edge-cases.md) for this block. Preserve the Edge cases heading. For a heading-only template, use descriptions and demonstration cards consistent with the other frames.

Document relevant, confirmed boundary inputs and expected behavior. Long or empty content, optional parts, and exceptional constraints are candidates to assess, not universal requirements. Ask when expected behavior is unknown. Findings requiring component changes follow the pause-and-approval rule. Do not present a proposed behavior as an existing behavior.

### Accessibility

Read [references/accessibility.md](references/accessibility.md) for source-backed UX recommendations, their impact, and tradeoff reporting. Preserve the accessibility heading, explanatory content, and demonstration area. Document practices relevant to the actual component and confirmed implementation requirements. Distinguish observed design facts, implementation recommendations, and results actually tested. Clarify the applicable standard and unknown interaction semantics. Do not copy sample search-field guidance into an unrelated component or claim runtime accessibility testing from the design alone.

### Animation

Preserve the animation heading and existing description/demonstration structure. Describe confirmed triggers, transitions, affected properties, timing, duration, easing, interruption behavior, and reduced-motion behavior where relevant. When library cross-checking is enabled, first investigate extractable animation facts through [references/taiga-ui.md](references/taiga-ui.md), including shared styles and tokens. Ask about product choices and parameters still unavailable after that investigation; do not copy sample values. If animation is not applicable, agree that conclusion. Demonstration frames and descriptions do not establish that a working prototype or implementation has been tested.

### Finalize the checklist

Finalize only the current block's checklist results after its agreed content and approved fixes are complete. Preserve the checklist's title, item order, grouping, and block annotations. Keep detailed findings and unresolved decisions in that block's bottom «Замечания и спорные моменты» subsection under the shared findings rules; use checklist statuses and a short pointer only when useful. Do not expand checklist labels in ways that break grouping or duplicate the full findings list. In update mode, changes to checklist content or statuses also require individual approval. Never mark checks belonging to unselected or unprocessed blocks as completed.

## 4. Preserve layout and verify

Keep the existing frames beside the component on the same page. Preserve frame identity, section order, hierarchy, styles, visual relationships, and layout conventions. Adapt text, measurements, demo instances, and the number of repeated blocks to confirmed data. Adjust height and auto layout to fit content without clipping; do not redesign unrelated content. In update mode, layout adjustments are changes requiring approval too.

Before presenting a change for approval, inspect both text and related demonstrations in the current block for unrelated template components, labels, and behavior. Present required text, demo, and associated layout changes concretely under the existing revision approval rule. Use real instances; label a static demonstration as static rather than implying a working transition.

Before writing, recheck the target node and current text. Load every font used by the edited text runs; a mixed fontName is not a font to load. Preserve or restore applicable hyperlinks, range token bindings, emphasis, and paragraph/list formatting after replacement. Correct accidental empty bullets or inherited formatting within the approved edit, without restyling unrelated content. Verify text, links, instance relationships, protected content, and the rendered result afterward.

Use real properties of the supplied frames for visual matching. Do not treat example photographs, links, or illustrations as part of the selected component's facts. Preserve the shared visual system when expanding initially empty sections. Do not delete a required section merely because it may be inapplicable.

Inspect the resulting canvas for:

- Correct source component and target frames.
- Every section and checklist item within the agreed block scope addressed; other blocks left untouched.
- No unrelated placeholder facts, examples, or copied state rules remaining in the editable scope; explicitly protected regions such as designer-owned history remain unchanged.
- Accurate instances, annotations, properties, and measurements.
- Readable text, correct wrapping, no clipping or overlap, consistent alignment and spacing.
- No unapproved changes to the source, finished documentation, or unrelated nodes.
- A bottom remarks/open-points subsection only in blocks with substantive findings, improvements, or open questions; accurate statuses and no duplicated finding inventories. Do not automatically remove an existing subsection without revision approval.

Correct assembly errors within the already authorized scope. In update mode, ask again if a correction goes beyond the specific approved change. Do not report a visual check you could not perform.

End with a short Russian report naming the reviewed blocks and approved documentation/source changes. Separately identify confirmed corporate differences from the library, retained findings and explicitly deferred decisions, and checks not performed. Distinguish a completed review from complete requirements or a ready component, and design/source inspection from tested implementation behavior. When reviewing a cross-check trial, distinguish evidence that the skill worked from evidence that the product implementation worked. Explicitly deferred requirements may remain after the agreed review finishes, with their status reported honestly. For essential unknowns not explicitly deferred, ask the next single clarification question rather than claiming completion.
