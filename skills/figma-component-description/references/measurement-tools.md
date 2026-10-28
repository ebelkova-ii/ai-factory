# Measurement Annotation Tools

Read when placing construction measurements. The supplied Figma template's `Tools for spech` area is the source of editable annotation instances. The names below preserve its original spelling.

| Meaning | Source component family | Choose and edit |
| --- | --- | --- |
| Width and height | `spec-sizelines` | Appropriate horizontal/vertical Direction and Numbers treatment; set the actual measured value. The inspected instances expose a Numbers value text property. |
| Corner radius | `spec-radius` | Appropriate corner Position; set the actual corner radius through the instance's text property. |
| Distance / gap | `spec-magrin` | Appropriate horizontal/vertical Position and text placement; replace the instance's value with the measured distance. |
| Internal padding | `spec-padding` | Appropriate horizontal/vertical Position and text placement; replace the value with the actual padding for that side. |

Resolve the current template's instances and accessible source components at runtime. Inspect supported properties before setting them; internal property IDs and available variants may differ by file. For a value without an exposed text property, use a supported text override without detaching the instance or changing the main annotation component. Do not assume a variant exists without checking.

Reuse an existing annotation instance or create an instance from its accessible source; keep the Tools area unchanged. Orient and size the annotation to the measured span and position it against the correct object/side/corner. Never use a padding marker for a gap or a generic size line instead of the provided radius marker. Do not recreate the annotation appearance manually when the supplied component is available.

Read actual dimensions, paddings, gaps, and corner radii from the relevant source layer. For external distances, use the appropriate common coordinate space and distinguish the gap from container padding. Do not confuse annotation geometry with the measured component's geometry. Values like 72, 8, 16, and 24 in the tool palette are sample values, not defaults.

Keep source annotation instances in Figma: they carry editable properties and geometry that an image cannot replace. A local screenshot may be an optional visual aid, not the source for measurement values or component creation. Do not hardcode current file/node IDs into reusable operations. If tools cannot be found or their source is unavailable, ask how to obtain them before substituting other annotations.
