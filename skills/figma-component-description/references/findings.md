# Remarks and Open Questions in Every Block

Read when drafting or updating any specification block. This shared rule applies to passport, construction, variants, states, responsive behavior, edge cases, accessibility, and animation. It supplements the block-specific guidance without authorizing edits outside the selected scope.

## Placement and appearance

End each processed block with a subsection titled «Замечания и спорные моменты», inside that block's frame, after its main content. Reuse the visual treatment of the construction token-attention cards: existing text styles, card backgrounds, corner radii, spacing, and, where useful, a relevant part demonstration. Use available nearby template cards as style references; do not modify the reference block just to reuse its appearance.

This subsection is now an agreed part of the output even if the original template lacks it. Preserve the surrounding layout and adjust auto layout/height to fit. For passport, place it outside and after the designer-owned history area; Owner, Last change, and the history region remain untouched. Normal container reflow is permitted within approved layout adjustments; do not edit protected content.

In construction, use this bottom subsection as the home of its token-binding attention cards. Do not duplicate the same full finding in both anatomy and the bottom subsection. Preserve the size demonstrations and the meaning of the existing anatomy section; use a short pointer when useful.

## Entries

Include only actual findings and material open questions, not a catalogue of correctly configured layers. For each entry, state concisely:

- A clear title and category: «Замечание» for an established defect, «Спорный момент» for an unresolved interpretation or decision. Never present uncertainty as a proven defect.
- The affected component/part/property, with enough location context to find it.
- What is observed and, when established, what is expected. Show relevant values or token names, not a full inventory of unchanged properties.
- The decision/status actually agreed: needs clarification, fix approved but pending, retained without correction, or fixed and verified. Do not claim a fix solely because it was approved.

For an unbound color, retain its actual HEX code and attention note; for unbound fonts or sizes, retain the actual values and applicable attention note. Group repeated identical issues with their count and a locatable description; preserve detailed IDs in local task evidence rather than listing them all on the canvas. Do not merge materially different values or cases.

Keep required behavior in the main specification text. Put source defects and decision disputes in this bottom subsection, with a short pointer beside a demonstration only when needed to avoid mistaking a defect for intended behavior. A source defect is not a reason to describe that defect as the expected state change.

If the block was actually checked and no findings or unresolved points remain, keep the subsection with «Замечаний и спорных моментов не выявлено». If checks are incomplete, state the unverified scope instead; do not claim there are no issues.

## Workflow and permissions

Include this subsection in the block draft and its approval. In revision mode, adding or changing entries follows the per-change approval rule. Its presence does not waive pauses for questions, authorize source-component fixes, or allow unresolved essential facts to be replaced by an open-question list while claiming completion.

Maintain findings in the current block only. If the same issue is relevant elsewhere, reuse known evidence and use a short reference when that other block is in scope; do not rewrite completed or unselected blocks automatically. Align this block's checklist statuses with retained findings, without changing item order or grouping annotations. Recording a finding does not mean the source passes the corresponding check.
