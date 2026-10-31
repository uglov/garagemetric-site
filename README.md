# GarageMetric Site

Public support site for GarageMetric.

## Pages

English:
- Home: `/`
- Privacy Policy: `/privacy/`
- Account deletion: `/delete-account/`

Ukrainian:
- Home: `/uk/`
- Privacy Policy: `/uk/privacy/`
- Account deletion: `/uk/delete-account/`

Every public page exposes an EN / UA language switch while keeping the English
URLs stable for Google Play and other store metadata.

The account-deletion page uses direct HTTPS `fetch` calls to Supabase Auth and
the production `delete-account` Edge Function. It has no third-party runtime
JavaScript dependency. The Supabase publishable key is intentionally public
client configuration; no service-role key or server secret is stored in this
repository.

## GitHub Pages

In repository settings:

1. Open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select **main** and **/(root)**.
4. Save.

Expected project-site URL:

`https://uglov.github.io/garagemetric-site/`
