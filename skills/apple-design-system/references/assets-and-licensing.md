## Assets And Licensing

Apple visual resources are not generic clip art. Use official Apple pages and
licenses before adding, bundling, exporting, or modifying Apple-owned resources.

## Required Asset Gate

For any font, symbol, icon, logo, badge, product image, bezel, template, or
Apple technology mark, record:

`asset | official Apple URL/license | intended use | permitted scope checked | implementation | verification`

Do not proceed from memory or third-party downloads.

## Fonts

- Prefer platform/system fonts through native APIs or CSS system stacks.
- Do not commit, bundle, serve, redistribute, or make Apple font files available
  over a network unless the project has rights and the official font license
  permits the exact target use.
- Use `https://developer.apple.com/fonts/` and
  `https://developer.apple.com/fonts/system-fonts/` for font availability and
  license context.
- For web, a system stack can request Apple platform fonts already installed on
  the user's device; it does not license bundling Apple font files.
- If typography requires a bundled web font, use a licensed non-Apple font or
  project-owned font unless Apple licensing explicitly permits the use.

## SF Symbols

- Use `https://developer.apple.com/design/human-interface-guidelines/sf-symbols`
  and `https://developer.apple.com/sf-symbols/` before symbol decisions.
- Check symbol availability against the deployment target.
- Match symbol weight, scale, rendering mode, and baseline to adjacent text.
- Do not use SF Symbols, or confusingly similar symbols, in app icons, logos,
  branding, or trademarked use.
- Do not export SF Symbols into non-Apple products unless the official terms
  permit that exact use.

## Apple Design Resources

- Use `https://developer.apple.com/design/resources/` for official templates,
  UI kits, icon templates, color guides, product bezels, tools, and technology
  assets.
- Use the Apple Design Resources license and relevant developer terms before
  using downloaded resources. Treat the license scope as narrow until verified
  for the exact product, platform, and deliverable.
- Official design resources are for designing Apple-platform software under
  their terms; they are not a license to ship Apple UI assets in arbitrary
  products or marketing.
- Do not use Figma community kits, extracted Apple assets, screenshots, private
  symbols, or reverse-engineered resources as substitutes.

## App Icons And Product Artwork

- Use the App Icons HIG page and current Apple Design Resources templates for
  platform-specific icon work.
- App icons must be original to the product. Do not include Apple logos, Apple
  hardware silhouettes, SF Symbols as logos, screenshots, text-heavy artwork, or
  Apple marketing imagery unless official guidance and rights permit it.
- Product bezels and App Store marketing assets require the relevant official
  Apple resource/terms. Do not invent device art that implies Apple endorsement.
- App Store badges, product-page artwork, screenshots, previews, promotional
  lockups, and campaign assets require the current App Store Marketing
  Guidelines and App Review Guidelines when App Store distribution or marketing
  is in scope.

## Apple Technology Marks

- For Apple Pay, Sign in with Apple, Wallet, Health, Music, App Store badges, or
  related marks, use only the official Apple technology page, marketing
  guidelines, and asset terms.
- Apple Pay and Wallet marks require their specific official marketing or
  wallet guidelines in addition to the HIG technology page.
- Use Apple marks truthfully and only when the product actually supports the
  technology.
- Do not modify marks, make them more prominent than the app's own brand, use
  them as product identity, or imply partnership/endorsement.
- Apple trademark/legal pages are license and legal support only; they do not
  establish visual design patterns or replace HIG pages.

## Web And Non-Apple Products

- Translate HIG principles through system stacks, semantic color, accessibility,
  layout, and interaction behavior.
- Do not bundle Apple fonts, symbols, templates, logos, product art, or first
  party screenshots just to make a web app feel Apple-like.
- Label the result honestly as Apple-inspired or Apple-style when it is not a
  native Apple-platform product.

## Hard Blockers

- Apple font files are committed, bundled, or served without verified rights.
- SF Symbols are used as logos/app icons/trademarks or outside permitted scope.
- Apple logos, screenshots, wallpapers, app icons, product bezels, or marketing
  assets are copied without official permission.
- Third-party downloads are treated as official Apple resources.
- UI implies Apple affiliation, certification, approval, or App Store acceptance.

## Release Scan

Before publishing a repo that includes this skill or Apple-style work, scan for
unintended Apple-owned assets and secrets:

- Font files: `.ttf`, `.otf`, `.woff`, `.woff2`, `.dfont`.
- Images/assets: `.icns`, `.png`, `.jpg`, `.jpeg`, `.svg`, `.pdf`, `.sketch`,
  `.fig`, `.psd`, `.ai` that may contain Apple templates, bezels, marks, or UI.
- Text references to Apple Design Resources downloads, SF Symbols exports,
  Apple logos, product bezels, private symbols, screenshots, wallpapers, and
  license-restricted assets.
- API keys, account identifiers, real device/user data, or personal data in
  examples and screenshots.
