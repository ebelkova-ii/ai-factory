# Conditional Remarks and Open Questions

Read when drafting or updating any specification block. This shared rule applies to passport, construction, variants, states, responsive behavior, edge cases, accessibility, and animation. It supplements the block-specific guidance without authorizing edits outside the selected scope.

## Placement and appearance

When a processed block has actual findings, required improvements, or material open questions, end it with a subsection titled «Замечания и спорные моменты», inside that block's frame, after its main content. Reuse the visual treatment of the construction token-attention cards: existing text styles, card backgrounds, corner radii, spacing, and, where useful, a relevant part demonstration. Use available nearby template cards as style references; do not modify the reference block just to reuse its appearance.

When needed, this subsection may be added even if the original template lacks it. Do not add it when there are no substantive entries. Preserve the surrounding layout and adjust auto layout/height to fit. For passport, place it outside and after the designer-owned history area; Owner, Last change, and the history region remain untouched. Normal container reflow is permitted within approved layout adjustments; do not edit protected content.

In construction, use this bottom subsection as the home of its token-binding attention cards. Do not duplicate the same full finding in both anatomy and the bottom subsection. Preserve the size demonstrations and the meaning of the existing anatomy section; use a short pointer when useful.

## Entries

Include only actual findings and material open questions, not a catalogue of correctly configured layers. For each entry, state concisely:

- A clear title and category: «Замечание» for an established defect, «Спорный момент» for an unresolved interpretation or decision, or «Доработка» for required work not yet designed or implemented. Never present uncertainty as a proven defect.
- The affected component/part/property, with enough location context to find it.
- What is observed and, when established, what is expected. Show relevant values or token names, not a full inventory of unchanged properties.
- The decision/status actually agreed: needs clarification, fix approved but pending, retained without correction, or fixed and verified. Do not claim a fix solely because it was approved.

For an unbound color, retain its actual HEX code and attention note; for unbound fonts or sizes, retain the actual values and applicable attention note. Group repeated identical issues with their count and a locatable description; preserve detailed IDs in local task evidence rather than listing them all on the canvas. Do not merge materially different values or cases.

Keep required behavior in the main specification text. Put source defects and decision disputes in this bottom subsection, with a short pointer beside a demonstration only when needed to avoid mistaking a defect for intended behavior. A source defect is not a reason to describe that defect as the expected state change.

If the block was checked and no substantive entries remain, do not create a subsection or a no-findings message. Removing or clearing an existing subsection in revision mode is a concrete change requiring approval. Incomplete checks must still be disclosed as material limitations or open checks; omitting an empty subsection does not establish compliance.

## Workflow and permissions

When needed, include this subsection in the block draft and its approval. In revision mode, adding or changing entries follows the per-change approval rule. Its presence does not waive pauses for questions, authorize source-component fixes, or allow unresolved essential facts to be replaced by an open-question list while claiming completion.

Maintain findings in the current block only. If the same issue is relevant elsewhere, reuse known evidence and use a short reference when that other block is in scope; do not rewrite completed or unselected blocks automatically. Align this block's checklist statuses with retained findings, without changing item order or grouping annotations. Recording a finding does not mean the source passes the corresponding check.

## Explicitly deferred decisions

A user request such as “add this to remarks” authorizes recording the described question or improvement at the identified location. It does not confirm the proposed behavior, approve a source change, or waive later approvals. If the content or location is ambiguous, ask one clarification question before writing.

Record what is known, what remains undecided, its effect on the specification, and the actual status. Reuse confirmed facts and do not invent error messages, visuals, timing, or applicability. Keep conditional scenarios conditional until their applicability is established.

After an explicit deferral, continue with the confirmed portion without repeatedly asking the same question. Retain the separate approval to advance to the next block. A review may finish with disclosed deferred work, but unresolved requirements must not be called complete, checks passed, or the component ready. If the unknown prevents even a safe limited description, explain that dependency and agree the limited record or scope. Do not use this path to bypass an essential unknown the user has not deferred.
