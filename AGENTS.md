# Codex / AI Agent Rules for GoPilotGit

This file is authoritative for AI agents working in this repository.

## Repository purpose

`GoPilotGit` is a **public product showcase and documentation repository**.

It is not the production app source repository.

## Hard security rules

NEVER add or request:
- Flutter app source (`lib/`)
- Android app source (`android/`)
- iOS app source (`ios/`)
- APK/AAB/IPA binaries
- keystores, certificates, signing files
- API keys, OAuth secrets, tokens
- service account files
- `.env` files
- `google-services.json`
- `GoogleService-Info.plist`
- private Firebase/Google Play configuration
- private endpoints
- local developer filesystem paths
- device serials
- raw internal terminal logs
- permit/customer/user PII
- real invoices, receipts, or trip records

Do not weaken `.gitignore` or the public-repository safety workflow.

## Content rules

- Do not invent app features.
- Distinguish released features from development/roadmap items.
- Do not publish a hard-coded subscription price unless the user explicitly provides a current public price for the repository.
- Do not claim iOS is released; currently describe it as in progress.
- Keep the core disclaimer visible: extracted/organized permit information must be compared with the official permit and current requirements.
- Keep the audience broad: truckers, hotshots, owner-operators, small fleets, and pilot/escort workflows.
- Do not describe GoPilot as only a pilot-car app.

## Screenshot rules

Only use images in `assets/screenshots/approved/`.

Before adding a screenshot:
1. inspect it visually
2. remove personal data
3. remove permit/customer identifiers
4. remove payment/account information
5. remove internal/debug information
6. ensure no API key/token is visible
7. keep the image only if it is clearly safe for a public repository

## GitHub quality goals

Maintain:
- polished README
- accessible image alt text
- clear documentation structure
- useful issue templates
- working internal links
- public-repo safety checks
- no broken badges or invented URLs
- no app source or secrets

## Pull requests

Before opening a PR:
- run the repository safety workflow locally where practical
- inspect the diff for sensitive information
- confirm no forbidden files were added
- summarize public-facing changes only
