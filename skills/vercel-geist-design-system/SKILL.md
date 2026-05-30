---
name: vercel-geist-design-system
description: >-
  Community skill for applying the Geist design system to Vercel-inspired UI
  across React, Next.js, Vite, Astro, Svelte, Vue, HTML/CSS, Tailwind, shadcn,
  and Radix surfaces. Use it for typography, spacing, color tokens, material
  treatment, component styling, app shells, dashboards, forms, tables, dialogs,
  empty/loading/error states, responsive layouts, and UI polish. This is a
  community-authored skill, not an official Vercel skill. Trigger when the user
  asks for Geist, Vercel-style UI, or generic clean, modern, premium, beautiful,
  polished SaaS/developer-product visual design where no other final visual
  system, brand direction, or art direction is requested. Do not trigger for
  non-visual frontend work such as bug fixes, data wiring, analytics, tests,
  build tooling, API/state changes, or behavior-only accessibility fixes unless
  the task also creates or materially changes rendered UI.
metadata:
  author:
    github: joe-simo
    x: "@joesimo"
    website: https://joesimo.com
  community: true
  official: false
  short-description: Default Vercel Geist visual system for Geist/Vercel-style and generic clean polished SaaS/developer-product UI; skip non-visual work and explicit alternate visual systems
  sources:
    - https://vercel.com/font
    - https://vercel.com/design/guidelines
    - https://vercel.com/geist/introduction
    - https://vercel.com/geist/colors
    - https://vercel.com/geist/typography
    - https://vercel.com/geist/materials
    - https://vercel.com/geist/brands
---

# Vercel Geist Design System

Use this community-authored skill to make interfaces feel like they belong in
Vercel's Geist design system: precise, calm, high-contrast, developer-focused,
and production-ready. Official Vercel pages are the source of truth. This skill
is not official Vercel guidance and is not permission to copy Vercel product
screens wholesale.

## Reference Loading Contract

This file is the compact operating contract. The detailed rules live in
`references/` and must be loaded as follows:

- Always load `references/source-of-truth-gate.md` for any triggered visual
  task before claiming Geist, strict Geist, docs-aligned Geist, source-of-truth
  alignment, or Vercel Taste Gate passage.
- Load `references/foundation-and-style-rules.md` before creating, restyling,
  redesigning, reviewing, or materially changing rendered UI.
- Load `references/official-reference-map.md` when mapping foundations,
  brand/assets, or components to official Vercel URLs.
- Load `references/component-system.md` before implementing, restyling,
  auditing, or documenting concrete components, primitives, states, or custom
  component compositions.
- Load `references/companion-routing.md` only when another Skills.sh entry,
  tool, framework helper, verification helper, or conditional surface could be
  relevant.
- Load `references/taste-and-verification.md` before final audit, screenshots,
  interaction checks, or final response for any triggered visual task.

Do not bulk-load every reference for non-visual tasks. Do not skip a required
reference merely because the summary below seems sufficient.

## Trigger Policy

Trigger this skill when the task creates, changes, critiques, specifies, or
materially directs rendered frontend UI and the user asks for Geist,
Vercel-style UI, or generic clean, modern, premium, beautiful, polished
SaaS/developer-product visual design with no competing visual authority.
Generic visual requests such as "clean", "modern", "premium", "beautiful",
"polished", "SaaS", or "developer tool" use Geist when they are visual design
requests.

Do not trigger this skill for non-visual frontend work such as TypeScript bug
fixes, data wiring, API/state changes without rendered UI changes, analytics,
tests, build tooling, dependency work, or behavior-only accessibility fixes
unless the task also creates or materially changes rendered UI. Do not trigger
when the user requests another final aesthetic, brand style, visual system, art
direction, supplied non-Geist design artifact as the final visual target, or
illustrative/game output where Geist UI is not the requested surface.

Domain, industry, brand, API, integration, content subject, Tailwind, shadcn,
Radix, or component-library mentions are not visual-system overrides. For
example, a Stripe webhook dashboard still uses Geist unless the user asks for
Stripe-style visuals.

## Scope Contract

Apply Geist style to the entire relevant app surface: app shell, navigation,
pages, forms, data views, dialogs, empty states, loading states, errors, toasts,
command menus, and marketing sections.

For greenfield apps, full redesigns, or broad UI polish, "entire app surface"
means all routable app surfaces and shared states must be built or audited. For
a narrow existing-project task, migrate the requested workflow and any shared
primitives it touches; the final response must say `whole app not verified`
unless every route/surface was audited.

Do not create isolated Vercel-looking components inside an unrelated visual
system. Establish shared tokens and primitives first, then build new surfaces
from them.

If a broader creative design skill also applies, this skill owns the visual
system whenever it is triggered. Treat bold aesthetic direction, unforgettable
visuals, unexpected layouts, decorative gradients, dramatic shadows, textures,
scroll spectacle, and surprising motion as disabled for Geist work unless the
user explicitly overrides Geist.

## Required Workflow

