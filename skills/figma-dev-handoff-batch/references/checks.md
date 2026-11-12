# Ten areas in one analysis

Use the entrypoint's onboarding, shared dataset, autonomous edits and single grouped decision package. The areas below describe coverage, not sequential approvals. Reuse findings across areas instead of asking the same question twice. Honor requested skips; do not make this run's skipped areas permanent defaults. Follow the live checklist order when it differs from the reference order; preserve its wording and legacy numbering.

## 1 — Флоу и навигация

Read relevant prototype links and supplied explanations. Establish entry points, actions/triggers, destinations/results, return/cancel/exit and alternatives where applicable. Appearance does not establish behavior. Put unknowns into the product-rules questionnaire; document confirmed non-obvious rules by targets. Do not narrate adequate existing navigation or demand a new prototype.

## 2 — Сборка и названия слоёв

Inspect semantic composition, hierarchy, grouping, duplicate elements, grid/alignment, auto layout, fixed/hug/fill, constraints, padding/gaps, overlays, clipping and scrolling. Distinguish wrapper spacing from component padding. Hidden content is not automatically unnecessary. Do not impose auto layout everywhere or arbitrary integer sizes.

Rename meaningful page-owned containers, text layers and own elements autonomously. Preserve library/technical contracts. Skip vector paths and unused hidden drafts. Put actual structural/layout corrections, including duplicate removal and sizing changes, into the correction group; no silent rebuilding.

## 3 — Компоненты

Inventory component families used directly by the page and significant dependencies of local components. List ready-made global Header/Footer as components without expanding their icon/browser/decorative internals. Inspect a nested part only for a specific issue, overridden product content or necessary local construction. Exclude Note, measurement and documentation families.

Use actual main-component relationships for local/library provenance; do not guess from names. Deduplicate variants of a family, recording relevant usage variants. Preserve exact original names. For local components include verified source links and identify coverage among the objects the designer has prepared in construction; record missing objects without adding instances. For library components reuse known source links, then make at most one source-resolution attempt per needed unknown family. On failure retain the original name without a component link and continue: no retries, alternate search chains or repeated token diagnosis. Use a verified common library link if available, clearly distinguished from individual component links. Missing source links alone are not a review blocker; distinguish that from unknown component behavior or missing construction coverage. Do not audit all tokens/styles/unused variants.

## 4 — Конструкция

Check available actual geometry/layout properties in the agreed scope for fractional values: local x/y coordinates, width/height, padding on each side, Auto Layout gaps and corner radii. Use property values from the shared dataset, not visual estimates or fractional absolute bounds produced by ancestor transforms. Preserve existing traversal and library boundaries; report unavailable properties or uninspected coverage honestly.

By default, leave fractional values unchanged and record them in the agreed findings area using [figma-output.md](figma-output.md): property name, exact observed value and a clickable link to the affected Figma node. Group equivalent findings only with labeled location links. If an exact link is unavailable, use the nearest established location and state the limitation; never invent a URL. Retain confirmed project exceptions or responsive/Fill calculation context alongside the observation: a fractional value alone does not establish a defect. Do not impose integer sizes or propose blanket rounding as a required fix. Any correction requires explicit approval of exact target values; general approval of handoff output is insufficient. Keep unresolved findings in the construction status under the existing checklist rules, without changing checklist text.

Use the prepared `constraction` and actual reference tools under [figma-output.md](figma-output.md), including its placement lanes and distinction between dimensions, local gaps, global spacing, padding and radii. Keep diagrams detailed and legible: parts, widths, individual-element heights, radii, gaps, padding, fixed/hug/fill, confirmed percentage widths with an explicit viewport/container reference, and confirmed flexible constraints. Do not annotate the overall height of a complete screen/page. Numeric information belongs in measurement tools, brief construction explanations in Notes. A current rendered size is not a universal fixed size or min/max.

Annotate one fullest valid designer-prepared configuration per equivalent construction; retain necessary nested measurements and show meaningful size differences on the prepared objects. Do not add or copy screens, product components or images into construction, even to complete coverage. Reuse existing sufficient diagrams and explicitly identify shared coverage. Record missing configurations or objects for the designer to supply, and continue with the available set. Place component lists in the same construction without reproducing library specifications. Reuse this specification for behavior, responsiveness and copy constraints.

