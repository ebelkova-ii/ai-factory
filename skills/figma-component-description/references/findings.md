# Conditional Remarks and Open Questions

Read once for the selected scope. These rules govern remarks in all eight blocks; [SKILL.md](../SKILL.md) governs questions, scope and approvals.

## Placement and appearance

Only substantive findings, required improvements or material open questions justify a bottom «Замечания и спорные моменты» subsection inside the affected block. Reuse nearby construction attention-card text styles, backgrounds, radii and spacing, with a part demonstration where useful. Do not modify the reference block to copy its appearance.

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

Include entries in the concrete documentation package; identify revise additions/edits/removals individually, even when approved together. An entry authorizes neither a source fix nor a completion claim with essential unresolved facts.

Place each finding in its affected selected block. If the same issue is relevant elsewhere, reuse known evidence and use a short reference when that other block is in scope; do not rewrite completed or unselected blocks automatically. Attribute each retained finding/deferral to its affected checks and dependencies, preserving order/grouping. Do not reject every check in a block for one unrelated issue. Separate unperformed checks from verified defects using the actual template status semantics; a finding never establishes compliance.

## Explicitly deferred decisions

A user request such as “add this to remarks” authorizes recording the described question or improvement at the identified location. It does not confirm the proposed behavior, approve a source change, or waive later approvals. If content or location is ambiguous, request the focused missing decision before writing.

Record what is known, what remains undecided, its effect on the specification, and the actual status. Reuse confirmed facts and do not invent error messages, visuals, timing, or applicability. Keep conditional scenarios conditional until their applicability is established.

After an explicit deferral, continue with the confirmed portion without repeatedly asking the same question. Apply approved independent output without transition gates; keep affected dependencies unresolved. A review may finish with disclosed deferred work, but unresolved requirements must not be called complete, checks passed, or the component ready. If the unknown prevents even a safe limited description, explain that dependency and agree the limited record or scope. Do not use this path to bypass an essential unknown the user has not deferred.
