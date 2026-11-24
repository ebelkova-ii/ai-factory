# Specification Block Map

Read once to resolve scope, target aliases and live checklist routing. Use [SKILL.md](../SKILL.md) for the shared analysis and approval workflow; this map adds no component requirements.

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

The Check-list frame controls routing and records review results; it is not a ninth specification block. Its 11 checks belong to the eight groups above. Checks in the same group share block ownership; they are not separate approval gates.

Any of the eight blocks may end with «Замечания и спорные моменты» when it has substantive findings, improvements, or open questions under the shared [findings rules](findings.md). Do not create an empty subsection or a no-findings message. It is a subsection within each block, not a separate workflow block. Reuse the construction token-attention card treatment; include only findings or material open points and group repeats.

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

Use the selected blocks' detailed references through the routing table in [SKILL.md](../SKILL.md). Source facts, findings and confirmed decisions may serve several selected blocks without authorizing edits to others.
