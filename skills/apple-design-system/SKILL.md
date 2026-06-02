---
name: apple-design-system
description: >-
  Community skill for designing, redesigning, reviewing, and polishing
  Apple-style interfaces using official Apple Human Interface Guidelines and
  Apple Developer design resources only. Use for platform-native and
  Cupertino-style UI across iOS, iPadOS, macOS, watchOS, tvOS, visionOS,
  SwiftUI, UIKit, AppKit, and web translations; typography, semantic color,
  layout, materials, Liquid Glass, SF Symbols, app icons, navigation, controls,
  components, accessibility, motion, platform adaptation, responsive behavior,
  asset/licensing boundaries, screenshots, and Apple-quality UI polish.
  Community-authored, not official Apple. Trigger for Apple HIG, Apple design,
  Apple-style UI, iOS UI, macOS UI, visionOS UI, Cupertino UI, SF Pro, SF
  Symbols, Liquid Glass, or native-feeling Apple-platform product design. Skip
  non-visual work unless it materially changes rendered UI.
metadata:
  author:
    github: joe-simo
    x: "@joesimo"
    website: https://joesimo.com
  community: true
  official: false
  short-description: Unofficial Apple HIG visual-system skill for native-feeling Apple-platform and Apple-style UI using official Apple sources only
  sources:
    - https://developer.apple.com/design/
    - https://developer.apple.com/design/human-interface-guidelines/
    - https://developer.apple.com/design/human-interface-guidelines/getting-started
    - https://developer.apple.com/design/human-interface-guidelines/foundations
    - https://developer.apple.com/design/human-interface-guidelines/patterns
    - https://developer.apple.com/design/human-interface-guidelines/components/
    - https://developer.apple.com/design/human-interface-guidelines/inputs
    - https://developer.apple.com/design/human-interface-guidelines/technologies
    - https://developer.apple.com/design/resources/
    - https://developer.apple.com/fonts/
    - https://developer.apple.com/sf-symbols/
    - https://developer.apple.com/documentation/technologyoverviews/interface-fundamentals
    - https://developer.apple.com/documentation/technologyoverviews/liquid-glass
    - https://developer.apple.com/support/terms
    - https://www.apple.com/legal/intellectual-property/guidelinesfor3rdparties.html
---

# Apple Design System

Use this community skill to make interfaces feel native to Apple platforms and
aligned with Apple's Human Interface Guidelines. Official Apple Developer pages
are the only design authority. This is not official Apple guidance and is not
permission to copy Apple apps, Apple marketing, Apple icons, Apple trademarks,
or private system UI.

## Reference Loading Contract

This compact file is the operating contract. Detailed rules live in
`references/`; load only what the task needs, but never skip a required gate
because this summary seems sufficient.

- Always load `references/source-of-truth-gate.md` for triggered visual work
  before claiming HIG alignment, Apple-quality polish, official-source
  verification, or Apple Taste Gate passage.
- Load `references/official-reference-map.md` when mapping foundations,
  platforms, patterns, components, assets, or technologies to current official
  Apple URLs.
- Load `references/foundation-and-style-rules.md` before creating, restyling,
  redesigning, reviewing, or materially changing rendered UI.
- Load `references/platform-and-pattern-map.md` before native app work,
  platform adaptation, multi-device design, web translation, navigation,
  modality, windowing, input, or spatial/tv/watch surfaces.
- Load `references/component-system.md` before controls, forms, navigation
  bars, tab bars, sidebars, toolbars, sheets, alerts, menus, lists, tables,
  collections, search, status states, or custom components.
- Load `references/component-and-interaction-coverage.md` for per-control
  choice rules, navigation/search/menu/modal details, forms/data entry,
  focus/keyboard/pointer/remote/crown/spatial input, haptics, or audio.
- Load `references/apple-interface-craft.md` before high-polish visual
  implementation, critique, redesign, or anti-template revision.
- Load `references/assets-and-licensing.md` before fonts, SF Symbols, app
  icons, Apple Design Resources, product bezels, logos, badges, Apple Pay,
  Sign in with Apple, Apple Wallet, or trademark-sensitive work.
- Load `references/privacy-and-data-use-gate.md` before permissions, tracking,
  accounts, sign-in, payments, health, location, camera, microphone, contacts,
  photos, personal data, screenshots with real data, or App Store-facing work.
- Load `references/accessibility-and-verification.md` before final
  implementation review, simulator/browser checks, screenshots, accessibility
  checks, or final response.
- Load `references/taste-and-verification.md` before final audit, screenshots,
  interaction checks, or final response for triggered visual work.

Use current official Apple pages before implementation or strict claims. Do not
use blogs, screenshots, cloned Apple UI, third-party design kits, template
repos, extracted private assets, or unofficial HIG summaries as authority.
Implementation and verification helpers may support native, web, browser, or
simulator work, but they never replace official Apple docs and never satisfy
Docs Evidence by themselves.

