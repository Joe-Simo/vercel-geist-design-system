## Privacy And Data Use Gate

Use this when UI or implementation touches permissions, accounts,
authentication, payments, tracking, analytics, personal data, health, location,
camera, microphone, photos, contacts, Bluetooth, local network, files, user
screenshots, or App Store-facing work. Official Apple privacy pages and
developer agreements remain the source of truth.

Use exact official pages from `official-reference-map.md` when applicable:
Privacy, App privacy details, User privacy and data use, Privacy manifest
files, AppTrackingTransparency, App Review Guidelines, and technology-specific
pages for Sign in with Apple, Apple Pay, Wallet, HealthKit, HomeKit, iCloud,
In-App Purchase, Maps, NFC, Siri, VoiceOver, and related capabilities.

## Required Data Inventory

Record:

`data/capability | purpose | official Apple URL | collection/access point | user control | disclosure/copy | storage/sharing | verification`

The UI must explain why access is needed before asking, request only when the
feature needs it, and provide recovery if access is denied.

## Permission And Protected Resource Rules

- Ask for protected access in context, not at launch unless launch truly needs
  it.
- Make the benefit clear in product language before the system prompt appears.
- Handle denied, limited, unavailable, and revoked permissions.
- Do not block unrelated app features behind unnecessary permissions.
- Do not place real personal data in screenshots, examples, seed data, fixtures,
  docs, public repos, or final reports.

## Tracking, Third Parties, And App Store Context

- For tracking/advertising identifiers, third-party SDK data, cross-app/site
  tracking, or App Store distribution, verify current official Apple privacy,
  App Review, App Store Connect, AppTrackingTransparency, and privacy manifest
  guidance before claims.
- When applicable, check privacy nutrition labels, privacy policy, purpose
  strings, `PrivacyInfo.xcprivacy`, third-party SDK responsibility, and App
  Tracking Transparency requirements.
- Do not imply privacy compliance from UI polish alone.

## Privacy UI Requirements

- Privacy prompts, settings, empty states, permission recovery, and account
  flows need clear writing and visible choices.
- Sensitive actions need confirmation, reversible states where possible, and
  plain-language consequences.
- Use Sign in with Apple, Apple Pay, Wallet, Health, or other Apple technology
  marks only when the product truly implements the technology and official
  guidelines/assets permit the exact usage.

## Claim Blockers

- Missing data inventory for a touched protected capability.
- Permission requested without clear purpose or recovery.
- UI screenshots or examples expose personal data.
- App Store/privacy claims made without current official Apple source rows.
- Third-party SDK or analytics behavior hidden from the design/review scope.
