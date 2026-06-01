## Component System

Map UI requirements to official Apple HIG components, platform-native APIs, or
constrained custom compositions before inventing custom controls. Component
styling is not enough; behavior, states, input, accessibility, and platform fit
must match the selected official pattern.

## Component Mapping

For each changed component, record:

`surface | requirement | official Apple page/API | platform variant | states | accessibility | verification`

Common components/patterns to verify against current Apple HIG pages:

- Actions and commands: Buttons, menus, menus/actions, context menus, toolbars,
  keyboard shortcuts, gestures, drag/drop, game controllers.
- Navigation and structure: Navigation bars, tab bars, sidebars, toolbars,
  split views/windows, lists/tables, collections, search.
- Forms and selection: Text fields, search fields, pickers, sliders, toggles,
  steppers, segmented controls, entering data, selection/input.
- Modality and feedback: Alerts, sheets, popovers/panels where supported,
  modality, feedback, loading, empty/error/recovery states, status, progress
  indicators, gauges, rating indicators, ratings/reviews, and activity rings.
- Content/data/technologies: Charts, maps, media controls, widgets, Live
  Activities, App Clips, Apple Pay, Sign in with Apple, complications, images,
  image views, App Shortcuts, Live Photos, and notifications.
- Iconography/assets: App icons, document icons where relevant, custom icons,
  SF Symbols, Apple Design Resources.

Open the exact current official page for each selected component or pattern
before designing/coding. If a page moved, search only Apple Developer domains
and cite the resolved official URL.

## HIG Index Reconciliation

Before broad component work, certification-style review, or all-in-one Apple
design-system claims, open the current HIG Components, Inputs, Patterns, and
Technologies indexes from `official-reference-map.md`. Compare the live Apple
navigation against this local map. If an official page needed by the task is
missing locally, use the live official URL, map it to the closest bucket, and
report the skill drift in the final response. Do not block the user's work just
because the local map is missing a live Apple page.

## State Requirements

Every interactive component needs relevant states:

- default, hover/pointer, pressed, focused, selected/current, disabled,
  loading, error, destructive, expanded/collapsed, checked/unchecked, mixed,
  high contrast, dark mode, reduced transparency, reduced motion.

Native platforms often provide state behavior automatically. Preserve it unless
there is a concrete reason to customize.

## Component Documentation Contract

For every component that maps to an Apple HIG page or native API, record:

- Exact official page/section consulted.
- Platform variant selected and variants rejected.
- The specific behavior/content/accessibility rule that affected the design.
- A short source-specific evidence point for the final Docs Evidence table.
- States implemented or preserved.
- Screenshot, simulator, browser, or accessibility verification.

Generic visual matching, CSS class names, memory of native controls, or a
third-party UIKit/Cupertino component name is insufficient when the official
page gives a more specific rule.

## Custom Controls

Custom controls are allowed only when a standard component cannot express the
task. They must:

- Match platform input expectations.
- Expose name, role, value, state, hint, keyboard/focus behavior, and pointer or
  touch behavior.
- Support Dynamic Type, localization, contrast, high contrast, reduced motion,
  and reduced transparency.
- Include error/recovery behavior and clear affordance.
- Be verified against the closest official Apple component or pattern.

If a custom control cannot meet the closest native component's input and
accessibility expectations, do not ship it as Apple-quality. Use a standard
control, simplify the interaction, or state the blocker.

## Native vs Web Implementation

- SwiftUI/UIKit/AppKit: prefer system components, semantic colors, text styles,
  materials, SF Symbols, and native accessibility APIs.
- Native custom drawing/canvas/SceneKit/RealityKit/WebGL: provide accessible
  equivalents, reduced-motion behavior, and standard controls for critical
  actions.
- React/web: use accessible primitives and CSS system stacks; translate Apple
  patterns without using restricted assets or fake-native behavior.
- Do not copy exact Apple first-party app screens. Build product-specific
  compositions that follow HIG principles.

## Mapping Aliases

Use these aliases to find the official Apple starting point:

- Dialog/confirm/alert dialog -> Alerts, Sheets, or Modality depending on
  severity, platform, and dismissal behavior.
- Drawer/panel/bottom sheet -> Sheets, Sidebars, Toolbars, Modality, or Windows
  depending on platform and task.
- Navbar/header -> Navigation Bars or Toolbars; for macOS also check menu bar,
  sidebars, and window toolbar expectations.
- Tabs/segmented views -> Tab Bars for top-level app sections where appropriate;
  Segmented Controls for same-surface choices; Sidebars or split views for
  larger adaptive structures.
- Switch/checkbox -> Toggles or platform-native selection controls.
- Dropdown/select -> Menus, Pickers, or native select-style controls depending
  on option count, platform, and input method.
- Data grid -> Lists and Tables or Collections; use Charts only for visualized
  quantitative data.
- Progress bar/spinner/status display -> Progress Indicators, Status, Gauges,
  Activity Rings, or Feedback depending on task, platform, and duration.
- Rating/review UI -> Rating Indicators and Ratings and Reviews; do not invent
  star widgets without current HIG and App Store context.
- Search box -> Search Fields and Searching.
- Toast/banner/snackbar -> Feedback, Loading, Alerts, or inline recovery. Do
  not replace important errors with transient-only messages.

Aliases are routing aids only. They inherit the official component's behavior,
content, accessibility, and platform constraints.

## Component Anti-Patterns

- Button-like visuals on elements that are not interactive.
- Links that look like actions or buttons that navigate without link semantics.
- Custom controls without labels, focus, keyboard behavior, pointer/touch
  affordance, VoiceOver names, or state announcements.
- Controls that resize or shift when loading, selected, disabled, or localized.
- Sheets and alerts used for routine layout because the page lacks structure.
- iOS-style tab bars, switches, or navigation bars pasted into macOS/web
  surfaces without matching behavior.
- Icons or SF Symbols used as decoration instead of communicating a concrete
  object, action, or state.
