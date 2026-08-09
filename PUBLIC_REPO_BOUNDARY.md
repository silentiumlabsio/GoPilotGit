# Public Repository Boundary

This repository is intentionally **not** the GoPilot application source repository.

## Allowed

Public-safe material may include:
- product overview documentation
- feature descriptions
- approved/redacted screenshots
- public release notes
- public roadmap items
- non-sensitive testing summaries
- public marketing graphics
- GitHub issue templates
- documentation-site files

## Never commit

Do not commit any of the following:

### Application source
- Flutter `lib/`
- Android `android/`
- iOS `ios/`
- platform source directories
- internal build scripts that reveal app implementation
- private tests that expose implementation details

### Build and signing material
- `.apk`
- `.aab`
- `.ipa`
- `.jks`
- `.keystore`
- `.p12`
- certificates or provisioning profiles
- signing passwords
- signing properties

### Service and API configuration
- `.env` files
- API keys
- OAuth secrets
- access tokens
- refresh tokens
- service-account JSON
- `google-services.json`
- `GoogleService-Info.plist`
- private endpoints or credentials
- billing credentials
- private Firebase configuration

### User / business data
- permit documents
- permit numbers tied to real customers
- VINs when sensitive
- customer names or phone numbers
- addresses
- invoices
- payment information
- receipts containing personal data
- real trip records
- location history
- crash logs containing PII

### Internal development evidence
- raw terminal logs
- local filesystem paths
- device serial numbers
- developer usernames
- private build hashes unless intentionally published
- private GitHub tokens
- Play Console credentials
- private email addresses

If there is any doubt, do not commit the file.
