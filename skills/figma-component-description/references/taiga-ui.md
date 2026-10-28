# Optional Taiga UI Cross-Check

Read only when the user enables Taiga UI cross-checking. This reference supplements the existing block workflow; it does not replace any scope, question, approval, source-protection, demonstration, or checklist rule in SKILL.md. Write user-facing questions and specification content in Russian.

## Establish the source once per task

Use the library and cross-check choice already supplied by the user. Otherwise ask about the library first, then ask separately whether to cross-check against Taiga UI. Ask exactly one question at a time and wait. A direct request for a Taiga cross-check already enables it. If declined, continue the original workflow without fetching Taiga documentation or making access to it a prerequisite.

When enabled, always use the latest stable Taiga UI release at task start. Do not ask for the company's installed version and do not hardcode a version number. Determine the stable release from the official package registry entry for `@taiga-ui/core` (the `latest` dist-tag, verifying it is not a prerelease) or the official repository's stable releases. Distinguish the library release from the MCP package version. Record the resolved version, verification date, and exact source URL in task context. Keep that baseline across blocks; do not silently switch versions mid-task. Resolve conflicting release evidence before claiming a latest-version cross-check.

Check that the documentation used covers this release. A page footer, an unversioned URL, or a server configured with `latest` is not sufficient by itself. Check the documentation/source metadata against the resolved release; consult the official repository at the corresponding release tag when needed. If the match cannot be established, explain the limitation and ask one question about how to proceed before relying on version-sensitive facts. Do not present stale or unverified documentation as verified latest-version evidence.

## Access and component matching

Use available connected Taiga MCP tools when present, after checking their actual schemas and documentation source. The official server documents `get_overview`, `get_list_components`, and `get_component_example`: read its overview first, search section IDs, then request the relevant component documentation. Do not assume the server is installed or that tool names/schemas remain unchanged. Never run setup or change client configuration automatically.

Without that MCP, use the official index and targeted documentation pages through available web tools:

