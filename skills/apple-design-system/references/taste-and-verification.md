## Apple Taste Gate

This is the mandatory quality gate for any task using this skill. The work is
not done until the verified scope passes official-source, platform, component,
asset, accessibility, and rendered-craft checks, or the final response states
the exact blockers and limited claim.

## Required Audit Loop

1. Run or inspect the app through the project's normal workflow and record the
   command, simulator/device/browser target, URL, or preview path.
2. Perform scope discovery: route/screen inventory, native targets, app entry
   points, navigation, shared primitives, design tokens, platform surfaces, and
   changed states. Include inaccessible, auth-gated, environment-gated, or
   dynamic screens with blocker reasons.
3. Select the target platform archetype and open current official Apple pages
   for the HIG root, platform, foundations, patterns, components, assets, and
   accessibility decisions that apply.
4. Complete the Foundation Gate from `foundation-and-style-rules.md`.
5. Complete platform/pattern mapping from `platform-and-pattern-map.md`.
6. Complete component mapping from `component-system.md`.
7. Complete the asset/license gate from `assets-and-licensing.md`.
8. Complete the privacy/data-use gate from `privacy-and-data-use-gate.md` when
   permissions, personal data, accounts, payments, tracking, or App Store-facing
   work is in scope.
9. Capture screenshots or equivalent visual evidence for changed screens/states
   across relevant device/window sizes. For web, inspect mobile, laptop,
   desktop, and wide viewports when the app can run. For native, use relevant
   simulators/previews/devices. For tvOS/watchOS/visionOS, include the platform
   input model and viewport/window context.
10. Run the interaction/accessibility matrix from
   `accessibility-and-verification.md`.
11. Scan anti-patterns in `apple-interface-craft.md`.
12. Revise failures, then repeat visual and interaction checks until the
    verified scope passes or a real blocker remains.

## Inventory Table

Use this during broad work:

`screen/surface/state | discovery source | official docs needed | platform/input | screenshot/evidence | interaction/accessibility | status`

For greenfield, full redesign, or broad polish work, every discovered routable
surface and required shared state must appear in the inventory. Whole-app claims
fail if any row is missing or incomplete.

## Pass Criteria

- Docs Evidence covers every required official Apple page for the verified
  surface, with exact page/section and concrete decision impact.
- The selected platform archetype matches the product: iOS, iPadOS, macOS,
  watchOS, tvOS, visionOS, or honest Apple-inspired web translation.
- Foundation evidence is visible in implementation: typography/text scaling,
  semantic color, layout/adaptivity, material/depth, SF Symbols/iconography,
  app-icon needs, motion, writing, accessibility, and privacy-sensitive states.
- Component evidence is visible: every mapped component or pattern follows the
  current official page and includes relevant states, input behavior, labels,
  focus, and accessibility.
- Assets pass license/trademark review: no unlicensed Apple fonts, logos,
  screenshots, product imagery, templates, SF Symbols misuse, or implied Apple
  affiliation.
- Privacy/data-use review passes when applicable: protected capabilities,
  personal data, tracking, accounts, payments, screenshots, and App Store-facing
  claims have official-source rows and recovery states.
- Existing product content, routes, data semantics, task flow, and brand intent
  were preserved unless the final report names a user request or concrete issue
  that required changing them.
- Screenshots or equivalent platform evidence show real UI states, not just a
  single static happy path.
- Layout survives relevant device/window sizes, Dynamic Type/text scaling,
  localization expansion, safe areas, split view/window resize, and input
  methods.
- Accessibility matrix passes or records exact blockers: VoiceOver/tree,
  keyboard/focus, platform input, appearance settings, reduced motion,
  increased contrast, reduced transparency, color differentiation, and recovery
  states.
- Anti-pattern scan finds no copied Apple app screens, fake native controls,
  generic Apple skinning, decorative blur/glass, unauthorized assets, tiny gray
  text, hover-only actions, or inaccessible custom controls.

## Official Claim Blockers

Do not claim `Apple Taste Gate passed`, `HIG-aligned`, `Apple-quality`,
`official-source-verified`, or `Production pass` when:

- A required official page was not opened or is blocked.
- Docs Evidence lacks an exact page/section or concrete decision impact.
- The app could run but screenshots/equivalent visual inspection were skipped.
- Interaction/accessibility checks were possible but skipped.
- Any required Apple asset/license check is unresolved.
- Any required privacy/data-use check is unresolved.
- The work copies Apple first-party screens or implies official Apple approval.
- The result is a web translation but is described as native HIG compliance.

Allowed limited claims:

- `local Apple-style fallback, not official-source-verified` when required docs
  are blocked.
- `docs consulted; visual/interaction verification blocked` when official pages
  were read but the app or visual checks could not run.
- `HIG-aligned candidate for verified scope` only when required docs,
  screenshots/evidence, interaction checks, and accessibility checks pass for
  that scope.

## Final Verification Checklist

Before finishing triggered visual work, verify:

- The first viewport/screen shows the real product or workflow unless the user
  explicitly requested marketing.
- The platform choice is explicit and supported by official Apple pages.
- Shared tokens/primitives carry the Apple-style decisions; there are no
  isolated Apple-looking widgets inside unrelated styling.
- Typography, color, material, icon, and motion choices are mapped to official
  pages and project primitives.
- Native frameworks use system components where possible; web translations keep
  HTML semantics, focus, zoom, and browser behavior intact.
- Every form/control has labels, states, error/recovery, focus, and relevant
  input behavior.
- Loading, empty, error, permission, privacy, destructive, and offline states
  are designed when applicable.
- Apple-owned fonts, symbols, logos, product images, templates, and marks are
  absent or explicitly permitted for the target use.
- Final response includes Docs Evidence, commands, simulator/browser target,
  screenshot/evidence paths or blockers, checked states, revisions made, and
  any `whole app not verified` limitation.
