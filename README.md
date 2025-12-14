# ChildrenActivity

A warm, practical collection of simple, adaptable learning activities and evaluation tools designed for students with Trisomy 21 (Down syndrome). This repository helps teachers prepare short, predictable, and scaffolded exercises so they can assess progress with clarity and confidence.

The tone of the materials is plain, positive, and classroom-friendly — easy to adapt for individual needs.

## Who this is for
- Primary: special-education teachers working with students with Trisomy 21.  
- Secondary: parents, therapists, and classroom assistants who implement or adapt activities.

## Project goals
- Offer short, structured activities tailored to the cognitive and sensory needs of students with Trisomy 21.
- Make content easy to customize (visuals, pacing, difficulty).
- Provide clear rubrics and simple recording templates so teachers can track small, measurable steps of progress.

## Key features
- Reusable activity templates: matching, sequencing, sorting, single-step reading tasks.
- Simple evaluation rubrics and progress notes suitable for IEPs.
- Multimedia-friendly activities (images, pictograms, audio cues).
- Accessibility-first choices (large text, high-contrast colors, clear layouts).
- Exportable reports: CSV-friendly data to include in student records.

## Technology
This is an Angular application (no Python). The UI and activity engine are built with Angular and standard web assets.

## Quick start (Angular)
1. Prerequisites
   - Node.js (recommended >= 16)
   - npm (comes with Node) or yarn
   - Angular CLI (optional but helpful): npm install -g @angular/cli

2. Clone the repo
   git clone https://github.com/abderrazekbhr/ChildrenActivity.git
   cd ChildrenActivity

3. Install dependencies
   npm install
   (or `yarn` if you prefer)

4. Run the development server
   - If the project has a start script in package.json:
     npm start
   - Or run with Angular CLI:
     ng serve --open
   Default dev server port: 4200.  
   To run on a different port:
     ng serve --port 4300 --open
   Or with npm:
     npm run start -- --port 4300

5. Build for production
   npm run build
   The production build will appear in the `dist/` folder (standard Angular output).

Note: If your project uses a specific npm script or proxy configuration, update these commands to match the repository package.json.

## Project layout (example)
- src/ — Angular source code
- src/app/activities/ — activity components and templates
- assets/ — images, pictograms, audio cues
- docs/ — teacher guides, screenshots, example rubrics
- data/ or activities/ — JSON activity definitions and rubrics

Adjust these paths if your project structure differs.

## Activity format (how to add / adapt)
Each activity should be short and focused. A suggested minimal activity structure:
- metadata.json — id, title, learning goal, recommended duration
- content.json — prompts, choices, correct answers, media references
- rubric.md — evaluation checklist (step-by-step observable behaviors)

To create a new activity:
1. Duplicate a template from src/app/activities/templates/
2. Edit metadata, content and rubric
3. Test locally with the dev server and adjust visuals/pacing

## Teaching guidance (practical tips)
- Short sessions (5–15 minutes) work best; repeat routines across days.
- Use consistent visual cues (same icons/colors for types of actions).
- Praise small, concrete behaviors and record them in the rubric immediately.
- Reduce distractions: single task per screen; large, clear buttons.

## Accessibility & privacy
- Prefer large fonts, high-contrast UI, and simple language.
- Use alt-text for images and captions for audio where possible.
- When recording student data, follow local policies and anonymize identifiers if sharing outside the school.

## Contributing
Contributions from teachers, therapists, and developers are welcome.
- Add or improve activities and rubrics
- Improve accessibility (contrast, text size, keyboard navigation)
- Add translations or multimedia assets
Open an issue to discuss larger changes, or submit a pull request with a short description of the pedagogical goal.

## License
Choose a license that fits your goals (MIT, CC BY-SA, etc.). If you’d like, I can add a recommended license for educational resources.

## Contact / Credits
Maintained by: @abderrazekbhr  
Thanks to teachers, therapists, and families who test and adapt these activities.

---

If this draft looks good I can:
- (A) create a new branch and open a pull request with this README, or
- (B) directly update README.md on main.

Tell me which option you prefer and I will apply the change. If you want more edits (shorter text, French/Arabic translation, or different folder names), tell me the specifics and I’ll incorporate them before committing.
