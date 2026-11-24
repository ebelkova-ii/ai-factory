# Passport Filling Rules

Read only for the selected passport block. Use [SKILL.md](../SKILL.md) for grouped questions, concrete package approval and checklist ownership.

All template fields remain present. Fill clear information in the draft without asking redundant questions. Include uncertain values in the requirement questionnaire or present supported proposals for agreement; do not invent them. Independently drafted content still belongs in the concrete approval package before writing.

| Field | Rule |
| --- | --- |
| Name | Use the source component's name, preserving its exact spelling. Distinguish the main component/set identity from an instance override or a variant-combination label; clarify only if the intended identity is ambiguous. |
| Level | Determine independently: `element`, `component`, or `pattern`. Use actual composition and purpose: an elementary UI unit, a reusable component, or a composition implementing a broader interaction scenario. These are classification cues, not a new required layer hierarchy. If ambiguous, propose a classification and obtain agreement. |
| Design status | Ask the user to choose exactly one of `to do`, `in progrees`, or `ready`. Do not infer approval or completion from visual polish. Reuse a confirmed, still-applicable choice from this set. |
| Development status | Ask the user to choose exactly one of `to do`, `in progrees`, or `ready`. Do not infer implementation from the design. Reuse a confirmed, still-applicable choice from this set. Keep the two status answers independent; both questions may appear in one questionnaire. |
| Role | Draft independently when purpose is clear from the component and confirmed context. Ask or propose for agreement when unclear. |
| Usage rules | Draft independently when supported by the component and confirmed context. Ask or propose for agreement when unclear. Distinguish proposed usage guidance from established product requirements. |
| Content rules | Draft independently when supported by the component and confirmed context. Ask or propose for agreement when unclear. Do not invent numeric limits, accepted formats, or validation behavior. |
| Owner | Designer-owned. Preserve the existing value, including an empty or placeholder value. Do not fill, replace, or ask for it as a prerequisite for completing the passport block. |
| Last change | Designer-owned. Preserve the existing value, including an empty or placeholder value. Do not update its date or ask for it as a prerequisite for completing the passport block. |
| Change history / history / История изменений | Designer-owned. Leave the entire history region unchanged, including placeholder entries, dates, authors, avatars, text, and layout. Do not fill it, append entries, clean it up, or ask for history information as a prerequisite for the passport block. |

Owner, Last change, and history are explicit exceptions to placeholder replacement and block-level cleanup. Their unchanged contents must not be reported as an incomplete agent task. In passport validation, verify that all three protected areas were preserved.

## Component documentation link

When Taiga cross-checking is enabled and passport is selected, include a clickable link to the matched component's official Taiga documentation page in Guides, using the existing link area or a compact labeled line. Resolve the real URL; do not guess it or link only the homepage. Versioned code/release citations remain separate evidence and do not substitute for this link. Disclose version limits of unversioned docs. If passport is outside scope, retain the URL in context and obtain scope authorization before editing it.

## Fixed readiness statuses

Both status fields use only these exact user-selected labels: `to do`, `in progrees`, `ready`. Preserve the requested spelling `in progrees`. Provide a separate answer for each field, explicitly offering all three options. The design and development questions may share one questionnaire; never infer one answer from the other.

If an answer or existing value is outside this set (for example, «Нет на проде»), ask the user to select an allowed status instead of inventing a mapping or adding another label. Preserve an outside-set fact as context when relevant; it does not determine readiness by itself. Write the selected labels exactly as listed rather than translating them. These rules govern future status choices; they do not authorize rewriting an existing specification without the applicable change approval.
