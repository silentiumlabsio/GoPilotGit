# Public Package Sanitization Report

This package was intentionally assembled as a public-safe GoPilot showcase repository.

## Excluded by design
- production Flutter source
- Android/iOS application source
- APK/AAB/IPA binaries
- signing keys and certificates
- service credentials
- API keys and tokens
- `.env` files
- private Firebase/Google Play configuration
- raw build logs
- local developer filesystem paths
- device serial numbers
- real user/trip/permit/customer data
- invoices and receipts
- private GitHub credentials

## Included
- public product documentation
- public-safe generated graphics
- issue/PR templates
- GitHub repository safety workflow
- public development/testing summary
- Codex agent rules
- optional static documentation page

## Safety controls
- `.gitignore` blocks common sensitive files and private app-source directories.
- `.github/workflows/public-repo-safety.yml` rejects common source/binary/credential mistakes.
- `AGENTS.md` instructs Codex/AI agents to preserve the public boundary.
- screenshot guidance requires redaction and approval.

## Media note
The graphics in this package were created specifically for this public repository and contain no real user or permit data.

Previously shared app screenshots are not silently copied into the package unless they are available as explicit, approved file inputs. Add only redacted screenshots to `assets/screenshots/approved/`.
