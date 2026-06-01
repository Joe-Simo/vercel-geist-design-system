## Apple Interface Craft

Use these craft patterns as Apple-HIG-aligned prompts, not templates. They are
local taste checks that must lead back to official Apple pages before strict
claims.

## Visual Tone

- Content leads. Chrome supports content, navigation, and actions without
  overpowering the task.
- Hierarchy comes from text style, semantic color, spacing, grouping, material,
  and platform structure.
- Apple-style restraint is not emptiness. Use density appropriate to the
  platform and task.
- Prefer calm, legible, high-contrast surfaces over decorative glass, gradient,
  and shadow effects.
- Personality comes from product content, clear affordances, thoughtful motion,
  and platform-appropriate details, not from copying Apple apps or marketing.

## Typography Craft

- Define roles: title, section, body, secondary, caption, label, code/data,
  control text.
- Preserve text hierarchy when Dynamic Type or browser/user text scaling
  changes.
- Avoid all-caps labels unless the platform/component convention supports them.
- Use symbol+text alignment deliberately; match weights and optical scale.
- For macOS tools, allow denser text but keep controls scannable.
- For watchOS/tvOS/visionOS, increase legibility for distance, motion, and
  input constraints.
- Keep titles and labels useful. Do not use oversized display text in compact
  toolbars, lists, menus, settings, alerts, or controls.

## Color Craft

- Prefer semantic tokens: label, secondary label, background, grouped
  background, fill, separator, tint/accent, destructive, success, warning.
- Use tint/accent for action and selection, not broad decoration.
- Keep status colors culturally and contextually clear, and pair them with text
  or symbols.
- Check color in light/dark, increased contrast, grayscale/color filter, and
  over material backgrounds.
- Use tint/accent consistently within a platform context. Do not create
  competing accent systems unless the official platform page and product brand
  require it.

## Material And Liquid Glass Craft

- Use material behind controls/navigation when it helps people retain context.
- Use solid or grouped backgrounds for dense forms, tables, code, or long
  reading surfaces.
- Do not place low-contrast gray symbols/text on translucent backgrounds.
- Avoid overlapping translucent panels unless platform guidance supports that
  hierarchy.
- For web approximations, use subtle blur/transparency only after confirming
  contrast, performance, and reduced-transparency fallback.
- If material makes the interface feel like a demo instead of a product, use a
  clearer grouped or solid surface.

## Motion And Feedback

- Use immediate feedback for taps, clicks, selection, toggles, validation, and
  loading.
- Use continuity motion for navigation only when it clarifies where content went
  or came from.
- Avoid slow springy motion for productivity workflows.
- Respect Reduce Motion with simple fades, cuts, or state changes.
- Symbol animations should communicate status or feedback, not decorate.
- Avoid motion that moves content away from the user's focus, delays recovery,
  or makes visionOS/spatial content physically uncomfortable.

## Composition Craft

- Start with the real workflow or content, not a decorative hero, unless the
  user explicitly requested a marketing surface.
- Use platform-native structure first: navigation stack, split view, sidebar,
  toolbar, tab bar, sheet, alert, list/table, collection, window, ornament, or
  focus area as appropriate.
- Group related controls close to the content they affect.
- Keep primary actions discoverable and secondary actions available without
  turning every surface into a button wall.
- Include loading, empty, error, permission, no-results, offline, and destructive
  recovery states when the surface can enter those states.
- Preserve existing brand language and product-specific information. Apple
  style should refine the product, not erase it.

## Anti-Patterns

- Generic iPhone mockup aesthetic pasted onto every product.
- Rounded rectangles plus blur without platform structure.
- Fake native controls that do not behave like native controls.
- Apple logo, app screenshots, copied Settings rows, or first-party app clones.
- Tiny gray text, insufficient contrast over materials, hover-only actions,
  custom controls without accessibility, and motion that blocks tasks.
- Using SF Symbols as brand marks or using unavailable/private symbols.
- Apple.com hero composition used for an app workflow, settings panel,
  dashboard, table, or dense tool.
- One-off colors, radii, fonts, shadows, or materials that bypass the selected
  platform and project tokens.
- Fake sample data or decorative screenshots used to make the UI look complete
  instead of real data, honest empty states, or user-provided content.
- Web pages that disable zoom, break Back/Forward behavior, trap keyboard focus,
  or hide native browser affordances to imitate an app.

## Failure Handling

- If the design looks like a generic Apple skin, stop and re-map the surface to
  the exact platform page, component pages, and content workflow.
- If the design copies Apple first-party UI, remove the copied composition and
  rebuild from product-specific requirements plus official HIG principles.
- If material/blur lowers contrast or makes hierarchy unclear, switch to a
  solid/grouped surface or a supported platform material with proper fallback.
- If a custom control cannot be verified with keyboard, pointer/touch, screen
  reader, Dynamic Type/text scaling, reduced motion, and platform states, use a
  standard control or report the blocker.
- If the product is web-only, translate Apple principles while keeping web
  semantics and browser behavior intact.
