# Specification Block Map

Read this compact map when resolving task scope and checklist routing. It records the user-confirmed grouping of the template on 23 October 2026. Detailed field-filling rules will be refined separately with the user; this map does not establish new requirements for a component.

## Block order and checklist ownership

| Order | Block | Checklist items | Purpose | Template content observed |
| --- | --- | --- | --- | --- |
| 1 | passport | «UX/UI вопросы — назначение и правила согласованы»; «Логика контента» | Identify the component and explain its purpose and usage/content rules | General info: Name, Level, design/development statuses, role, last change, Owner; Guides: Usage rules, Content rules; history |
| 2 | construction | «Анатомия — части, размеры и токены описаны»; «Подключены актуальные токены» | Show geometry and nested-part sizes; scan all layers for token-binding issues | Size examples and measurement annotations; anatomy reports only attention findings, with repeated issues grouped |
| 3 | variants | «Вариативность задокументирована и ограничена» | Explain variant differences, purpose, and limits | Repeated variant description and demonstration rows |
| 4 | states | «Есть все необходимые состояния и они описаны»; «Названия properties актуальны и консистентны» | Explain states and review the names/consistency of component properties | State headings, descriptions, and visual demonstrations |
| 5 | responsive behavior | «Responsive поведение понятно и описано» | Explain behavior across relevant widths and resizing conditions | Condition/width headings, descriptions, demonstrations, and annotations |
| 6 | edge cases | «Edge кейсы есть в вариантах и задокументированы» | Explain relevant boundary scenarios and expected behavior | Scenario heading, explanation, and demonstration |
| 7 | accessibility | «Accessibility — описаны лучшие практики для текущего компонента» | Document component-specific accessibility guidance and distinguish it from verified implementation results | Heading, guidance text, and demonstration |
| 8 | animation | «Анимация — описано поведение, параметры» | Document component-specific motion behavior and parameters | Heading, description area, and demonstration; placeholder content must not be treated as approved motion rules |

The Check-list frame controls routing and records review results; it is not a ninth specification block. Its 11 checks belong to the eight groups above. Two checks in one group are worked through as one block before moving onward.

All eight blocks end with «Замечания и спорные моменты» under the shared [findings rules](findings.md). It is a subsection within each block, not a separate workflow block. Reuse the construction token-attention card treatment; include only findings or material open points and group repeats.

## Recognizing frames

Use the actual nearby frames, their titles, structure, and checklist brackets/annotations. Common aliases:

- `passport`: `component passport`, `Сomponent passport`, `General info`, `Guides`, `История изменений`, `history`.
- `construction`: `сonstruction` (including a Cyrillic initial character), `Anatomy`, `Construction`, `Состав`.
- `variants`: `Variants`.
- `states`: `States`, `Состояния`.
- `responsive behavior`: `Responsive`, `responsive`.
- `edge cases`: `Edge cases`, `Edge кейсы`.
- `accessibility`: `Accessibility`.
- `animation`: `Animation`.

These names are routing hints, not fixed node IDs. Do not hardcode the reference file, page, component, or node identifiers. Follow an unambiguous updated live checklist; clarify conflicts rather than silently substituting this map.

## Scope and boundaries

Select all, one, or several blocks from the user's request, independently of create/revise mode. Process selected blocks in their relative checklist order. Missing unselected templates do not block the task. Keep all other blocks and checklist statuses unchanged.

Reuse confirmed facts across blocks without repeating the brief. A need for information from another block is not permission to edit it. In particular, properties reviewed under states may describe variants, and tokens reviewed under construction may be used throughout the component; their checklist ownership does not authorize edits to other documentation blocks.

Within each block, follow the approval cycle in SKILL.md. Detailed writing conventions, field requirements, demonstration coverage, and completion rules are not newly settled by this map. Preserve existing agreed rules until the user refines the relevant block. No screenshot or example value proves behavior of the selected component.

## Block-specific filling guidance

For passport, read [passport.md](passport.md) only when working on that block. Its field rules override earlier general placeholder-cleanup guidance: Owner, Last change, and the history region are protected and remain untouched.

For construction, read [construction.md](construction.md); for measurements, follow its link to the measurement-tool reference. Size coverage, layout, nested-component, and layer/token requirements are recorded there. Unbound colors use their actual HEX code; unbound typography and sizes use their actual values. All receive an attention note. Rules for the remaining blocks await their sequential review with the user.

For variants, read [variants.md](variants.md). Show and describe every existing variant-property combination, not a representative subset. Additional filling conventions are still being refined with the user.

For states, read [states.md](states.md). Include states of both the selected component and its nested components, grouped by state family in the live template. Use concise visual descriptions without token-to-token diffs, paired examples, and only behaviorally valid combinations. Record contradictory source variants as findings.

For responsive behavior, read [responsive.md](responsive.md). Separate observed sizes from confirmed rules and content sizing from fixed dimensions. Demonstrate agreed behavior with real instances and measured annotations; retain deferred width and mobile-presentation decisions as open findings.

For edge cases, read [edge-cases.md](edge-cases.md). Confirm applicability and expected behavior for the current scenarios. Distinguish local unavailability from no available result, and preliminary empty-state proposals from approved component UI. Preserve unresolved presentation decisions in the bottom findings subsection.
