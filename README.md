# Gym Trainer PWA

Netlify-ready pure front-end workout tracker PWA.

## Version
3.2

## Bulk Exercise Images
The app automatically checks `assets/exercises/<exercise-slug>.webp` for every exercise. Existing hyphens are preserved as single hyphens. You can still use `exercise-images.js` for custom overrides.

## Notes
All data is stored locally in the browser. Use Settings > Export Data regularly for backup.


### Patch Notes

- Exercise Database no longer displays automatic image fallback filename text in list cards or edit mode.
- Existing exercise editor X button now prompts to delete the exercise using the app confirmation dialog.
- Exercise image action buttons in edit mode are smaller and fit on one line.
- Editing an exercise opens the editor inline near the selected exercise and scrolls the editor into view.
- Today workout cards now show live up/down kg indicators when the current highest set weight differs from the most recent previous completed workout for the same exercise.


#### v2.3 Dashboard Update
- Rebuilt Home dashboard with Today hero card, Last 30 Days training/rest card, Personal Best card, Training Balance stacked bar, Quick Actions, and Weight Trend.
- Added target-area hero images under assets/targets for all default target areas.
- Quick Actions now navigate to Today, Settings body weight input, and Log.


##### v2.4 Clean Dashboard Styling Update
- Replaced emoji-style dashboard and bottom navigation icons with minimalist monochrome SVG stroke icons.
- Refined Home dashboard card styling, typography, spacing, shadows, and icon badges to match a cleaner modern mobile UI style.
- Preserved all v2.3 app functionality and data logic.
- Kept assets/targets/ folder empty for user-supplied target-area images.


##### v2.4 Refinement Update
- Home Last 30 Days and Personal Best cards now use a plain white background to match the Training Balance card.
- Today tab target area selector now includes a small chevron dropdown icon to indicate it is clickable.
- assets/targets/ remains empty for user-supplied target images.


###### v3.1 Equipment Field Update
- Added optional Equipment dropdown to Exercise Database with Dumbbell, Barbell, Smith Machine, Cable Machine and Weight Machine options.
- Equipment can be left blank and only one equipment option can be selected per exercise.
- Displayed selected equipment on Today and Log exercise cards using the Exercise Database lookup.


####### v3.2 Rename Sync, Daily Weight and Collapsible Today Cards
- Exercise Database renames now update linked Today and historical Log records through exerciseId.
- Log view mode now resolves Equipment from the Exercise Database.
- Added optional daily body weight display/editing in Log, synchronized with Settings Weight History and Home Weight Trend.
- Added session-persistent collapsible Today Exercise Cards with a minimal chevron header control.


####### v3.4 Advanced Mode and Version Placement
- Moved the app version from the header to a standalone themed text label at the bottom of Settings.
- Added a persistent Advanced Mode toggle to the Today header; the setting defaults to OFF.
- When Advanced Mode is ON, newly added exercises copy the exact previous completed sets and weights by unique exerciseId.
- Cardio exercises copy the previous duration and distance; exercises without history retain normal empty/default values.
- Copy last behavior remains unchanged.
