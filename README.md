# Gym Trainer PWA

Netlify-ready pure front-end workout tracker PWA.

## Version
2.8

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


###### v2.8 Hero Logic, Home Title, Exercise Database and Custom Target Update
- Updated the Hero Card to use the current Today tab plan when Today has any exercises, including complete or incomplete exercises.
- Kept same-weekday-last-week fallback only when Today has no exercises listed.
- Updated Hero Card exercise count to use all Today Exercise Cards when using the Today plan source.
- Matched Last 30 Days, Personal Best and Training Balance card titles to the Weight Trend gradient title style.
- Made Exercise Database rows more compact and aligned exercise-name font sizing with the Exercise Database heading.
- Updated Custom Target Areas so delete is only available inside edit mode, with the edit icon in the normal row action position.
