# Changelog

Changes to the Hackwarts landing page, recorded from the project prompts.

## 2026-10-12

### Landing page

- Created a single-page Hackwarts landing page with the supplied full-screen background video and centered wizarding emblem.
- Matched the supplied visual reference with a dark cinematic scene, gold accents, and a top navigation bar.

### Typography and cursor

- Applied Pirata One as the page-wide typeface.
- Replaced the initial cursor with a custom wooden wand featuring carved details, a diagonal tilt, and a magical glow.
- Tilted the wand cursor to 45 degrees and added two revolving, glowing magical points for fine-pointer devices; touch and reduced-motion users retain a static cursor.

### Navigation

- Increased the navbar size, then redesigned it to include the Hackwarts emblem, Home, About, Houses, Tracks, Schedule, FAQs, Contact, and a Register Now action.
- Added responsive navigation layout for mobile screens, including a horizontally scrollable link row.
- Replaced the navbar's standalone crest and text with the supplied Golden Hackwarts Wizarding Emblem image.

### Audio and loading

- Added the supplied background song with a play/pause control.
- Added a magical loading screen that waits for the logo and video metadata, with a timeout so loading cannot block the page indefinitely.
- Replaced the static loading panel with `Video Project 8.mp4`, playing from 00:09 through 00:17 before the overlay slides up.
- Temporarily disabled the intro video with a feature flag; it stays unloaded and can be turned back on by setting `enableIntroVideo` to `true`.

### Wand cursor motion

- Tilted the wand cursor to 45 degrees.
- Added two subtle glowing points that continuously orbit the wand on fine-pointer devices, while respecting reduced-motion preferences and leaving touch cursors unchanged.

Future project prompts that change the page should be added here as new entries.
