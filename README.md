# Skills

[![skills.sh](https://skills.sh/b/joe-simo/skills)](https://skills.sh/joe-simo/skills)

Community Agent Skills by `joe-simo`.

## Vercel Geist Design System

`vercel-geist-design-system` is a community Agent Skill for designing and reviewing Vercel-inspired interfaces with the Geist design system. It helps agents apply Geist typography, spacing, colors, materials, component styling, app shells, interaction states, screenshot audits, and UI polish across React, Next.js, Tailwind, shadcn, Radix, and other frontend surfaces.

The skill treats official Vercel sources as the design authority: Geist Font, Geist foundations, Geist component pages, Geist Brands, and the Vercel Web Interface Guidelines. Skills.sh companions are routing helpers only; they do not replace official Geist docs or prove Geist compliance by themselves.

For existing products, the skill now includes a preservation gate: agents should restyle intentional content, routes, CTAs, brand-defining effects, credential displays, navigation, contact paths, and footer ownership before replacing or inventing alternatives. This is public guidance for any project using the skill, not a project-specific rule.

The main `SKILL.md` stays compact for lower initial context use. Detailed source gates, component mappings, style rules, companion routing, and verification checks live in `skills/vercel-geist-design-system/references/` and are loaded only when relevant.

The current companion routing covers:

- Core Geist and guideline helpers: `geist`, `geistdocs`, and `web-design-guidelines`
- Implementation helpers: `building-components`, `shadcn`, React best practices, Next.js guidance, and Vercel composition patterns
- Verification helpers: browser automation, browser verification, full-flow verification, and before/after visual comparison
- Conditional surfaces: AI Elements, Streamdown, `json-render/react-three-fiber`, View Transitions, Geist learning labs, and Remotion Geist video work

The skill intentionally avoids routing Vercel platform/runtime skills for visual design work unless the user explicitly asks for that product capability.

This is community-authored by `joe-simo`. It is not an official Vercel skill.

## Install

```bash
npx skills add joe-simo/skills
npx skills add joe-simo/skills --skill vercel-geist-design-system
```

## Example Prompts

```txt
Design this Next.js dashboard with strict Vercel Geist system quality.
```

```txt
Review this React app and make the UI feel like a cohesive Geist-based product.
```

```txt
Refactor these shadcn components so they follow Geist typography, spacing, materials, and interaction patterns.
```

```txt
Audit this landing page and app shell against Vercel Geist design-system expectations.
```

```txt
Create an AI chat surface that uses Vercel-style Geist UI, with AI Elements only as implementation infrastructure.
```

```txt
Render a constrained React Three Fiber scene from json-render inside a Geist-styled product page.
```

## Attribution

GitHub: `joe-simo`

X: `@joesimo`

Website: [joesimo.com](https://joesimo.com)

## Links

- [skills.sh/joe-simo/skills](https://skills.sh/joe-simo/skills)
- [skills.sh/joe-simo/skills/vercel-geist-design-system](https://skills.sh/joe-simo/skills/vercel-geist-design-system)
