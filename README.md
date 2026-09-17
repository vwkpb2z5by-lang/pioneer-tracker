# Pioneer Tracker V2.1 Foundation

This version deliberately returns to the simple V2 foundation and incorporates the annotated iPhone feedback.

## Core changes
- Removed the wife-specific message from Settings.
- Home pace status now uses the current date and month-to-date target:
  - Ahead of Pace
  - On Pace
  - Behind Pace
  - Goal Reached
- Home explains why the pace status is shown.
- Removed the redundant Home-page “Log Service” button; Add remains a dedicated bottom tab.
- Add now uses a full Monday–Sunday month calendar inspired by the provided Field Service Activity example.
- Calendar dots show dates that already contain service or extra-credit entries.
- Selected date is centered and displayed as a full readable date.
- Existing entries for the selected date are shown before the entry form.
- Extra Credit has its own Add mode, a 30-hour monthly maximum, and a reason/notes field.
- Six-Month Test has been simplified into:
  - Month X of N
  - Current monthly goal
  - Total during test
  - Average per month
  - Months remaining
- App is generic enough for any publisher/pioneer/service-hours goal:
  - Name
  - Congregation/group
  - Service role/goal label
  - Custom base monthly goal
  - Goal percentage
- Seven layout color themes.
- Weekly Plan tab remains simple and uses Monday–Sunday targets from Settings.
- History supports filtering, editing, and deleting both service and extra-credit entries.
- JSON backup/import.
- Migrates existing data from the original V2 app and the stripped-down V2 Foundation when possible.

## Stability decision
There is intentionally NO service worker in this version.
Recent versions had stale-cache/loading issues. V2.1 unregisters old service workers and focuses on reliable browser storage and GitHub Pages delivery.

## GitHub Pages update
Replace the contents of your current repository with:
- index.html
- manifest.json
- icons/

Do not upload an old sw.js/service-worker file. Delete it from the repository if it is still there.

After GitHub Pages deploys, open the site in Safari once before using the Home Screen icon. The header should display “V2.1 Foundation”.
