# Optional Taiga UI Cross-Check

Read once when Taiga UI cross-checking is enabled. Use the shared dataset and package workflow in [SKILL.md](../SKILL.md); this reference governs evidence, not editing permissions. Write questions and specification content in Russian.

## Establish the source once per task

Use the library and cross-check choice already supplied by the user. Otherwise include separate library and cross-check decisions in the onboarding questionnaire; wait for each needed answer before dependent research. A direct request for a Taiga cross-check already enables it. If declined, proceed without fetching or depending on Taiga documentation.

When enabled, always use the latest stable Taiga UI release at task start. Do not ask for the company's installed version and do not hardcode a version number. Determine the stable release from the official package registry entry for `@taiga-ui/core` (the `latest` dist-tag, verifying it is not a prerelease) or the official repository's stable releases. Distinguish the library release from the MCP package version. Record the resolved version, verification date, and exact source URL in task context. Keep that baseline across blocks; do not silently switch versions mid-task. Resolve conflicting release evidence before claiming a latest-version cross-check.

Check that the documentation used covers this release. A page footer, an unversioned URL, or a server configured with `latest` is not sufficient by itself. Check the documentation/source metadata against the resolved release; consult the official repository at the corresponding release tag when needed. If the match cannot be established, disclose it and request the focused next-step decision before relying on version-sensitive facts. Do not present stale or unverified documentation as verified latest-version evidence.

## Access and component matching

Use available connected Taiga MCP tools when present, after checking their actual schemas and documentation source. The official server documents `get_overview`, `get_list_components`, and `get_component_example`: read its overview first, search section IDs, then request the relevant component documentation. Do not assume the server is installed or that tool names/schemas remain unchanged. Never run setup or change client configuration automatically.

Without that MCP, use the official index/pages for discovery. Prefer an available GitHub connector for exact-tag/commit source files when it supplies the needed capability; otherwise use supported official web sources. Keep the same release baseline across fallbacks and avoid repeated cache/404/network attempts without new evidence. Do not make a connector or installation mandatory. Official entry points:

