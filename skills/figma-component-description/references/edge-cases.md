# Edge Cases Filling Rules

Read when working on edge cases. Follow the block map, block approval cycle, and shared findings rules.

## Select relevant cases

Derive cases from the component's purpose, inputs, actual states, and confirmed usage scenarios. Establish which constraints belong to the component and which are supplied by its host scenario; do not convert example limits into universal component rules. Template examples are structural references, not required scenarios for every component.

Ask about unknown applicability and expected behavior one question at a time. Explain a hypothetical case with a concrete example when needed, then confirm that it applies. Exclude cases the user says are irrelevant to the current scenarios without treating that answer as a universal guarantee for every use of the component. Do not impose an exhaustive generic catalogue.

Distinguish a locally unavailable option or period from no available result anywhere in the scenario. If recovery requires finding an available result, consider what happens when none exists and clarify that outcome. Do not invent search direction, fallback selection, errors, limits, or recovery behavior.

## Describe and demonstrate

For each applicable case, state its condition and confirmed expected behavior. Preserve the Edge cases heading and the live template's description-and-card treatment. Replace unrelated example content with the actual component's cases.

Use real instances and internally consistent sample content. When helpful, show the triggering condition and expected result as a pair with clear labels. A condition illustration is not necessarily a screen on which the interface should remain. Static examples document the agreed behavior; do not claim they implement or verify a working transition.

If the user proposes a message or an empty state whose visual design is unresolved, distinguish the candidate text from approved component UI. Label any demonstration as preliminary, retain the exact agreed text, and put the unresolved presentation decision in the bottom findings subsection. Do not silently add a new state to the source component or claim the design is finalized.

## Verify and retain open points

Check demonstrated content, variant flags, source-instance relationships, and layout. Verify that unavailable items are not shown selected where that combination is prohibited, and that a claimed recovery example actually contains an available result. Preserve source components, completed blocks, and unrelated checklist entries.

Include «Замечания и спорные моменты» only when substantive entries are needed under [findings.md](findings.md); do not add an empty subsection or a no-findings message. Separate confirmed behavior from design proposals and unresolved decisions. Retain user-deferred questions without claiming the corresponding requirement is fully resolved. Report design/specification verification separately from runtime behavior that was actually tested.
