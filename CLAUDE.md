# Claude Code instructions — TINELLA

Read `README.md`, `PROJECT_CONTEXT.md`, `AGENTS.md`, and `design/OBJECT_REGISTRY.md` before implementing any object.

Project goals: stone CNC product design, accurate CAD-first manufacturing, market research and business feasibility.

**Non-negotiable**:
- Never infer fabrication geometry from an AI-generated rendering. Earlier sheets contain mutually inconsistent flat views.
- Model a single solid/assembly first; derive all orthographic outputs and Blender assets from that same model.
- Explicitly mark design assumptions and distinguish verified facts from visual hypotheses.
- Use mm, named parts, material specifications, tolerance ledger and a revision identifier.
- ARCO = two arches at 45° seen in top section; verify geometric interpretation in true 3D.
- BAMBOO = marble cylindrical members and same-stone cylindrical feet; no rope, no casters. Removable C&C Milano MAREMMA cushions appear only in visual renders; reserve a clear volume in engineering views.
- Confirm the fabric article/code/colorway before asserting an exact surface texture.
- Never market gres/porcelain/ceramic as quarried stone. Label mixed-material products.
- When researching sales, use public evidence and confidence grades; do not imply verified unit sales without a primary source.
- Do not store third-party copyrighted catalogue photos or private manufacturer quotations in the public repository without permission.

When creating a geometry change, create a technical description, dimensions, editable source, outputs and changelog in the same PR. Propose test coupons and structural reviews for long-span pieces.

Suggested cycle: research → technical sketch → parametric CAD → projected views → interference and mass check → Blender render → shop review → sample prototype → costing → iteration.

Do not replace historical iterations; move invalidated ones under `archive/superseded` when they become available.
