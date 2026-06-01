## Platform And Pattern Map

Start with the platform. Apple design is not one universal visual skin. A good
Apple-style result chooses the correct platform archetype before color, radius,
material, or animation work.

## Platform Fit

- iOS: touch-first direct manipulation, safe areas, Dynamic Type, navigation
  stacks, tab bars, sheets, clear feedback, privacy prompts, and one-hand
  reachability where relevant.
- iPadOS: adaptive layouts, multitasking, resizable windows, sidebars, split
  views, drag/drop, keyboard/pointer support, Apple Pencil where relevant, and
  content that survives split view and Stage Manager.
- macOS: menu bar, resizable windows, toolbars, sidebars, inspectors, document
  and window conventions, keyboard shortcuts, pointer precision, denser
  controls, and explicit focus behavior.
- watchOS: glanceable content, short interactions, Digital Crown, complications,
  minimal text, large readable targets, health/safety sensitivity, and quick
  recovery.
- tvOS: focus engine, remote input, large readable layouts, visible focus,
  distance viewing, sparse action density, and media-first hierarchy.
- visionOS: shared spaces and full spaces, windows, volumes, ornaments, depth,
  eye/hand input, indirect gestures, comfort, readable 2D content, careful
  motion, and appropriate immersion level.

## Official Pages To Open As Needed

Open current official Apple Developer pages for the relevant platform and
pattern. Use exact URLs in `official-reference-map.md` first.

Required platform rows:

`platform | official URL | platform traits used | input methods | window/device classes | verification`

Use the canonical platform URLs from `official-reference-map.md`, including
iOS, iPadOS, macOS, watchOS, tvOS, visionOS, and Games when applicable.

Common pattern rows:

`pattern | official URL | why it applies | selected platform variant | rejected alternatives | verification`

If a path has changed, search only `developer.apple.com/design/human-interface-guidelines`
and record the current official URL.

## Pattern Rules

- Navigation must match platform expectations. Do not use iOS tab bars in a
  macOS document app or macOS sidebars in a compact iPhone flow without a clear
  adaptive reason.
- Use modality sparingly. Sheets, popovers, alerts, and full-screen covers need
  clear purpose, dismissal, keyboard/focus behavior, and recovery.
- Settings belong where people expect them for the platform; do not bury
  essential controls inside decorative UI.
- Search should be discoverable, scoped, cancellable, and adaptive.
- Empty, loading, error, permission, offline, and privacy states are part of the
  Apple-quality surface.
- Use platform input conventions: touch, pointer, keyboard, remote, crown,
  Pencil, eye/hand, and voice where applicable.
- Respect platform windowing. macOS, iPadOS Stage Manager/split view, visionOS
  windows, and web responsive layouts all need resize behavior, not one fixed
  screenshot size.
- Privacy and permission moments need clear purpose, user control, recovery,
  and platform-native wording/placement where possible.
- Game, media, maps, charts, live activities, widgets, Apple Pay, Sign in with
  Apple, Wallet, and other technology flows require their exact official HIG or
  technology page before visual or interaction claims.
- Technology flows such as AirPlay, Always On, AR, CarPlay, Game Center,
  generative AI, HealthKit, HomeKit, iCloud, In-App Purchase, Maps, NFC,
  SharePlay, Siri, VoiceOver, Wallet, widgets, Live Activities, and App Clips
  require their exact official page from `official-reference-map.md`.

## Platform Anti-Patterns

- Applying an iPhone-like skin to macOS, iPadOS, tvOS, watchOS, visionOS, or web
  without matching that platform's interaction model.
- Stretching iPhone layouts to iPad instead of using adaptive layouts,
  multitasking, keyboard, pointer, and split-view behavior.
- Shipping macOS tools without menu commands, keyboard shortcuts, resizable
  windows, toolbar/sidebar conventions, or pointer-focused density.
- Building watchOS flows with deep text-heavy screens or no Digital Crown and
  glanceability considerations.
- Designing tvOS with touch/hover assumptions, weak focus states, or text too
  small for distance viewing.
- Creating visionOS layouts with excessive peripheral motion, sudden immersion,
  overlapping controls, poor spatial comfort, or no indirect-gesture path.
- Treating Apple.com marketing pages as app UI source material.
- Creating fake native controls in web UI that do not behave like native or web
  controls.
- Ignoring keyboard, pointer, focus engine, remote, crown, eye/hand, or Pencil
  input when the target platform supports or expects it.
- Hiding essential workflow state inside decorative sheets, cards, or blur.
- Using immersive visionOS treatment when a plain window would be more
  comfortable and task-appropriate.

## Web Translation

For Apple-style web UI:

- Use HIG principles as inspiration, but do not claim native HIG compliance.
- Prefer system font stack and platform-adaptive CSS.
- Avoid unauthorized SF Symbols/font bundling and Apple asset use.
- Recreate behavior only when it improves the product; do not skin a web app as
  fake iOS/macOS if the interaction model remains web-native.
- Use real HTML semantics, browser-native accessibility, responsive layout,
  visible focus, and URL/back-button behavior. Do not degrade web conventions to
  mimic native UI.
- Name the result `Apple-inspired web UI` or `Apple-style web translation`, not
  `HIG-compliant native UI`.
- Final evidence for web work must explicitly say `Apple-style web translation,
  not native HIG compliance`, and must verify no restricted Apple assets,
  bundled Apple fonts, SF Symbols exports, product bezels, first-party screens,
  or Apple marks were used without rights.
