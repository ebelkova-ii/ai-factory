# Construction Filling Rules

Read only for the construction block. It owns the anatomy/dimensions and token-currency checklist checks. Read [measurement-tools.md](measurement-tools.md) only when resolving or placing measurement annotations. Apply the block approval and per-change revision rules from SKILL.md.

## Preserve the template

Keep the header, Tools for spech palette, `size` and `anatomy` sections, and the supplied layout conventions. Preserve row/column relationships, labels, demonstration cards, styles, and spacing. Adapt repeated rows/cards and frame height to actual coverage without flattening or redesigning the layout. Do not create desktop/mobile categories that do not exist for the component; clarify uncertain category mappings.

All sample components, part names, counts, descriptions, measurements, and token values in the editable specification area are placeholders. Replace them with the selected component's data. The Tools palette itself is a reusable reference, not a sample component to replace or a part to document.

## Size and dimensions

- Include every existing size of the selected component; do not reduce coverage to representative sizes. Identify actual sizes from component definitions and confirmed context, not copied template labels. Treat a size label separately from a count of all variant combinations; ask if that distinction is unclear.
- Use real instances/demonstrations for each size and the annotation components from Tools for spech. Cover actual width, height, relevant gaps, paddings, and corner radii using the matching tools.
- Read values from the actual component/layer represented in the demonstration. Describe flexible dimensions and their sizing behavior rather than presenting one rendered measurement as a universal fixed size. Clarify behavior unavailable from the design.
- For a composite component, extract its nested component parts into demonstration areas too and annotate their dimensions. Preserve the relationship to the parent, instance overrides, and applicable parent-size context. Do not detach or alter source components just to obtain demonstrations. Ask if a source or required information is inaccessible.
- Retain existing layout relationships when adding enough examples for complete size coverage. Keep annotation labels readable and anchored to the measured part.

## Anatomy and bindings

- Check every actual layer and element for color, typography/font, and size/spacing bindings, including nested and hidden/conditional parts. Track scan coverage internally; read large hierarchies in bounded batches without discarding layers. Full scan coverage does not require a full layer catalogue on the canvas.
- Replace example part inventories with only the layers/properties that require attention, placed in the block's bottom «Замечания и спорные моменты» subsection under [findings.md](findings.md). Do not duplicate them in anatomy or list correctly bound layers, their token inventories, or a complete source-layer registry. The size/dimension demonstrations above remain required and are unaffected by this filtering.
- Each finding identifies the affected part/path, property, actual value, and concise attention note. Show a relevant part demonstration when useful. Group repeated instances with the same issue, values, and context into one entry, with a count and a locatable description; preserve exact affected IDs in local task evidence rather than printing hundreds of IDs on the canvas. Do not combine different values or issues under an ambiguous entry.
- Collect bindings per layer internally and publish only evidence relevant to findings. Preserve exact token/style names when needed to explain a problem. Distinguish a Figma style from a variable binding; do not label arbitrary literal values as tokens. If no substantive findings remain, do not create a bottom subsection, a no-findings message, or normal-layer cards. Report the verified scope and any unperformed checks honestly under the shared findings rules.
- Resolve available aliases and relevant modes without inventing a token source. For mixed text styling, inspect relevant text runs rather than assigning one font/style to the entire layer. Reuse shared token metadata across layers while retaining each layer's binding relationship.
- Binding presence does not establish token currency. Verify currency against the accessible agreed source of truth; ask when the source is unknown or unavailable. Absence of a binding does not by itself authorize changing the component. Follow the separate problem/fix approval rule when an actual problem is identified.
- For a color property with no token binding, show its actual HEX code and the Russian note «Требует внимания: цвет без токена». Attribute it to the correct layer/property; preserve opacity separately when relevant instead of losing it in the displayed value. Do not substitute a guessed nearest token. Record this as an attention item and follow the component-problem approval rule before any attempted fix.
- For typography/font and size properties without a token binding, show the actual value with its units where applicable and the Russian note «Требует внимания: нет привязки к токену». Identify the affected property precisely; retain any actual Figma style name separately rather than implying no style exists. Do not invent a token or replace the value automatically. Any proposed fix requires the separate approval for changing the source component.

## Block checks

Before requesting content approval, account for every existing size and nested component requiring dimension demonstrations. Verify that all layers were scanned internally but that anatomy publishes only attention findings, with repeated identical findings grouped. Verify annotation tool semantics and measurement values, no copied sample facts, accurate binding attribution, and preservation of the template's layouts and Tools palette. Do not assess coverage by the number of layers printed on the canvas.

After approved edits, inspect the changed construction frame for clipping, overlap, broken instances, incorrect measurements, and missing coverage. Update only this block's checklist items under the applicable approval policy. Ask before moving to variants or the next selected block.

The user-confirmed unbound-value convention applies to colors, typography/fonts, and sizes. An attention note records the missing binding; it is not permission to repair the source or proof that a specific token must be used.
