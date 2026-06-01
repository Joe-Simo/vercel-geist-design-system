## Accessibility And Verification

Apple-quality UI must work with system accessibility settings, input methods,
appearance modes, platform conventions, and real content. The Accessibility HIG
page is mandatory for triggered visual work unless the task cannot affect user
experience.

## Required Checks

For the verified scope, check:

- VoiceOver or accessibility tree: names, roles, values, traits, hints, groups,
  headings, labels, state changes, live updates, and modal boundaries.
- Keyboard/focus: Tab order, focus rings, Escape/Enter/Space, arrow keys,
  shortcuts, focus restoration, and no traps.
- Pointer/touch/remote/crown/spatial input as applicable.
- Dynamic Type/text scaling and localization expansion.
- Light/dark mode, increased contrast, reduced transparency, reduce motion,
  differentiate without color, color filters/grayscale, bold text where
  relevant, and high-contrast browser/system modes.
- Safe areas, window resizing, split view/multitasking, orientation, and device
  classes relevant to the platform.
- Loading, empty, error, permission, offline, privacy, destructive, and recovery
  states.
- Hit targets, spacing, and control reachability using the current Accessibility
  page's platform-specific guidance.
- Content alternatives for images, video, audio, charts, maps, canvas, 3D,
  RealityKit, SceneKit, WebGL, and generated art when they convey information.

## Platform Evidence

When possible:

- Native Apple app: run in simulator/device previews matching target platforms.
- Web app: run in browser on mobile and desktop viewports, with system
  appearance and reduced-motion/reduced-transparency equivalents where possible.
- Capture screenshots for changed states and view sizes.
- Run lint/typecheck/build/tests and accessibility tooling available in the
  project.
- For SwiftUI/UIKit/AppKit, use available previews, simulators, XCTest/UI tests,
  Accessibility Inspector, or platform accessibility APIs when practical.
- For watchOS/tvOS/visionOS, include the target simulator/device class and input
  model in the evidence, not just a desktop screenshot.

## Hard Blockers

- App does not build or primary flow cannot run.
- UI breaks under text scaling, localization, safe areas, split view, or window
  resizing.
- Primary flow cannot be completed with the required input methods.
- Missing accessible names/roles for custom controls.
- Text or symbols are unreadable in dark mode, high contrast, or over materials.
- Required content is hidden in canvas/image/video with no accessible
  equivalent.
- Apple assets, fonts, symbols, or logos are used outside license/rights.
- Work copies Apple first-party screens or implies official Apple affiliation.
- Web UI disables zoom, hides focus, traps keyboard navigation, or breaks native
  browser/system accessibility settings to mimic app behavior.
- visionOS/spatial motion risks discomfort and no reduced-motion or stable
  windowed alternative is provided.

## Interaction Matrix

Use this matrix for every changed flow:

`check | pass/fail/N/A | evidence or blocker`

Cover applicable items:

- VoiceOver/accessibility tree names, roles, values, states, and grouping.
- Keyboard and focus behavior, including shortcut conflicts.
- Touch/pointer/remote/crown/eye-hand/Pencil input as relevant.
- Modal/sheet/alert focus, dismissal, and restoration.
- Dynamic Type/text scaling, localization expansion, and long content.
- Light/dark, increased contrast, reduced transparency, reduce motion,
  differentiate without color, grayscale/color filters, and bold text.
- Safe areas, orientation, window resizing, split view, Stage Manager, external
  displays, or spatial window scaling as relevant.
- Loading, empty, error, permission, privacy, destructive, and recovery states.

## Apple Visual Gate

Before `Apple-quality`, `HIG-aligned candidate`, `official-source-verified`, or
`Apple Taste Gate passed`, record:

`surface | platform | official docs rows | components mapped | appearance modes | Dynamic Type/text scaling | contrast/color settings | reduced transparency | reduced motion | input methods | screenshots/evidence | status`

Native Apple-platform work needs relevant simulator/device/preview evidence. Web
work needs browser viewport evidence and must be labeled as Apple-style web
translation, not native HIG compliance.

## Final Report

Use this concise report for triggered visual work:

```text
Scope:
Platform/surface:
Official Apple docs used:
Components/patterns mapped:
Typography/color/material/icon decisions:
Viewports/devices/states checked:
Accessibility settings checked:
Commands:
Screenshots/evidence:
Revisions made:
Decision: HIG-aligned candidate / Production pass / Fix required
Limitations or whole-app not verified:
```

Do not claim `HIG-aligned candidate`, `Apple-quality`,
`official-source-verified`, `Apple Taste Gate passed`, or `Production pass`
when required docs, screenshots, accessibility checks, or platform states were
not verified. Use `docs consulted; visual/interaction verification blocked` or
`local Apple-style fallback, not official-source-verified` when appropriate.
