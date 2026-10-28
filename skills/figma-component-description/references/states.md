# States Filling Rules

Read only when working on the states block. Follow the block map and SKILL.md approval cycle. These rules are being refined with the user sequentially.

## Coverage

Include states of both the selected component as a whole and its nested components, such as date cells and navigation controls. Inspect accessible source definitions of nested components as needed; do not limit coverage to the state currently shown in the selected instance.

Identify which component or part each state belongs to, preserving its exact source/property names. Keep parent states and nested-part states distinguishable. Reuse source information for repeated identical nested components without repeating the same questions.

Do not interpret a variant such as day/year as an interaction state merely because it is a variant property. Do not invent missing states or alter source components without approval.

Validate that combinations are permitted by confirmed behavior, not merely present in the source. Do not blindly enumerate a Cartesian product of flags. For example, if a disabled item cannot be selected, exclude selected + disabled from valid states and demonstrations. Existing contradictory source variants are assembly findings, not proof that the combination is supported. Keep them unchanged without separate fix approval. This state-validity rule is distinct from the variants block's inventory of existing variant combinations.

Check independent indicators as well as interaction states, including their valid combinations where relevant. A current-day/current-year marker is not the same as selection and must not silently disappear from coverage. Derive the actual state families and combinations from the current component and confirmed requirements; do not impose a date-picker-specific list on every component.

## Grouped layout

Follow the user's live state-block structure. Group examples of the same state family under one heading and one concise description, with a shared demonstration card/grid. For a date cell, families may include hover, selected, disabled, weekend, and today; these are examples, not required headings for unrelated components. Do not restore an older layout of one long description per combination after the user has reorganized the template.

Put comparable pairs in the existing grid, with a short context caption above each pair when other flags affect its appearance. Reuse the supplied spacing, typography, and card treatment. Expand only as needed for actual relevant combinations; omit duplicated examples. Identify a different owning part or presentation mode in the relevant caption. A group may show an unchanged appearance when that absence of change is a confirmed rule.

Distinguish two caption roles. In the context/property caption above a demonstration pair, highlight each complete enabled Boolean assignment (for example `weekend=on` or `disabled=on`) with the bound token `text/service/positive/text-service-positive`; keep `off` neutral (`true`/`false` follow the same convention when used by the source). Green means the flag is enabled, not that the example is usable or defect-free. Apply it only to that text range and preserve other styling. Baseline/target labels directly above individual instances stay gray with the template's `text/secondary/text-secondary-normal` token, even when written `selected=on`, `disabled=on`, or `today=on`. Determine the caption's role from its place in the template, not merely the presence of `=on`. Reuse actual reference bindings rather than unbound RGB/HEX colors, and verify range bindings after text replacement. Do not apply this highlighting to component artwork, narrative paragraphs, or enum values such as `state=hover`.

## State description

For each state, describe:

- When it becomes active: confirmed trigger, condition, or restriction.
- What visually changes compared with the relevant baseline of the same part, in plain language (background, number color, marker, or a confirmed absence of change).
- How the component/part behaves while in that state.

Inspect corresponding layers and bindings internally when needed to verify visible changes; distinguish a binding change from a resolved value changing because of a mode change. Do not publish baseline → target token names, token paths, layer-by-layer parameter diffs, or unchanged inventories. Describe state findings visually too, using exact values only where necessary to identify a defect; token-binding audits belong to construction. Clarify an unknown baseline, trigger, behavior, or value one question at a time; do not infer implementation behavior from appearance alone.

Do not publish a raw structural diff as intended state behavior. Different internal wrappers, overrides, or source variants can produce numerical geometry differences without establishing an intended change in padding, size, or radius. Check that compared properties represent the same semantic element and confirm ambiguous geometry changes before including them. When the user clarifies an invariant, omit it from the change list; retain any source discrepancy separately as evidence rather than changing the source without permission. Component-specific values belong in task records, not universal skill rules.

Inspect the actual layer hierarchy before comparing parameters: locate the owning frame, internal wrappers, and the element that visibly changes. Match layers by role and nesting, not just names, array order, or a root-level numeric diff. In particular, distinguish the component frame's padding from padding of an internal wrapper; verify which layer owns each value before describing a padding change.

When the whole component has no state change and state changes belong to its internal elements, keep the general description short: «Состояние целого компонента не меняется. Смена состояний заложена во внутренние элементы». Use this only when supported by inspection and confirmed context. Describe visible changes in the relevant internal-element groups and defects in the bottom findings subsection instead of repeating their inventory or task commentary in the general description.

## Paired demonstrations

Show each state demonstration as a side-by-side pair: baseline/source state → target state. Label both and identify the owning component/part. Use comparable real instances, keeping variant configuration and content consistent except for the state-related changes being documented.

Use the baseline stated in the description. If it is unclear or unavailable, ask instead of inventing a source state. A pair illustrates confirmed appearances; it does not assert a working prototype or a tested interaction. Preserve the template's demonstration-card layout and adapt its repeated blocks to include the pairs.

## Verify consistency and approved fixes

Check confirmed relationships between related elements across all applicable valid state combinations, including independent indicators. If two elements are required to share a color, verify their actual token bindings and resulting appearance: account for resolved modes, paint opacity, and cumulative opacity through their respective ancestor layers. Matching RGB values or token names alone is insufficient. Apply only relationships established for the current component; do not assume every marker must match nearby text. Keep this technical verification internal and report discrepancies under the findings rules.

After an approved source-component fix, verify the affected source variants, nested instances in the parent component, and existing specification demonstrations. Confirm that the fix propagated and inspect local overrides if an instance still differs. Do not silently reset intentional overrides or conceal a source defect by editing only demonstration instances. Verify the affected visuals and bindings before marking the finding fixed; report any propagation problem that remains unresolved.
