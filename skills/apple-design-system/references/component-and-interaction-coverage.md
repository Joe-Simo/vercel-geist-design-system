## Component And Interaction Coverage

Use this after `component-system.md` when a task involves concrete Apple
components, navigation, forms, input, focus, haptics, audio, or platform
interaction. It provides routing and choice rules; official Apple pages remain
the source of truth.

For every applied item, record:

`need | selected Apple page | exact section | platform variant | rejected alternatives | states/input | accessibility | verification`

## Navigation And Structure

- Start with Navigation and search, then select the concrete structure:
  navigation bar, tab bar, tab view, sidebar, split view, toolbar, menu bar, or
  window.
- Use tab bars for top-level app sections, not actions. Check sidebar/tab
  adaptation on iPadOS and larger contexts.
- Use sidebars and split views for hierarchical or multi-pane content,
  especially iPadOS/macOS and adaptable layouts.
- Use toolbars for commands that affect current content. Group actions, handle
  overflow, and keep primary actions visible without overloading the bar.
- macOS work must consider menu bar commands, keyboard shortcuts, resizable
  windows, sidebars, inspectors, and window toolbar behavior.

Official pages: Navigation and search, Navigation Bars, Tab Bars, Tab Views,
Sidebars, Split Views, Toolbars, Windows, The Menu Bar, Keyboards.

## Menus And Commands

- Choose the menu type by intent: menu bar for app/document commands, context
  menu for object-specific secondary actions, pull-down/pop-up buttons for
  compact command or option sets, and standard menus for grouped actions.
- Keep menu labels specific. Use icons only when they clarify common actions.
- Preserve unavailable/disabled states instead of hiding important commands
  when people need to understand state.
- Destructive commands need clear labeling, confirmation or undo where
  appropriate, and platform-consistent placement.

Official pages: Menus, Menus and actions, Context Menus, The Menu Bar,
Pull-down Buttons, Pop-up Buttons, Buttons, Keyboards.

## Modality, Sheets, Alerts, And Popovers

- Use alerts for urgent decisions, destructive confirmation, or critical
  information requiring action.
- Use sheets for focused tasks related to the current context. Avoid modal
  stacking and provide clear dismissal/recovery.
- Use popovers for lightweight contextual controls where the platform supports
  them; do not use them as full-screen navigation.
- Action sheets are for compact action choices where the platform pattern fits.
- Unsaved-change flows require explicit save/discard/cancel semantics and focus
  restoration.

Official pages: Modality, Alerts, Sheets, Action Sheets, Popovers, Buttons,
Writing, Accessibility.

## Forms, Data Entry, And Search

- There is no universal HIG "form" shortcut. Build forms from official data
  entry, text field, label, picker, toggle, segmented control, stepper, slider,
  search, token field, keyboard, and accessibility guidance.
- Every editable control needs a persistent label or equivalent accessible name,
  useful placeholder/example text only when appropriate, validation near the
  problem, and keyboard/input type appropriate to the platform.
- Search must be discoverable, scoped, cancellable, and recoverable. Include
  suggestions, tokens, scopes, or filters only when they improve the task.
- Avoid pre-disabling submission to hide validation. Let people discover and
  fix errors with focused, local messages.

Official pages: Entering Data, Text Fields, Labels, Virtual Keyboards, Search
Fields, Searching, Token Fields, Pickers, Sliders, Toggles, Steppers, Segmented
Controls, Accessibility.

## Lists, Tables, Collections, And Data Views

- Choose Lists and Tables for rows, structured data, settings, or tabular
  comparison; choose Collections for visual grids or repeated content objects.
- Define whether selection navigates, edits, toggles, or opens detail. Do not
  make row behavior ambiguous.
- Include empty, loading, error, no-results, reorder, delete, edit, sorting, and
  filtering states when the data model can enter them.
- macOS tables need sorting/resizing/keyboard and pointer behavior where the
  task expects it.
- For hierarchy, consider sidebars, split views, outline views, or disclosure
  rather than deep nested custom cards.

Official pages: Lists and Tables, Collections, Outline Views, Scroll Views,
Sidebars, Split Views, Searching, Accessibility.

## Control Choice Rules

- Buttons initiate immediate actions. Style, content, and role must communicate
  meaning.
- Pickers choose from a constrained set; menus/pull-downs are not automatic
  replacements when platform picker behavior is expected.
- Sliders adjust a continuous value; pair with exact values when precision
  matters and give immediate feedback.
- Toggles represent binary state. Use checkboxes/radio-style controls only when
  the platform and native framework actually expose that pattern.
- Steppers adjust a value in discrete increments and need the value nearby.
- Segmented controls switch related views or modes on the same surface; do not
  use them as decoration or overloaded navigation.

Official pages: Buttons, Pickers, Sliders, Toggles, Steppers, Segmented
Controls, Labels, Accessibility.

## Input, Focus, And Gestures

- Standard gestures should behave as people expect. Custom gestures need visual
  affordance, discoverability, feedback, and accessible alternatives.
- Drag and drop needs valid drop feedback, copy/move semantics, undo/recovery,
  and no hidden destructive action.
- Keyboard support must respect standard shortcuts, Full Keyboard Access, focus
  order, and localized shortcut behavior.
- Pointer, focus engine, remote, Digital Crown, and eye/hand input need
  platform-specific evidence. Do not verify tvOS/watchOS/visionOS from a mouse
  screenshot only.

Official pages: Gestures, Drag and Drop, Pointing Devices, Focus and Selection,
Keyboards, Game Controllers, Digital Crown, Designing for tvOS, Designing for
watchOS, Designing for visionOS, Spatial Layout.

## Haptics, Audio, And Feedback

- Use haptics and audio to reinforce state, success, warning, or physicality;
  never make sound/haptics the only way to perceive critical information.
- Respect silent mode, system volume, reduced motion/comfort, and user control.
- Keep custom haptics/audio consistent; avoid novelty feedback in productivity
  flows.
- visionOS audio/spatial experiences require comfort and immersion evidence.

Official pages: Feedback, Playing Haptics, Playing Audio, Motion,
Accessibility, Designing for visionOS.

## Status, Progress, Ratings, And Reviews

- Use progress indicators only for actual pending work; preserve layout and
  explain blocking waits when needed.
- Use status and gauges for state people need to monitor or compare; pair color
  with text, symbols, or shape.
- Use rating indicators and ratings/reviews only when the product genuinely
  collects, displays, or links to review information. App Store-facing review
  flows require current App Store and HIG evidence.
- Complications, activity rings, Live Activities, and notifications are
  platform surfaces, not decorative widgets; verify their exact official pages.

Official pages: Status, Progress Indicators, Gauges, Rating Indicators, Ratings
and Reviews, Activity Rings, Complications, Live Activities, Notifications.

## Per-Component Claim Rule

Do not claim Apple-quality component work unless each changed component has:

- Required official page row and platform variant.
- States and error/recovery behavior.
- Input and focus behavior for the target platform.
- Accessibility-tree or native accessibility evidence.
- Screenshot/simulator/browser evidence for relevant sizes and appearances.
