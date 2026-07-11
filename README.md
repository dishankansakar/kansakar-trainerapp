# Gym Trainer PWA

Netlify-ready pure front-end workout tracker PWA.

## Version
2.7

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


###### v2.5 Interaction, Icon and Image Handling Update
- Added tap-and-hold reordering for Today workout exercise cards, with order saved immediately.
- Replaced destructive remove/delete X buttons with minimalist SVG bin icons, while keeping delete-set and close/cancel X controls unchanged.
- Improved exercise image selection by resizing/compressing uploaded images before saving, with friendly errors for unsupported or oversized images.
- Shortened Exercise Database image editor buttons to Add, Replace, and Remove with smaller mobile-friendly styling.
- Included target-area image assets under assets/targets/ for the Home dashboard hero image.

###### v2.6 Reorder, Edit Icon and Home Plan Logic Update
- Fixed Today tab tap-and-hold reordering so active dragging locks manual page scrolling and supports controlled edge auto-scroll.
- Replaced app-wide Edit text buttons with a transparent minimal SVG edit icon, while keeping Done as text.
- Updated the Home Today card to use the workout logged on the same weekday last week for display-only target and exercise count logic.
- Updated the Home Today card to show Rest Day with 0 Exercises when last week's matching weekday has no logged workout.
- Removed the Today card calendar icon column and redundant Last 30 Days trained/rest summary text.

###### v2.7 Home, Rest Day and Settings Refinement Update
- Added a Rest Day image asset and displays it on the Home Today card using the same blue gradient card style as target-area days.
- Replaced the edit icon with a thinner modern SVG edit icon.
- Removed the Custom Target Areas explanatory footer and removed the Includes label from custom target summaries.
- Simplified the Home greeting spacing and typography, and removed the motivational subtitle.
- Updated Personal Best to follow the Home Today card target logic, showing Rest Day when the Today card displays Rest Day.
- Removed the Home Quick Actions card.
