# Titan Workout PWA V6.2

Device-only hypertrophy workout app for Android, iPhone and desktop.

## What is included
- Device-only IndexedDB autosave
- Unique workout sessions
- Dashboard, calendar, history and PRs
- Exercise details and hypertrophy cues
- Curated embedded videos where a verified match was available
- Targeted YouTube fallback for less-common variations
- Offline workout logging (videos require internet)
- Backup export/import

## Run locally on Windows
1. Extract the ZIP.
2. Open Terminal in the folder.
3. Run `npx serve .`
4. Open the displayed local address.

For installation on a phone, deploy the folder to an HTTPS web host.


## V6.1 testing features
- Duplicate and customize workouts.
- Substitute and reorder exercises.
- Edit sets, rep targets, and rest periods.
- Restore original workouts.
- Custom programs are device-only and included in backups.


## V6.2 persistence fix
- Restored missing autosave queue and pending-save flush functions.
- Entries now save after typing, on change/blur, and before workout completion.
- Service-worker cache bumped so deployed devices receive the repaired build.
