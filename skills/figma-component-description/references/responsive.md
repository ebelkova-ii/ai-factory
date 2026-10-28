# Responsive Filling Rules

Read when working on responsive behavior. Follow the block map, approval cycle, and shared findings rules. Inspect only the current component, relevant nested layout, and this block's template.

## Establish the rules

Separate observed dimensions/settings from confirmed requirements. A component being 340 px wide in one example does not establish a fixed-width rule. Inspect auto layout, resizing, min/max dimensions, wrapping, clipping, and relevant overflow; ask about intended behavior that the source cannot establish. Do not infer breakpoints or supported widths from example labels or unrelated design-system variables.

Distinguish fixed dimensions from dimensions determined by content. A content-sized frame may retain the same resulting height because its row/item count is constant. Describe that dependency accurately rather than calling its height fixed. When content quantity changes, clarify which parts resize and which dimensions, spacing, or cell sizes remain unchanged.

Distinguish reuse of the same component on mobile from its presentation container. Using the same component does not establish a popover, bottom sheet, breakpoint, or change in width. If the user explicitly defers a decision, retain it as an open point in the bottom findings subsection and continue only with established facts; do not mark the overall responsive requirement fully agreed.

## Fill and demonstrate

Preserve the Responsive heading and the live template's description/card treatment. Replace unrelated sample content with groups for the actual resizing rules and confirmed contexts. Reuse confirmed information instead of repeating the brief. Describe dependencies and limits plainly; do not duplicate construction's full geometry inventory.

Use real component instances and representative content that produces each agreed layout. For a calendar, the displayed month/year, weekday alignment, and number of required week rows must agree. Adapt demonstration content and supported instance overrides; do not change the source or force a dimension merely to simulate an unconfirmed rule. Do not present static examples as a working responsive implementation.

When annotating dimensions, use the supplied palette under [measurement-tools.md](measurement-tools.md). Measure each assembled example and set its annotation to that actual value; do not rely solely on a predicted height. Preserve source instances, layout settings, and the Tools palette. Verify source/instance distinctions, content, bounds, annotations, and visual layout after assembly.

End with «Замечания и спорные моменты» under [findings.md](findings.md). Keep observations, hypotheses, confirmed requirements, and unresolved decisions distinguishable. Preserve deferred questions rather than inventing a solution or removing them after a demonstration succeeds.