## 5 — Состояния и поведение

For relevant states establish owner, trigger/condition, visible change, available actions and result. Consider normal, loading, error, success, empty, disabled, hover/focus/pressed, validation and optional-content rules only where applicable. Do not require every state or skeleton everywhere. Variants alone do not prove valid behavior combinations.

Group missing rules such as validation timing, sending/retry, persistence and visibility into product questions. Missing UI messages remain requirements/findings; do not invent text. Supplement existing Notes/construction with confirmed behavior. If additional examples are needed, record them for the designer to supply; do not generate or add product examples to construction.

## 6 — Адаптивность и крайние случаи

Read the applicable project responsive contract before assessing widths or proposing corrections: reference design widths, runtime breakpoints, grid, units, sizing behavior and any separate compositions or legacy exceptions. Use these documented rules without re-asking established values; include only missing essentials or concrete source conflicts in the questionnaire. Do not impose standard device widths or infer limits from one size. Read counterparts outside scope only with narrow authorization.

Evaluate layout dimensions and behavior against the applicable project requirements. Do not classify an individual Figma property as a defect without implementation context and supporting evidence. Cite the relevant project rule for findings and proposed corrections, and distinguish observed design properties from tested runtime behavior; documentation alone does not prove implementation behavior.

For each equivalent rule group inspect one fullest representative and meaningful differences: resizing, wrapping, rearrangement, clipping/overflow, scaling, scrolling and fixed/hug/fill/min/max. Exercise applicable long/short/empty/dynamic content, hidden blocks and missing images using confirmed behavior and the same designer-prepared control set; do not create additional copies to fill missing cases. Do not invent test lengths or fallback rules. Static data alone does not establish tested resizing. Record unexercised cases honestly. Do not silently rebuild the source.

## 7 — Грамотность и типографика

Follow [text-review.md](text-review.md). Check spelling, grammar, punctuation and typography; exclude editorial rephrasing, shortening, tone changes and comments suggesting new formulations. Compare actual characters across all corresponding in-scope device, breakpoint and theme variants for matching scenarios/states/data, including the exact positions of explicit line breaks, nonbreaking spaces binding prepositions and other word groups, and nonbreaking hyphens (U+2011). These must match the selected source unless an exception was explicitly approved; automatic wrapping is not an explicit line break. Use the onboarding source for autonomous parity; unresolved canonical text enters the questionnaire.

NBSP corrections can be autonomous. Other exact replacements enter the proofreading group with location, before/after and reason. Preserve variables, values, links and semantics. Reuse construction/responsive evidence for wrapping and actual text-container constraints; do not invent character limits or repeat post-write comparisons.

## 8 — Изображения и ассеты

Reuse prepared images and inspect meaningful versions/crops, completeness, export boundaries, masks, proportions, transparency and names. Record missing images or versions for the designer to supply; do not add or copy them into construction. Propose needed export settings only for the prepared asset set; never remove source images or masks. Do not export every library icon or component.

Prepare agreed raster formats at 2x, preserving vector formats without mechanically applying 2x. Source resolution and actual export settings matter; a heading is not a setting. Document fit/fill/crop, alignment/anchors, scaling/focal point and meaningful responsive differences once in construction. Keep agreed brand restrictions. No bulk export/archive unless explicitly requested; do not claim actual file quality/weight checked without inspecting files. Report unknowns/skips separately.

## 9 — Доступность

Use agreed requirements. Consult current primary normative sources for numerical/compliance claims when needed; do not impose a blanket target size or infer conformance. Inspect applicable contrast with actual backgrounds/opacity, visible focus, labels/accessible-name requirements, target size/separation, non-color information and intended interaction/reading order. Reuse state/copy data. Record concrete issues or essential questions in the shared package. Static designs do not prove DOM/ARIA, keyboard, screen-reader behavior or runtime hit areas.

## 10 — Анимация

Use accessible prototype/motion settings and confirmed flow/state rules. Absence of settings does not automatically mean non-applicable. For distinct applicable transitions document trigger, affected elements/properties, endpoints, duration, easing, relevant delays/interruption and reduced-motion rules. Group equivalent transitions. Missing material rules enter the questionnaire; never invent motion. Changes to prototype/animation need approval. Reuse Notes/construction; do not require video or new demonstrations.