- [Documentation index](https://taiga-ui.dev/llms.txt)
- [Component documentation](https://taiga-ui.dev/)
- [Official repository and releases](https://github.com/taiga-family/taiga-ui)
- [Official MCP instructions](https://taiga-ui.dev/ai/mcp/)
- [Markdown documentation format](https://taiga-ui.dev/ai/llms/)

Discover exact component URLs through the index or navigation. Markdown pages are optional; if the reader rejects `text/markdown`, use the HTML page. Follow relevant API, example, nested-component, or same-release source links as necessary. Do not load the entire `llms-full.txt` or unrelated components by default. If no supported reader can access an essential source, explain what failed and ask one question about the required next step; do not claim the cross-check succeeded.

Match by purpose, composition, properties, and behavior, not only the Figma name. For example, `date-picker` might correspond to `Calendar`, `InputDate`, or a composition. If several candidates fit, ask the user to confirm the mapping before applying their facts. Identify the direct counterpart and relevant documented usage contexts or compositions. For example, Calendar can also be used inside InputDate; a matching standalone Calendar is not a reason to ignore that integration. For a composition, identify each relevant part and its source. Distinguish the component, host field, and display container and their responsibilities. A usage context is not automatically another Figma variant axis. Follow only relevant links for the current block, without expanding editing scope. If no counterpart is found, explain this and agree the next source or approach instead of choosing a vaguely similar component. Do not edit the source or expand block scope to make the mapping fit.

## Use evidence within the current block

Fetch only what the current selected block needs and reuse confirmed sources across blocks. Evaluate each subject below when relevant; this table does not make every example or API capability a mandatory requirement.

| Block | Relevant Taiga evidence | Preserve the existing boundary |
| --- | --- | --- |
| Passport | Purpose, usage conditions, content formats and constraints | Use the Figma identity and existing Level rules. Ask separately for readiness statuses. Leave Owner, Last change, and history untouched. |
| Construction | Composition, nested parts, supported size options and relevant API | Measure Figma and inspect its actual bindings. Taiga defaults do not establish corporate token currency or authorize replacing geometry/styles. |
| Variants | Supported options, their purpose, and combination constraints | Show all existing Figma variant combinations under the existing rules. Do not generate absent variants or assume every API input is a Figma axis. |
| States | State triggers, behavior, ownership by nested parts, and interaction constraints | Use real states and agreed examples. Library documentation does not prove corporate runtime behavior or permit fabricating a missing state. |
| Responsive | Documented sizing, overflow, supported contexts, and mobile approaches | Do not turn an example width, a global breakpoint, or one optional mobile approach into a component requirement. |
| Edge cases | Documented value limits, validation, empty/long content, and recovery constraints | Confirm applicability and unknown expected behavior. Example application settings are not universal rules. |
| Accessibility | Component semantics, keyboard rules, labels, and component-specific guidance | Retain accessibility.md, primary WCAG/WAI-ARIA sources, explanations of user impact, and tradeoffs. Do not certify accessibility from documentation or Figma. |
| Animation | Documented triggers, transitions, timing/easing, interruptions, and reduced motion | Distinguish defaults from demo settings. Missing documentation does not mean no animation; clarify essential unknowns. |

Keep three evidence types explicit: observed Figma facts, documented Taiga UI behavior/capabilities, and confirmed corporate requirements or overrides. Company teams change visual styling; this does not prove that every behavioral default is inherited. Use documented Taiga facts as attributed reference material in the block draft. Before describing them as the corporate component's established behavior, confirm applicability from supplied context or ask one question about a material unknown. Reuse already confirmed applicability rather than asking again for each fact. Carry confirmed corporate differences across subsequent blocks; do not replace them with library defaults. Compare new evidence with relevant recorded decisions and previously read content before proposing a requirement. Use SKILL.md for cross-block conflicts and declined changes, and findings.md for explicit deferrals.

For each source used, retain its exact URL, relevant section, release baseline, and verification date. Show attribution in the Codex draft; include compact source links in the agreed content of the current Figma block. Do not add a ninth block, alter protected history, or write sources to other frames without authorization. Sources are not findings by themselves: keep ordinary attribution outside the findings subsection.

A visual difference alone is not a defect. Explain meaningful behavior conflicts as differences to clarify before calling them defects. Do not automatically migrate a corporate component to the newest Taiga behavior or overwrite corporate design choices. Confirmed requirements govern the specification; where a proposed requirement conflicts with library capability, surface the limitation instead of implying it is already implemented. Record material unresolved differences in the current block's «Замечания и спорные моменты» under findings.md, without bypassing questions about essential information.

## Keep the existing approval cycle

Taiga evidence enriches the current block's draft; it does not approve that draft, authorize any source-component fix, authorize updating completed documentation, or approve advancing to the next block. Continue the existing one-question rule, create/revise approval rules, real-instance demonstrations, protected fields, and checklist ownership. Preserve unselected blocks and all unrelated content.

Do not mark a check passed merely because Taiga documents the capability. Verify what can actually be checked in Figma, distinguish reference guidance from tested implementation results, and report unavailable checks honestly. An unavailable source, unmatched component, or essential unknown must not be hidden behind a completion claim.

## Investigate animation before requesting missing parameters

For the current release, trace component and container styles through shared keyframes, global styles, design tokens, and any applicable overrides or reduced-motion mechanisms. Do not stop at a symbolic duration or claim there is no animation because one component stylesheet has no declaration. Separate container entrance/exit from internal cell hover/selection.

Extract supported facts: triggers, affected properties, start/end values, duration and delay, easing, direction, interruption/cancellation, and reduced-motion behavior. Cite the exact source and token provenance. Check the resolved dependency version through a lockfile or built artifact when available: a dependency range does not prove which patch version supplied the value. Otherwise name the specific inspected dependency version and state the remaining uncertainty. Do not embed a trial component's numeric defaults as universal requirements.

Distinguish source-code defaults, example overrides, browser computed styles, and measured motion. Browser inspection can verify actual applied parameters when available; do not claim it happened when only source was read. System-preference detection alone does not prove which motion is disabled. Investigate its consumers before describing the exact reduced-motion effect.

First use accessible evidence for extractable library facts. Then ask one question about product choices or genuinely unavailable parameters. Label library values as reference values until corporate applicability is confirmed. Recording an unresolved motion decision follows findings.md and never establishes tested animation.
