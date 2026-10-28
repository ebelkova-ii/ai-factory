# Passport Filling Rules

Read only when creating or revising the passport block. Use the block map for checklist ownership and SKILL.md for approvals.

All template fields remain present. Fill clear information in the draft without asking redundant questions. When a value is uncertain, ask one question or present a concrete proposal for agreement; do not silently invent it. Preparing a value independently does not bypass block approval before writing to Figma or per-change approval in revision mode.

| Field | Rule |
| --- | --- |
| Name | Use the source component's name, preserving its exact spelling. Distinguish the main component/set identity from an instance override or a variant-combination label; clarify only if the intended identity is ambiguous. |
| Level | Determine independently: `element`, `component`, or `pattern`. Use actual composition and purpose: an elementary UI unit, a reusable component, or a composition implementing a broader interaction scenario. These are classification cues, not a new required layer hierarchy. If ambiguous, propose a classification and obtain agreement. |
| Design status | Ask the user to choose exactly one of `to do`, `in progrees`, or `ready`. Do not infer approval or completion from visual polish. Reuse a confirmed, still-applicable choice from this set. |
| Development status | Ask the user to choose exactly one of `to do`, `in progrees`, or `ready`. Do not infer implementation from the design. Reuse a confirmed, still-applicable choice from this set. Ask about the two statuses separately under the one-question rule. |
| Role | Draft independently when purpose is clear from the component and confirmed context. Ask or propose for agreement when unclear. |
| Usage rules | Draft independently when supported by the component and confirmed context. Ask or propose for agreement when unclear. Distinguish proposed usage guidance from established product requirements. |
| Content rules | Draft independently when supported by the component and confirmed context. Ask or propose for agreement when unclear. Do not invent numeric limits, accepted formats, or validation behavior. |
| Owner | Designer-owned. Preserve the existing value, including an empty or placeholder value. Do not fill, replace, or ask for it as a prerequisite for completing the passport block. |
| Last change | Designer-owned. Preserve the existing value, including an empty or placeholder value. Do not update its date or ask for it as a prerequisite for completing the passport block. |
| Change history / history / История изменений | Designer-owned. Leave the entire history region unchanged, including placeholder entries, dates, authors, avatars, text, and layout. Do not fill it, append entries, clean it up, or ask for history information as a prerequisite for the passport block. |

Owner, Last change, and history are explicit exceptions to placeholder replacement and block-level cleanup. Their unchanged contents must not be reported as an incomplete agent task. In passport validation, verify that all three protected areas were preserved.

## Fixed readiness statuses

Both status fields use only these exact user-selected labels: `to do`, `in progrees`, `ready`. Preserve the requested spelling `in progrees`. Ask one question per field, explicitly offering all three options, for example: «Какой статус дизайна выбрать: to do, in progrees или ready?» Then ask separately about development.

If an answer or existing value is outside this set (for example, «Нет на проде»), ask the user to select an allowed status instead of inventing a mapping or adding another label. Preserve an outside-set fact as context when relevant; it does not determine readiness by itself. Write the selected labels exactly as listed rather than translating them. These rules govern future status choices; they do not authorize rewriting an existing specification without the applicable change approval.
