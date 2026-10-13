# Changelog

Changes to the Hackwarts landing page, recorded from the project prompts.

## 2026-10-12

### Landing page

- Created a single-page Hackwarts landing page with the supplied full-screen background video and centered wizarding emblem.
- Matched the supplied visual reference with a dark cinematic scene, gold accents, and a top navigation bar.

### Typography and cursor

- Applied the provided Harry P font site-wide, with Pirata One retained as a fallback.
- Increased navigation link and registration-button text sizes while keeping the mobile header within narrow screens.
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

## 2026-10-13

### Full Theme and PDF Content Integration

- Implemented the complete dark mystical theme matching the visual design reference, with glowing golden section numbers (`01`, `02`, `03`, `04`, `05`, `06`, `07`) and calligraphy flourish underlines.
- Extracted and integrated all content from the Hackwarts 3-page PDF document: Black Rabbit community profile, 24-hour offline hackathon scope, motto "Where Code Becomes Magic", Vision & Objectives, Impact, Schedule, 5 Tracks, Submission Guidelines, and Leadership Contacts.
- Created and styled the exact ornate golden filigree boxes from Section 02, complete with corner brackets, accent studs, glowing golden headers, and translucent dark glassmorphism.
- Added Section 01 featuring Black Rabbit's origins and a floating 3D Sorting Hat with levitation animation and ambient glowing particles.
- Added Section 02 featuring the offset "Goal / Vision & Objectives" box, the snowy owl flying with the sealed Hogwarts acceptance letter, and "The Three Wizarding Stages" (Dementor's Trial, Wizarding Build, Triwizard Finale).
- Added Section 03 featuring the Four Houses of Hackwarts (Slytherin, Gryffindor, Ravenclaw, Hufflepuff) with interactive tab switching, high-resolution house crests, house traits, notable wizards, and 4-column overview grid.
- Added Section 04 detailing the five technical tracks: Charms & Artificial Intelligence, Defense Against the Dark Arts, Potions & Data Science, Magical Engineering, and Department of Mysteries.
- Added Section 05 detailing the complete 24-hour timeline from 10:00 AM Day 1 to 10:00 AM Day 2 with interactive timeline scroll.
- Added Section 06 featuring official submission guidelines (Git repo, README, working demo, project summary), evaluation rubrics, and expandable accordion FAQs.
- Added Section 07 featuring Black Rabbit leadership contacts (Vedant Sakpal, Sumit Kumar) with direct call links, and an interactive team registration form with house and track selection.
- Connected smooth-scrolling navigation with scroll spy that dynamically highlights the active navbar item as the user explores the castle.
- Restored the exact hero scene layout: the centered golden Hackwarts emblem (`.identity`) floats majestically above the wizard and castle backdrop video without buttons or textual overlays, perfectly matching the original cinematic framing while keeping all full-length sections below.

### House Roster Alignment (Three Houses)

- Removed the Hufflepuff clan across the entire site, aligning with Page 2 of the official Hackwarts PDF ("Three houses: Gryffindor, Slytherin & Ravenclaw").
- Updated Section 03 to "The Three Houses of Hackwarts", removing the Hufflepuff tab selector button and house showcase card.
- Adjusted the house showcase grid to a balanced 3-column layout (`repeat(3, 1fr)`) with responsive wrapping on mobile.
- Updated the registration form dropdown, FAQ house sorting description, and JavaScript `houseData` state dictionary to reflect the 3 houses.

### Typography Refinement for Readability

- Replaced the pervasive movie-logo font across general content with a regal, highly readable classical wizarding system:
  - **Headings & Display (`--font-heading`, `--font-display`)**: Set to `Cinzel` (with `Cinzel Decorative` and `Georgia` fallbacks) for authentic, noble, gold-inscribed fantasy headers that are crisp and legible.
  - **Body & Paragraphs (`--font-body`)**: Set to `EB Garamond` at `18px` with `line-height: 1.7` for rich, spellbook-like readability across all descriptions, vision boxes, stages, and FAQ answers.
  - **UI, Navigation & Forms (`--font-ui`)**: Set to `Outfit` and `Cinzel` uppercase for navigation links, registration buttons, track tags, timestamps, wizard pills, and input controls.
- Reduced cartoonish movie-logo stylization while preserving the immersive dark magical atmosphere.
