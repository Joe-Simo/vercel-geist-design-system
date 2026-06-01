## Foundation And Style Rules

Apple-aligned design starts with current HIG principles, platform fit, clarity,
deference to content, direct manipulation, feedback, consistency, privacy, and
accessibility. Use this file as a gate, not as a substitute for official pages.

For every foundation used, open the matching official Apple page from
`official-reference-map.md` and capture Docs Evidence before strict claims.

## Typography

- Prefer platform/system typography through native APIs or CSS system stacks.
- Use Dynamic Type or platform text styles where supported. Preserve hierarchy,
  line wrapping, control fit, and information scent when text size changes.
- Use the official Typography and Accessibility pages for platform default and
  minimum size decisions; do not invent numeric type scales from memory.
- Keep text legible: avoid tiny sizes, thin body weights, excessive typefaces,
  negative tracking, cramped line height, and truncation that hides meaning.
- Use SF Symbols alongside text only when they clarify an action or concept;
  match symbol weight, scale, and baseline to adjacent text per the current SF
  Symbols guidance.
- Use custom fonts only when they improve brand expression without weakening
  legibility, localization, Dynamic Type, or platform feel.
- For web, use `-apple-system, BlinkMacSystemFont, system-ui, sans-serif` as
  the safe system stack. Do not name or bundle Apple font files in CSS unless
  the project has verified rights for the exact target use.
- For code, tables, terminal-like content, or technical identifiers, use the
  project's established monospace or platform-appropriate system mono; do not
  imply Apple font licensing if the font is not actually licensed or bundled.

## Color

- Use semantic system colors when building native Apple-platform UI.
- Support light and dark appearances, increased contrast, reduced transparency,
  color filters, and platform accent behavior.
- Use color consistently. Do not use the same color for conflicting meanings.
- Never rely on color alone for status, selection, validation, or interactivity.
- Custom brand color must still pass contrast, vibrancy/material, selection,
  disabled, pressed, and high-contrast states.
- Prefer wide color only when the asset pipeline and display target support it;
  provide stable fallbacks.
- On web, map Apple-style color roles to project tokens such as label,
  secondary label, background, grouped background, fill, separator, tint,
  destructive, success, and warning. Do not hard-code a fake iOS palette.

## Layout And Adaptivity

- Design for device class, window size, orientation, split view, keyboard,
  pointer, touch, remote, crown, spatial input, and safe areas as applicable.
- Use platform-native layout behavior where possible: safe areas, Auto Layout,
  SwiftUI layout, size classes, resizable windows, toolbars, sidebars, tab bars,
  sheets, and split views.
- Keep content readable and controls reachable at all supported sizes.
- Avoid fixed pixel layouts that break on Dynamic Type, localization, Stage
  Manager, split view, external displays, or visionOS window scaling.
- Use whitespace, alignment, grouping, and hierarchy before decorative borders.
- Use the Accessibility page for platform-specific target-size guidance. Do not
  ship tiny custom controls just because they look refined in a screenshot.
- For dense macOS tools, density can increase, but keyboard focus, pointer
  affordance, readable labels, and resize behavior still have to hold.

## Materials And Depth

- Use materials to clarify hierarchy between foreground and background, not as
  decoration.
- Liquid Glass and standard materials must respond to system settings such as
  reduced transparency and increased contrast.
- For Liquid Glass claims, open Materials plus Apple's current Liquid Glass and
  Adopting Liquid Glass technology overview pages. Prefer standard
  SwiftUI/UIKit/AppKit controls when they already adopt platform materials.
- Keep text and symbols legible over materials. Use semantic vibrant colors
  rather than hard-coded low-contrast values.
- Avoid stacking many translucent panels. Too much blur/glass weakens focus,
  contrast, performance, and platform taste.
- For non-native web UI, approximate depth carefully with CSS only when it helps
  hierarchy; do not claim native Liquid Glass behavior.
- Use solid/grouped backgrounds for dense forms, tables, code, long reading,
  and error/permission flows when material hurts legibility.

## Icons, Symbols, And App Icons

- Prefer SF Symbols for Apple-platform interface symbols when license and
  platform allow.
- Check symbol availability for the OS versions the product supports.
- Do not customize Apple product/feature symbols when official guidance forbids
  customization.
- Choose variants for meaning: outline for many toolbar/list contexts, fill for
  selection/emphasis where appropriate, slash for unavailable/disabled concepts,
  and enclosed forms for small-size legibility.
- Do not use symbols as decorative wallpaper or brand marks.
- Do not use SF Symbols, or confusingly similar symbols, as app icons, logos, or
  trademarked marks.
- App icons should be simple, recognizable, platform-appropriate, and not rely
  on transparency, screenshots, text-heavy artwork, or Apple logos.
- Verify current official icon/app-icon production guidance before final icon
  claims.
- Use the official Apple Design Resources and current app icon templates only
  within their license.
- For supported platforms, check Icon Composer/layered icon guidance and verify
  appearance variants, size reduction, dark/tinted contexts, and backgrounds.

## Motion

- Motion should explain causality, continuity, hierarchy, and feedback.
- Respect Reduce Motion and avoid required large parallax, spin, zoom, or
  spatial motion.
- Keep animations interruptible and state-driven. Avoid ornamental motion that
  delays tasks.
- On visionOS, use depth and motion with restraint; readable content should stay
  mostly flat and stable.
- Use official Motion and SF Symbols/Symbols framework guidance for symbol
  effects. Do not invent universal timing/easing values as HIG rules.
- If animation is decorative or makes the task slower, remove it or limit it to
  an optional enhancement with reduced-motion behavior.

## Writing And Content

- Use the official Writing guidance for labels, empty states, alerts,
  permission explanations, errors, onboarding, and settings copy.
- Write direct, human labels that describe the user's action or the system
  state. Avoid generic marketing copy inside task surfaces.
- Do not use Apple product names, platform names, or technology names as visual
  decoration. Use them only when they truthfully identify compatibility,
  platform behavior, or an enabled technology.
- Preserve domain terminology and existing product language unless it conflicts
  with clarity, accessibility, privacy, or official platform conventions.

## Foundation Gate

Before screen work, record:

`foundation | official Apple URL | section/page | platform impact | implementation target | verification`

The gate must cover, when applicable:

- Platform/system typography and text scaling.
- Semantic color, light/dark, contrast, and color-blind-safe cues.
- Layout/adaptivity: safe areas, windows, orientation, split view, dynamic text,
  localization, device classes, and input methods.
- Materials/Liquid Glass and reduced-transparency fallback.
- SF Symbols/iconography and app-icon needs.
- Motion/reduced-motion behavior.
- Writing/content clarity.
- Accessibility and privacy-sensitive states.

If a foundation is not relevant, say why. If it is relevant and not source
checked, do not claim HIG alignment for that surface.
