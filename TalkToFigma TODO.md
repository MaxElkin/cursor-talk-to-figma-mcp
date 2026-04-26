# TalkToFigma TODO

## High-value Figma Plugin API gaps

### Variables and design tokens

- Add tools to read, create, update, delete, and bind variables.
- Add support for variable collections and modes.
- Add support for inspecting and editing variable bindings on nodes.

This is one of the most valuable missing areas for design-system automation.

### Styles authoring

- Add tools to create, update, and delete paint styles.
- Add tools to create, update, and delete text styles.
- Add tools to create, update, and delete effect styles and grid styles.

Current support includes style inspection, but not style management.

### Component property definitions

- Add tools to define and edit component properties directly.
- Support boolean, text, instance-swap, and variant properties.
- Support preferred values, property descriptions, and schema inspection.

Current support can create variants and apply instance overrides, but not manage the component property model itself.

### Variant set management

- Add tools to combine standalone components into a component set.
- Add tools to rename and normalize variant axes and values.
- Add tools to reorder and restructure variant sets.

Current support can create variants, but not perform richer component-set operations.

### Vector and boolean geometry

- Add tools for ellipse, polygon, star, line, and vector nodes.
- Add tools for boolean operations such as union, subtract, intersect, and exclude.
- Add tools for flattening and outlining strokes.
- Add tools for masks and clipping workflows.

Current node creation is limited to rectangles, frames, and text.

### Images and fills

- Add tools to create image fills from raw image data.
- Add tools to edit paint arrays, image transforms, crop, and scale behavior.
- Add tools for richer multi-fill and multi-stroke editing.

Current support is stronger on export than on image-fill authoring.

### Rich text styling

- Add tools for range-level text styling.
- Add tools for mixed text inspection and mutation.
- Add tools for paragraph spacing, list formatting, hyperlinks, and OpenType features.

Current support can create text and replace full contents, but not edit typography deeply.

### Layout and constraints depth

- Add tools for constraints.
- Add tools for rotation and transforms.
- Add tools for clipping and overflow-related properties.
- Add tools for layout grids and advanced sizing rules.

Current auto-layout support is useful, but still partial.

### Effects

- Add tools for shadows, layer blur, background blur, and blend modes.
- Add tools for effect list editing and opacity-related controls.

Current styling support does not cover Figma effects in a meaningful way.

### Page and document structure

- Add tools to create, rename, reorder, and delete pages.
- Add tools to create and manage sections.
- Add tools for broader document organization workflows.

Current support is mainly node-level rather than document-structure-level.

### Prototype authoring

- Add tools to create and edit prototype reactions directly.
- Support navigation actions, overlays, transitions, flows, and starting points.
- Keep `get_reactions` for inspection, but add write-side APIs.

Current support can inspect reactions and draw visual connectors, but not author prototypes.

### Plugin metadata and dev-mode APIs

- Add tools for shared plugin data.
- Add tools for relaunch data.
- Add tools for dev resources and codegen-adjacent metadata.

These would be useful for stronger design-to-code integrations.

### Library workflows

- Add tools to import components from libraries by key.
- Add tools to inspect and manage library-origin components more deeply.
- Add tools to support richer cross-library swap workflows.

Current support includes local component inspection and component instantiation, but library workflows are still thin.

### FigJam-specific APIs

- Add tools for sticky notes, tables, and more first-class FigJam nodes.
- Add deeper support for FigJam interaction and board-specific workflows.

The current surface is clearly optimized for design files rather than FigJam.

## Suggested priorities

1. Variables and variable bindings
2. Style creation and editing
3. Component property/schema editing
4. Variant set normalization and management
5. Vector and boolean operations
6. Prototype authoring
7. Plugin metadata and dev-mode APIs

## Current strengths

TalkToFigma is already solid for:

- design inspection
- basic node creation and editing
- annotations
- text replacement
- auto-layout adjustments
- variant creation
- instance override inspection and application
- icon-resource traversal

The biggest leverage now is expanding from node manipulation into design-system, component-schema, and prototype authoring workflows.