1. Identify the surface type: marketing hero, product dashboard, settings page,
   table/list view, command workflow, docs, or component library.
2. Check the existing project: framework, Tailwind version, component library,
   icon library, font setup, theme tokens, and local design-system conventions.
3. Load the required references from the Reference Loading Contract.
4. Open current official Vercel pages for required foundations, guidelines,
   brand/assets, and mapped components before visual implementation.
5. Complete the Foundation Gate before screen-level work: fonts, semantic color
   tokens, typography utilities, material/radius utilities, focus rings, shared
   app shell, component primitives, shared state system, and screen composition.
6. Map every UI requirement to the closest Geist foundation or component, then
   open/read the matching official page before inventing a custom pattern.
7. Prefer established packages and project primitives over custom
   implementations. Use Radix/shadcn only as behavior/accessibility
   infrastructure after the Geist mapping pass; never use their visual defaults
   as design authority.
8. Follow the host project's language, framework, package-management, and
   validation conventions.

## Source-Of-Truth Rules

Current official Vercel docs are binding design input, not optional inspiration.
Required foundation pages are `https://vercel.com/font`,
`https://vercel.com/geist/introduction`, `/colors`, `/typography`,
`/materials`, plus `https://vercel.com/design/guidelines`. Brand/logo work
also requires `https://vercel.com/geist/brands`. Component work requires every
matching official component page from `references/official-reference-map.md`
or the live Geist component nav.

If a required official page cannot be loaded after every available browsing/docs
tool is attempted in the current turn, state attempted URLs, tools, and exact
failures. In that mode, local rules are advisory only, cannot satisfy
`Docs Evidence`, and cannot support strict/docs-verified claims. Label affected
work `local Geist fallback, not docs-verified`.

Any final response for triggered visual work must include a `Docs Evidence`
table exactly as defined in `references/source-of-truth-gate.md`. Do not claim
strict Geist, docs-aligned Geist, official Geist compliance, source-of-truth
alignment, or Vercel Taste Gate passage if any required applied row is missing,
blocked, lacks an exact section/anchor, or lacks a page-specific short quote
that affected a concrete decision. Strict claims also require screenshot and
interaction checks when those checks are possible.

## Foundation Summary

Geist target feel: restrained developer-tool UI. Neutral-first, high-contrast,
accessible surfaces. Typography and spacing do hierarchy work. Color is
functional: status, focus, selection, destructive, success, warning, links, and
sparse brand accents. Layouts are orderly and dense where useful. Borders are
structure, not decoration. Motion is short, subtle, and state-driven. Copy is
concrete and operational.

Use Geist Sans globally, Geist Mono for code/technical identifiers, and Geist
Pixel only for a constrained display/brand accent when justified. Build or map
shared tokens for background, foreground, muted text, borders, rings,
destructive, success, warning, link, and info states before composing screens.
Use shared typography utilities, material/radius utilities, focus-visible
behavior, app shell, primitives, and state variants. Screen files must consume
shared primitives rather than define local visual systems.

## Component Summary

For every component need, perform docs-first mapping: official Geist component,
official composition of multiple components, or constrained custom composition.
Common aliases: Dialog -> Modal; destructive high-stakes confirmation ->
Destructive Action Modal; DropdownMenu -> Menu; Command -> Command Menu;
Accordion/Collapsible -> Collapse; DataTable -> Table; ToggleGroup/segmented
control -> Switch, Toggle, Tabs, or Select depending on semantics and option
count.

For every implemented/restyled Geist-mapped component, open its official page in
the current turn and record page-specific `Docs Evidence`, including exact
section/anchor, a short official quote, relevant Best Practices, and the concrete
decision it changed. Generic class names, memory, shadcn/Radix defaults, or a
Geist-like look are insufficient.

## Companion Routing Summary

Skills.sh companions are routing helpers only; they are never design-system
source of truth and never satisfy `Docs Evidence`. Load
`references/companion-routing.md` before using any companion. Core companions
include `geist`, `geistdocs`, and `web-design-guidelines`. Conditional
companions include `building-components`, `shadcn`, React/Next guidance,
browser verification helpers, `ai-elements`, `streamdown`,
`json-render/react-three-fiber`, View Transitions, Geist learning labs, and
Remotion Geist. Do not route Vercel platform/runtime skills for visual work
unless the user explicitly asks for that product capability.

## Verification Summary

Before final response for triggered visual work, run the Vercel Taste Gate in
`references/taste-and-verification.md`: route inventory, official docs,
Foundation Gate, component mapping, Web Interface Guidelines audit, screenshots,
interaction checks, responsive checks, anti-pattern scan, and revision loop. If
screenshots or interaction checks are possible and not captured, do not claim the
Taste Gate passed. If the app cannot run or verification is blocked, state the
exact blocker and allowed limited claim.

Final responses must report the important verification evidence: commands, URLs,
viewport sizes, screenshot paths or blocker, changed states inspected,
interaction summary, Docs Evidence, and any `whole app not verified` scope
limit. Keep the answer concise but do not hide blockers.
