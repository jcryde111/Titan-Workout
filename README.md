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
