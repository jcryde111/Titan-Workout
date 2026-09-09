# Titan Workout PWA V6.6

Hotfix release restoring startup initialization, program/workout selectors, and IndexedDB history loading. Existing TitanWorkoutV5 IndexedDB data is preserved.

# Titan Workout PWA V6.5

V6.5 corrects the training-page movement preview system.

## V6.5 movement preview changes
- Replaces the generic muscle-group animation with exercise-specific movement-path schematics.
- Distinguishes presses, rows, pulldowns, flyes, curls, triceps extensions, squats, hinges, leg presses, leg curls/extensions, hip thrusts, calf raises and major core movements.
- Shortcut to Size abdominal hip-thrust variations are explicitly treated as abdominal movements rather than the glute hip thrust used in Lean Mass Builder.
- If Titan cannot identify a reliable movement pattern, it shows no fake animation and directs the user to the exact form notes/video search.

# Titan Workout PWA V6.3

Major training-experience update.

## V6.3
- Workout-session notes with local autosave.
- Dashboard 30-day and current-month counters now count completed workouts only.
- Workout duration is derived from actual set timestamps, preventing stale/open sessions from reporting multi-day durations.
- Lightweight animated movement cues are shown on the main training page without downloading third-party GIF files.
- Short-form exercise video search links and expanded form information.
- Removed exercise Move Up / Move Down controls.
- Substitution browser filters alternatives by the same muscle focus and by Gym / Hotel / Bodyweight.
- Substitutions can be temporary for the current workout or saved as the program default.
- Previous completed workout set values appear greyed beside the current weight/reps fields.
- Exercise Library is organized by muscle focus and includes expanded location-aware alternatives.
- Program Library / selector added. Lean Mass Builder contains the current four workouts.
- Shortcut to Size program shell is selectable, but detailed copyrighted/source exercise pages were not reconstructed from web material. Re-add the original source/screenshots to populate it accurately.
- Backup version 8 stores programs, notes, sessions and overrides.

## Storage
Titan continues to use the existing `TitanWorkoutV5` IndexedDB database so prior logged sets and sessions remain available after upgrading.


## V6.4 Shortcut to Size
- Populates the full 12-week Shortcut to Size training schedule from the user-provided program PDF.
- Includes all three phases and four weekly microcycles.
- Workout selector is grouped by week.
- Weeks 1-2 are marked rest-pause on the last set; weeks 3-4 are marked drop-set on the last set.
- Previous-workout values carry across Shortcut to Size weeks for the same workout slot.
- Adds all Shortcut to Size exercises to the exercise library and substitution system.
- Existing V6.3 users automatically replace the empty Shortcut to Size shell with the populated program without overwriting Lean Mass Builder.


## V6.7 dashboard/navigation hotfix
- Bottom navigation now highlights only the page currently being viewed.
- Dashboard Last 30 Days and This Month counters use the completed-session timestamp rather than the date an old/in-progress session was first opened.
- Completed history and calendar use the same completion-date logic so dashboard dates stay consistent.
- Existing IndexedDB data is preserved.


## V6.8 training render hotfix
- Restored the missing workout render function that was accidentally dropped from V6.5-V6.7.
- Program and workout selectors now render the selected workout exercises again.
- Set inputs, previous-set references, exercise info, rest timers, substitutions, and autosave event handlers are reattached whenever a workout is opened.
- Uses the same IndexedDB database and does not clear existing workout history.
