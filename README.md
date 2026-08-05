# Get Expansively public site

A lightweight, framework-free public website for `getexpansively.com` with:

- Homepage
- Privacy Policy
- Terms of Service
- Community Guidelines
- Support page
- Privacy Choices page
- Account Deletion instructions

The site is plain HTML/CSS/JavaScript and ships with an Nginx Docker image for Coolify.

## Local preview

From this folder:

```bash
python3 -m http.server 8080
```

Open `http://localhost:8080`.

## Deploy with Coolify

1. Push this repository to GitHub, GitLab, or another Git provider.
2. In Coolify, create a new resource from the repository.
3. Select **Dockerfile** as the build type.
4. Assign these domains to this resource:
   - `https://getexpansively.com`
   - `https://www.getexpansively.com`
5. Keep the application and API on their existing resources:
   - `https://app.getexpansively.com`
   - `https://api.getexpansively.com`
6. Remove the Squarespace forwarding rule that redirects the root domain to `app.getexpansively.com`.
7. Point the root and `www` DNS records to the server/proxy used by this Coolify resource.

## App Store URLs

- Marketing URL: `https://getexpansively.com/`
- Privacy Policy URL: `https://getexpansively.com/privacy/`
- Support URL: `https://getexpansively.com/support/`
- Privacy Choices URL: `https://getexpansively.com/privacy-choices/`
- Account deletion information: `https://getexpansively.com/account-deletion/`

## Before publishing

Review every statement against the app's actual behavior, especially:

- Data types collected and transmitted
- Third-party SDKs and service providers
- Location collection
- Private messaging
- Retention and deletion behavior
- Payments, advertising, and analytics if added later
- Minimum age and geographic availability
- Business name, address, and governing-law language

The legal pages are practical drafts, not legal advice. Have qualified counsel review them before broad launch.

## Official Apple references used while preparing the checklist

- App Review Guidelines: https://developer.apple.com/app-store/review/guidelines/
- App privacy in App Store Connect: https://developer.apple.com/help/app-store-connect/manage-app-information/manage-app-privacy/
- Account deletion guidance: https://developer.apple.com/support/offering-account-deletion-in-your-app/