## Trigger Policy

Trigger when a task creates, changes, critiques, specifies, or materially
directs rendered UI and asks for Apple HIG, Apple design, Apple-style UI,
iOS/iPadOS/macOS/watchOS/tvOS/visionOS UI, native Apple-platform feel,
Cupertino UI, SF Symbols, SF Pro, Liquid Glass, or Apple-quality polish.

Do not trigger for backend-only work, build tooling, tests, data wiring, or
behavior-only fixes unless rendered UI is created or materially changed. An
explicit non-Apple final visual system overrides this skill.

## Content, IA, And Product Preservation Gate

When applying Apple style to an existing product, preserve user-approved
content, brand identity, routes, navigation intent, platform role, data model,
and task flow unless the user explicitly asks to change them or they create a
concrete accessibility, performance, correctness, security, privacy, or
legal/trademark problem.

Restyle before replacing. Do not turn every app into a Settings clone, iPhone
mockup, Apple.com marketing page, or fake native shell. Use the target
platform's official patterns to support the product's real workflow.

## Operating Loop

1. Identify the platform, surface, audience, task, input methods, device
   classes, app/window context, content, and implementation stack.
2. Inspect the project before designing: native framework or web stack, current
   components, design tokens, icon/font setup, routing/navigation, validation
   commands, accessibility tooling, and existing brand language.
3. Load required references and open current official Apple pages for every
   applied foundation, platform, pattern, control, symbol, icon, material, and
   accessibility claim.
4. Choose the platform archetype before styling. iOS, iPadOS, macOS, watchOS,
   tvOS, and visionOS have different density, navigation, input, windowing,
   depth, focus, motion, typography, and accessibility expectations.
5. Complete the foundation gate: typography, semantic colors, layout/adaptivity,
   materials, depth, iconography/SF Symbols, app icon needs, accessibility, and
   platform states.
6. Map each UI requirement to an official Apple foundation, platform pattern,
   component, or constrained custom composition before inventing behavior.
7. Complete asset/license and privacy gates whenever Apple resources, protected
   capabilities, personal data, or screenshots/evidence are in scope.
8. Implement through project-local primitives and platform-native APIs when
   available. For web, translate Apple principles without claiming native HIG
   compliance or using restricted Apple assets.
9. Verify across platform-relevant viewports/devices/states, interaction
   methods, accessibility settings, appearance modes, and motion/material
   preferences. Revise failures before final response.

## Non-Negotiables

Official Apple Developer documentation is binding input, not optional
inspiration. If the needed official Apple pages cannot be loaded after available
browsing/docs tools are attempted, state attempted URLs and failures. Local
rules then become advisory only and cannot support `official-source-verified`,
`HIG-aligned`, or `Apple-quality` claims.

Official source evidence must be page-specific. A generic memory of Apple UI,
system font usage, SF Symbols usage, rounded corners, blur, or platform-looking
classes does not prove HIG alignment. If the result looks merely like a generic
Apple-flavored skin and not a platform-appropriate product surface, revise it.

Do not copy Apple product screens, Settings.app, Apple.com marketing,
first-party app layouts, icons, wallpapers, screenshots, private symbols,
private materials, trademarked product art, or Apple trade dress. Use Apple
names, platform names, SF Symbols, and official guidelines only as nominative
references when needed.

Respect Apple asset and font licensing. Use system fonts through platform APIs
or CSS system stacks where appropriate. Do not commit, bundle, serve, export,
or redistribute Apple fonts, SF Symbols, Apple logos, product bezels,
templates, screenshots, wallpapers, or other Apple-owned graphic assets unless
the project has rights and the official license permits the exact target use.

Apple style is not just rounded rectangles, blur, or a Cupertino color palette.
Native-feeling Apple UI is platform-adapted, content-first, direct, legible,
semantic, restrained, accessible, responsive to system settings, and respectful
of user control.

## Verification Contract

Before final response for triggered visual work, run the Apple Taste Gate in
`references/taste-and-verification.md`: scope inventory, current official docs,
Foundation Gate, platform/pattern mapping, component mapping, asset/license
gate, privacy/data-use gate, screenshots or simulator/browser inspection,
accessibility/interaction checks, anti-pattern scan, and revision loop.

If a native or web app can run, inspect the relevant platform/device/window
sizes plus changed states such as menus, alerts, sheets, search, forms, empty
states, loading, errors, privacy/permission prompts, and dense data views. If
screenshots or interaction checks are possible and not captured, do not claim
the Apple Taste Gate passed. If verification is blocked, state the exact
blocker and use only the allowed limited claim.

Final responses must report the important evidence concisely: commands, URL or
simulator/device target, viewport/window sizes, screenshot paths or blocker,
changed states inspected, accessibility summary, Docs Evidence, revisions made
because of the audit, and any `whole app not verified` scope limit.