- [Documentation index](https://taiga-ui.dev/llms.txt)
- [Component documentation](https://taiga-ui.dev/)
- [Official repository and releases](https://github.com/taiga-family/taiga-ui)
- [Official MCP instructions](https://taiga-ui.dev/ai/mcp/)
- [Markdown documentation format](https://taiga-ui.dev/ai/llms/)

Discover exact component URLs through the index or navigation. Markdown pages are optional; if the reader rejects `text/markdown`, use the HTML page. Follow relevant API, example, nested-component, or same-release source links as necessary. Do not load the entire `llms-full.txt` or unrelated components by default. If an essential source is inaccessible, report the failure and request the dependent decision; do not claim success or repeat failed access without new evidence.

Match by purpose, composition, properties, and behavior, not only the Figma name. For example, `date-picker` might correspond to `Calendar`, `InputDate`, or a composition. If several candidates fit, ask the user to confirm the mapping before applying their facts. Identify the direct counterpart and relevant documented usage contexts or compositions. For example, Calendar can also be used inside InputDate; a matching standalone Calendar is not a reason to ignore that integration. For a composition, identify each relevant part and its source. Distinguish the component, host field, and display container and their responsibilities. A usage context is not automatically another Figma variant axis. Follow relevant links for the selected block scope and reuse shared evidence without expanding editing scope. If no counterpart is found, explain this and agree the next source or approach instead of choosing a vaguely similar component. Do not edit the source or expand block scope to make the mapping fit.

## Share evidence across selected blocks

Collect only the evidence the selected blocks need, in bounded requests, and reuse confirmed sources instead of fetching them again per block. Evaluate each subject below when relevant; this table does not make every example or API capability a mandatory requirement.

| Block | Relevant Taiga evidence | Preserve the existing boundary |
| --- | --- | --- |
| Passport | Purpose, usage conditions, content formats and constraints | Use the Figma identity and Level rules, independent readiness answers and protected fields. Include the official component-page link in Guides under [passport.md](passport.md); code citations are separate. |
| Construction | Composition, nested parts, supported size options and relevant API | Measure Figma and inspect its actual bindings. Taiga defaults do not establish corporate token currency or authorize replacing geometry/styles. |
| Variants | Supported options, their purpose, and combination constraints | Show all existing Figma variant combinations under the existing rules. Do not generate absent variants or assume every API input is a Figma axis. |
| States | State triggers, behavior, ownership by nested parts, and interaction constraints | Use real states and agreed examples. Library documentation does not prove corporate runtime behavior or permit fabricating a missing state. |
| Responsive | Documented sizing, overflow, supported contexts, and mobile approaches | Do not turn an example width, a global breakpoint, or one optional mobile approach into a component requirement. |
| Edge cases | Documented value limits, validation, empty/long content, and recovery constraints | Confirm applicability and unknown expected behavior. Example application settings are not universal rules. |
| Accessibility | Component semantics, keyboard rules, labels, and component-specific guidance | Retain accessibility.md, primary WCAG/WAI-ARIA sources, explanations of user impact, and tradeoffs. Do not certify accessibility from documentation or Figma. |
| Animation | Documented triggers, transitions, timing/easing, interruptions, and reduced motion | Distinguish defaults from demo settings. Missing documentation does not mean no animation; clarify essential unknowns. |

Separate Figma observations, attributed Taiga facts and confirmed corporate requirements/overrides. Visual customization proves no behavioral inheritance. Confirm material corporate applicability from context or the thematic questions before presenting library behavior as established. Reuse confirmed applicability and corporate departures across blocks instead of reverting to defaults. Check new evidence against recorded decisions and relevant earlier content; use SKILL.md for conflicts/refusals and findings.md for deferrals.

For each source used, retain its exact URL, relevant section, release baseline, and verification date. Show attribution in the Codex draft; include compact source links in the agreed content of the current Figma block. Do not add a ninth block, alter protected history or write sources outside the approved target scope. Sources are not findings by themselves: keep ordinary attribution outside the findings subsection.

A visual difference alone is not a defect. Explain meaningful behavior conflicts as differences to clarify before calling them defects. Do not automatically migrate a corporate component to the newest Taiga behavior or overwrite corporate design choices. Confirmed requirements govern the specification; where a proposed requirement conflicts with library capability, surface the limitation instead of implying it is already implemented. Record material unresolved differences in affected selected blocks under findings.md; essential questions remain dependencies.

## Evidence is not approval

Taiga evidence is reference material, not permission to change documentation or sources. Use the concrete package under [SKILL.md](../SKILL.md), preserving selected scope, real demonstrations, protected fields and checklist ownership.

Do not mark a check passed merely because Taiga documents the capability. Verify what can actually be checked in Figma, distinguish reference guidance from tested implementation results, and report unavailable checks honestly. An unavailable source, unmatched component, or essential unknown must not be hidden behind a completion claim.

## Investigate animation before requesting missing parameters

For the current release, trace component and container styles through shared keyframes, global styles, design tokens, and any applicable overrides or reduced-motion mechanisms. Do not stop at a symbolic duration or claim there is no animation because one component stylesheet has no declaration. Separate container entrance/exit from internal cell hover/selection.

Extract supported facts: triggers, affected properties, start/end values, duration and delay, easing, direction, interruption/cancellation, and reduced-motion behavior. Cite the exact source and token provenance. Check the resolved dependency version through a lockfile or built artifact when available: a dependency range does not prove which patch version supplied the value. Otherwise name the specific inspected dependency version and state the remaining uncertainty. Do not embed a trial component's numeric defaults as universal requirements.

Distinguish source-code defaults, example overrides, browser computed styles, and measured motion. Browser inspection can verify actual applied parameters when available; do not claim it happened when only source was read. System-preference detection alone does not prove which motion is disabled. Investigate its consumers before describing the exact reduced-motion effect.

First use accessible evidence for extractable library facts. Then group product choices or genuinely unavailable parameters into the relevant thematic questions. Label library values as reference values until corporate applicability is confirmed. Recording an unresolved motion decision follows findings.md and never establishes tested animation.
