# CAD → Orthographic → Blender Protocol

1. Define a geometrically valid canonical model (CadQuery / FreeCAD / Rhino / other openable source).
2. Fix datum, direction labels, dimensions and permissible tolerances in mm.
3. Check object body/manifold, intersections, internal wall thickness, minimum radii, unsupported spans and CNC tool access.
4. Generate plan, front, side and sections *programmatically from the model*, never hand-draw independent variants.
5. Export STEP (or exchange CAD), GLB/OBJ meshes and vector projections generated from that exact version.
6. Render in Blender using only exported geometric mesh; realistic stone textures can vary, geometry cannot.
7. Run view-to-view silhouette comparison and annotated dimension checks.
8. List joinery, stone/metal interface, manufacturing fixture and assembly order.
9. Store a versioned revision package: `source/ model/ views/ renders/ QA.md`.

### Mistakes to avoid
- SOGLIA plan depicting a horizontal slot while frontal drawing shows unrelated vertical excavation.
- ARCO side view unrelated to double-arch geometry.
- MASSA side view invented independently of crossed supports.
- SEDUTA changing construction between views.
- Mixing cushion geometry with structural technical drawings on BAMBOO.
- Displaying render dimension labels as if approved CAD.
