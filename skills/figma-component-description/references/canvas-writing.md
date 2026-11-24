# Figma API Safety, Canvas Writing and Verification

Read once before the first API inspection; reuse when writing. Use the scope, concrete approvals and dependencies in [SKILL.md](../SKILL.md). These rules govern assembly and verification; they grant no additional editing permission.

## Safe collection

Use APIs compatible with the connected document mode: in `dynamic-page`, resolve instance sources with `getMainComponentAsync()` rather than the synchronous getter. Inspect actual capabilities instead of assuming a fixed API surface.

Guard getters individually. Cache a component-set schema failure and do not repeat the same failing `componentPropertyDefinitions`/`variantProperties` access across its variants. Preserve the complete structural inventory; use names as explicitly labeled fallback evidence, not verified definitions. Failed access proves neither absence nor permission to repair the source. Retry only with materially new evidence or capability.

Before returning data through the bridge, normalize mixed/symbol sentinels into explicit markers. Preserve real values, errors and per-run/per-occurrence coverage; do not serialize a sentinel as a font, token or measurement. Read actual text runs where mixed styling matters.

## Preserve and guard

Keep source/target identities, same-page placement, section hierarchy, styles, layout conventions and unrelated content. Adapt repeated cards, height and auto layout only within the described approved output. Preserve Owner, Last change, the whole history region and Tools for spech, including samples. Never treat protected contents as unfinished cleanup. Compare protected text, identities, bindings and authored layout settings separately from computed bounds. Approved normal Auto Layout reflow may move history or change Fill widths without changing protected contents/settings; do not force fixed geometry to make a snapshot match. Actual unauthorized content/settings changes still require recovery.

Before overwriting, narrowly check the actual target identity/type and affected text/properties against the approved before-state, preferably in the bounded write operation. An external change requires refreshing affected facts and resolving a materially changed proposal before overwriting. Do not reload all source/templates for every mutation. Use successful write results to update known values and IDs.

Load every actual font used by edited runs; a mixed fontName sentinel is not a font. Cache loaded fonts and exposed properties. Preserve or restore hyperlinks, range token bindings, emphasis, styles and paragraph/list formatting during replacement. Fix accidental empty bullets or inherited formatting only within the approved change. Do not restyle unrelated content.

## Demonstrations and measurements

Use real instances with supported properties/overrides and accurate source relationships. Never detach or alter the main component to make an example work. Replace unrelated template components, labels and behavior as well as text within the editable approved scope. Treat template photographs, illustrations and links as presentation, not component facts. Label static demonstrations as static; they do not establish a working transition or tested implementation.

Retain required coverage: every existing variant combination and size, necessary nested parts, valid paired states and agreed responsive/edge cases. Shared evidence does not authorize representative-only demonstrations. Use the live template's grouping/grid, typography, spacing and card treatment; extend it consistently for heading-only sections. Do not delete required sections because applicability is unknown.

For annotations, read [measurement-tools.md](measurement-tools.md) when needed and inspect the live palette contract once. Use real annotation instances with actual dimensions, padding, gap and radius values from the represented target, not template defaults or screenshot estimates. Keep tools editable, oriented/anchored to the correct span/side/corner and readable. Distinguish source geometry, demonstration geometry and annotation geometry. Do not substitute drawn imitations or images for available tools.

## Bounded writes and recovery

Apply approved independent objects in bounded batches; execute dependencies sequentially. Do not assume transactions, rollback or unsupported API operations. Source fix → immediate affected propagation check → dependent demos/docs; a materially changed draft needs a focused renewed approval.

After a partial failure, retain successful results and inspect only the failed target/dependency. Do not replay the entire package or repeatedly retry an inaccessible source without new evidence. Clean only artifacts created by the failed attempt; never remove existing user content. Fix assembly mistakes within the already authorized result. Recovery requiring new content, layout or scope needs a concrete decision.

## Consolidated output verification

Use the shared coverage record and successful write results, then inspect changed frames in one consolidated pass; split large regions into bounded views without losing coverage. Check:

- Correct identities and approved scope; protected and unselected content preserved.
- Accurate text, links, relevant range formatting, source-instance relationships, properties and actual measurements.
- Complete required sizes/variant combinations/nested demonstrations and the relevant block-specific checks; no unrelated editable placeholders or copied behavior.
- Rendered readability, wrapping, clipping, overlap, alignment and spacing of text, demonstrations, cards and annotations together.
- Substantive remarks only, no duplicate full findings inventories, and checklist results supported by actual inspection.

Use rendered views of changed areas for visual QA. Successful API writes or bounds alone do not prove visual quality. Do not screenshot every question, revisit unchanged frames routinely or repeat the full source audit. Actual write errors, suspect geometry and source propagation need immediate narrow verification rather than waiting for the final pass. After correcting an error, recheck the affected result.

Verify approved source fixes across affected source variants, nested parent instances and existing demos. Read the propagation subsection of [states.md](states.md) if needed; do not start an unrelated full block review. Preserve intentional overrides and report failed propagation honestly.

For checklist preservation, compare row identity/mapping, wording/order and expected status semantics. A native variant swap may replace descendant IDs; changed child IDs alone are not a wording failure or reason to replay successful writes. Finalize only authorized results supported by each check under SKILL.md. Do not set planned completion when inspection fails; leave it pending unless the concrete unresolved result was authorized. If render, links, source access or any required check cannot be verified, state the specific limitation. Never claim an inspection, source fix, working prototype or runtime test that did not occur.
