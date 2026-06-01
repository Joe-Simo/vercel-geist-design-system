## Reference-First Contract

Official Apple Developer documentation is the design authority. This skill is
the enforcement layer that makes the agent use current official Apple sources
instead of memory, screenshots, templates, or generic Cupertino styling.

- Do not rely only on this skill summary when official docs are available.
- For UI that creates, changes, critiques, specifies, or materially directs
  rendered output, consult the HIG root plus every applied foundation, platform,
  pattern, component, accessibility, and asset/license page.
- Use `official-reference-map.md` to find official Apple URLs, then open the
  relevant live page in the current turn before implementation or strict claims.
- If a required official page cannot be read, follow the fallback and claim
  limits below.
- Do not treat system-font usage, SF Symbols usage, rounded corners, blur,
  native-looking classes, or copied app screenshots as sufficient. The visual
  result must be platform-adapted, legible, semantic, accessible, and coherent
  across the verified surface.

## Required Workflow

1. Identify the platform, surface, context, user task, input methods, device or
   window classes, content, and implementation stack.
2. Select the matching Apple platform and pattern references before designing.
   Do not use iPhone, Settings, or Apple.com marketing composition as the
   universal target.
3. Inspect the project first: framework, native UI layer or web stack, theme
   tokens, component primitives, font/icon setup, routing/navigation, validation
   commands, accessibility tooling, and current brand language.
4. Open the required official Apple foundation and platform pages, then
   complete the Foundation Gate before screen-level styling.
5. Map every UI requirement to the closest official Apple pattern/component or
   platform-native API before creating a custom pattern.
6. Preserve existing product content, routes, data semantics, and workflow
   intent unless a concrete issue or user request requires change.
7. Follow the host project's language, framework, package-management, and
   validation conventions.

## Official Source-Of-Truth Gate

For any task using this skill, current official Apple docs are binding design
input, not optional inspiration. Before visual implementation, open the
relevant official pages for foundations, platforms, components, patterns,
accessibility, assets, and guidelines. Do not rely on memory, screenshots,
generic Apple heuristics, or third-party kits when an official Apple page covers
the decision.

Required pages by decision type:

- Foundations: HIG root, Typography, Color, Layout, Materials, SF Symbols, App
  Icons, Motion, Writing, and Accessibility as applicable.
- Platform: the official target platform page, such as iOS, iPadOS, macOS,
  watchOS, tvOS, or visionOS.
- Components/patterns: every concrete matching component or pattern URL from
  `official-reference-map.md`, such as Buttons, Tab Bars, Sidebars, Sheets,
  Alerts, Text Fields, Search Fields, Lists and Tables, or Modality.
- Assets/licensing: Apple Design Resources, Apple Fonts, SF Symbols, developer
  terms, and any technology-specific page for Apple Pay, Sign in with Apple,
  Wallet, product bezels, badges, logos, or marks.

Apple legal, terms, and license pages can satisfy asset/license and trademark
checks only. They are not visual design authority and do not replace HIG
foundation, platform, pattern, component, accessibility, or writing pages.

If a listed page redirects or cannot be loaded, do not treat it as source of
truth. Use the closest accessible official Apple page only as supplemental
context and state the fallback. The original required topic remains `blocked`
unless the relevant official page or section was read. If a listed page
redirects to a canonical Apple URL, record the final URL in Docs Evidence and
prefer that non-redirecting URL in future edits.

## Docs Evidence Contract

For triggered visual work, the final response must include a concise Docs
Evidence table with one row for every required official page for the task.

Use these columns:

`official URL | status | exact page/section | short exact quote or exact failure | implementation target | concrete decision/change | verification`

Rules:

- A consulted row must name the exact official page or section and include a
  short source-specific quote or paraphrased evidence that affected a concrete
  implementation decision. Keep quotes brief and copyright-safe.
- Foundation, platform, accessibility, asset/license, and applied component rows
  can be only `consulted` or `blocked`.
- Adjacent checked-and-rejected component rows can be `not applicable` only with
  a rejection reason.
- A required applied page is `blocked` only if available browsing/docs tools
  were attempted in the current turn and the row names the exact failures.
- Do not claim `HIG-aligned`, `Apple-quality`, `official-source-verified`,
  `Apple Taste Gate passed`, official Apple compliance, Apple approval, App
  Store review outcome, or platform acceptance if any required applied row is
  missing, blocked, lacks a page/section, or lacks concrete verification.
- Do not claim all-in-one or broad system coverage when required category/index
  pages from `official-reference-map.md` were not checked for the task scope.
- If any required source is blocked, the only allowed claim for affected
  surfaces is `local Apple-style fallback, not official-source-verified`.
- If screenshots, simulator, browser, or interaction checks are possible and
  not performed, use only `docs consulted; visual/interaction verification
  blocked`, not `Apple Taste Gate passed`.

## Forbidden Authorities

Do not use blogs, Medium posts, Dribbble shots, Figma community files,
reverse-engineered app screenshots, third-party UI kits, template repos,
StackOverflow, Reddit, unofficial HIG mirrors, or copied Apple product screens
as design authority.

Do not use old HIG PDFs or archived docs when current Apple Developer pages are
available. Archived docs can explain legacy behavior only when the product must
support legacy Apple platforms and current docs do not cover the question.

## Originality And Trademark Posture

- Community skill, not official Apple.
- Apple HIG is design authority; Apple app screens are not templates to clone.
- Do not reproduce Apple proprietary artwork, product imagery, wallpapers,
  icons, app screens, symbols outside license, or Apple marketing composition.
- For web/non-Apple products, translate platform principles; do not imply the
  product is made by Apple, endorsed by Apple, or using official Apple UI
  assets.
