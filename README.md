https://github.com/Yanag1-san/tutorial-html-css-js-2sem-2025/releases

# Hands-On HTML, CSS & JavaScript Tutorial — 2nd Semester 2025 🚀

[![Releases - Download](https://img.shields.io/badge/Releases-Download-blue?logo=github&style=for-the-badge)](https://github.com/Yanag1-san/tutorial-html-css-js-2sem-2025/releases)

<img src="https://raw.githubusercontent.com/github/explore/main/topics/html/html.png" width="80" alt="HTML logo"> <img src="https://raw.githubusercontent.com/github/explore/main/topics/css/css.png" width="80" alt="CSS logo"> <img src="https://raw.githubusercontent.com/github/explore/main/topics/javascript/javascript.png" width="80" alt="JavaScript logo">

A concise, hands-on classroom tutorial for HTML, CSS, and JavaScript. This repo collects slides, example projects, exercises, and starter templates for the 2nd semester 2025 course. The material suits classroom use, lab work, and self-study.

Table of contents
- About
- Why this course
- What you will learn
- Audience
- Course structure
- Weekly syllabus
- Files and project layout
- Setup and run (Releases)
- Quick start examples
- Code snippets and common patterns
- Exercises and graded work
- Teaching notes and class flow
- Tools and tips
- Accessibility checklist
- Browser compatibility guide
- Best practices and patterns
- Additional resources
- How to contribute
- License
- Contact

About
This repository contains step-by-step class material for a full semester. It combines theory and practice. You will build real pages and small apps. The content breaks into short modules that you can run in class or at home. Each module has slides, a demo, a starter template, and exercises.

Why this course
Students must know how the web works. They must read and write HTML. They must style with CSS and add behavior with JavaScript. This course focuses on core skills. It uses live coding and small projects. The aim: give confidence to build accessible, responsive sites and simple interactive apps.

What you will learn
- HTML structure and semantic elements
- Forms and validation
- CSS layout: Flexbox and Grid
- Responsive design and media queries
- Modern CSS features: variables, custom properties, transitions
- JavaScript core: DOM, events, fetch, promises
- Module patterns and simple bundling
- Small project wiring: structure, assets, deployment
- Debugging with browser DevTools
- Accessibility basics and semantic markup

Audience
- Students in second-semester web development
- Beginner to intermediate developers who want a structured path
- Teachers who need a classroom plan and ready-to-run material

Course structure
The repo follows a modular structure. Each module includes:
- Slides (PDF or HTML)
- Demo app or example folder
- Starter template for exercises
- Exercise instructions with test criteria
- Reference cheatsheet

Weekly syllabus (14 weeks)
Week 1 — Intro to HTML and the web
- How the web works: client, server, HTTP
- Basic HTML: tags, attributes, structure
- Head vs body, meta tags, document outline

Week 2 — Text, links, images, lists, tables
- Semantic elements: header, main, nav, footer, article, section
- Image optimization and formats
- Accessible link text

Week 3 — Forms and input types
- Input types, labels, fieldsets
- Native validation and pattern attribute
- Form submission: GET vs POST

Week 4 — CSS fundamentals
- Selector types and specificity
- Box model, margin, padding, borders
- Display property and positioning

Week 5 — Layout with Flexbox
- Main properties: justify-content, align-items, flex-basis
- Common patterns: nav bars, card rows

Week 6 — Layout with Grid
- Grid container, grid-template, area naming
- Responsive grid patterns

Week 7 — Responsive design
- Media queries and breakpoints
- Fluid typography and responsive images

Week 8 — Advanced CSS
- Variables, custom properties
- Transitions and transforms
- Pseudo-classes and pseudo-elements

Week 9 — JavaScript fundamentals
- Types, variables, functions, control flow
- Arrays and objects
- Console and simple debugging

Week 10 — DOM and events
- Querying nodes, node vs element
- Event listeners, event delegation
- Creating and inserting elements

Week 11 — Asynchronous JavaScript
- Promises, async/await
- Fetch API and JSON handling
- Error handling patterns

Week 12 — Module patterns and simple build
- ES modules, import/export
- Small bundling with simple tools or no build
- Deploying a static site

Week 13 — Small projects (project week)
- Build a multi-page site or single-page app
- Focus on structure, performance, accessibility

Week 14 — Review and final demo
- Project demos and peer feedback
- Final polish and deploy

Files and project layout
This repo uses a clear folder layout:
- docs/        -> class slides and PDFs
- examples/    -> small demo projects per topic
- starters/    -> starter templates for exercises
- exercises/   -> exercise text and expected outputs
- assets/      -> images, icons, fonts, and shared assets
- tools/       -> utility scripts (lint, simple server)
- README.md    -> this file

Each module folder inside examples/ contains:
- index.html
- styles.css
- script.js
- README.md with exercise tasks

Setup and run (Releases)
This repo uses GitHub Releases to distribute compiled assets and packaged starter sets. Use the release page to get the latest package.

Download and run the release file:
1. Visit this releases page: https://github.com/Yanag1-san/tutorial-html-css-js-2sem-2025/releases
2. Download the release asset that matches your need (zip or tar.gz).
3. Extract the archive to a local folder.
4. Open the folder and run the included index.html files in your browser. For demos that require a server, run the provided start script or use a simple HTTP server:
   - Node: npx http-server ./folder -p 8080
   - Python 3: python -m http.server 8080
5. Use the browser to open http://localhost:8080 and test the demos.

Quick start (local)
1. Clone the repo
   git clone https://github.com/Yanag1-san/tutorial-html-css-js-2sem-2025.git
2. Open starters/basic-site/index.html in a browser
3. Start editing HTML and refresh the page
4. For live reload, run a small server tool listed in tools/

Quick start examples
Example: Simple responsive layout (starters/basic-site)
- Open index.html
- Observe the meta viewport tag:
  <meta name="viewport" content="width=device-width, initial-scale=1">
- Inspect layout in DevTools with device toolbar
- Try changing breakpoints in styles.css

Example: Fetch and render JSON (examples/fetch-demo)
- script.js:
  fetch('/data/users.json')
    .then(r => r.json())
    .then(data => renderUsers(data))
- renderUsers creates DOM nodes and inserts them into a list

Code snippets and common patterns
HTML semantic layout
- Use header, nav, main, footer
- Use section and article for content chunks
- Keep headings in order: h1 then h2

Basic reset
- Apply a minimal reset or normalize
  *, *::before, *::after { box-sizing: border-box; }
  html, body { margin: 0; padding: 0; }

Responsive image
  <img src="cover.jpg" alt="Cover image" width="1200" height="600" loading="lazy" />

CSS variables
  :root {
    --color-primary: #0b66c3;
    --gap: 16px;
  }
  .btn {
    background: var(--color-primary);
    padding: calc(var(--gap) / 2) var(--gap);
  }

Flexbox card row
  .cards {
    display: flex;
    gap: 16px;
    flex-wrap: wrap;
  }
  .card {
    flex: 1 1 220px;
    min-width: 220px;
  }

Grid layout example
  .grid {
    display: grid;
    gap: 16px;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  }

Event delegation pattern
  document.querySelector('.list').addEventListener('click', event => {
    const btn = event.target.closest('button');
    if (!btn) return;
    handleClick(btn.dataset.id);
  });

Fetch with async/await
  async function loadData(url) {
    const res = await fetch(url);
    if (!res.ok) throw new Error('Fetch failed');
    return res.json();
  }

Exercises and graded work
Each week includes exercises. A typical exercise follows this structure:
- Goal: short, clear objective
- Tasks: numbered steps to complete
- Requirements: accessibility and responsiveness criteria
- Deliverable: zipped folder or Git commit link
- Grading rubric: points for structure, CSS, JS, accessibility

Sample exercise (Week 3: Form)
Goal: Build an accessible contact form
Tasks:
1. Create a form with name, email, message
2. Add labels and fieldset
3. Use pattern attribute for email validation
4. Prevent default submission and show a confirmation using DOM
Requirements:
- All inputs have labels
- Tab order follows visual order
- Form shows inline error for invalid input
Deliverable: upload folder or push to repo under exercises/week-3/form

Teaching notes and class flow
- Start with short demo and live code
- Assign pair programming tasks
- Use short checkpoints after each feature
- Peer review: swap projects and run quick checklists

Sample class plan (50-minute)
0–5 min: Goals and agenda
5–15 min: Quick demo of new topic
15–30 min: Live coding with student questions
30–45 min: Student hands-on exercise
45–50 min: Review and assign homework

Tools and tips
Editors and extensions
- Use VS Code or similar
- Install HTML, CSS, JS lint extensions
- Use Live Server or similar for quick reload

Browser DevTools
- Use Elements panel to inspect DOM and styles
- Use Network panel to inspect resources and latency
- Use Console for logs and debugging
- Use Accessibility pane for basic checks

Version control
- Commit early and often
- Use small commits with clear messages
- Branch for major changes

Accessibility checklist
- Use semantic HTML
- Provide alt text for images
- Ensure keyboard navigation works
- Use color contrast ratio >= 4.5:1 for body text
- Use aria roles only when native HTML does not provide required semantics
- Add lang attribute to html element

Browser compatibility guide
- Test in Chromium, Firefox, and Safari
- Avoid APIs that lack wide support without polyfills
- Use feature detection, not userAgent sniffing
  if ('fetch' in window) { /* use fetch */ }

Best practices and patterns
Performance
- Minimize large images
- Use modern image formats (webp) when possible
- Defer non-critical JS with defer or module type

Structure
- Keep CSS modular by scope or naming
- Prefer small utility classes for common layout needs
- Keep JS behavior separate from markup where possible

Security basics
- Escape untrusted data before inserting into innerHTML
- Use textContent for plain text insertion
- Avoid eval and similar patterns

Common mistakes
- Overuse of divs instead of semantic elements
- Forgetting to include viewport meta tag
- Inline styles with no responsive plan

Project ideas (small to medium)
- Portfolio site with contact form and gallery
- To-do list with localStorage
- Weather app using public API and fetch
- Simple quiz app with timed questions
- Photo gallery with lightbox and keyboard controls
- Multi-page site with navigation and active state

Real project flow (example: Portfolio)
1. Plan content and sections
2. Create semantic HTML skeleton
3. Build responsive layout with Grid for main sections
4. Add nav with anchor links and active state
5. Add contact form with client-side validation
6. Optimize images and assets
7. Test across devices and browsers
8. Deploy to static host

Deployment
- Host on GitHub Pages for static sites
- Use simple CI to build and push
- Set correct base path if project uses subfolder

Testing and validation
- Use HTML validators and CSS linters
- Use Lighthouse for performance and accessibility checks
- Manual test keyboard navigation and screen reader where possible

Reference cheatsheets (inside repo)
- HTML tag reference
- CSS properties quick guide
- JavaScript DOM methods table
- Common accessibility attributes

Slides and teaching assets
Slides live in docs/ as PDF and HTML. Use them as class prompts and for quick review. Slides include code examples and live demo links inside examples/.

Images and icons
Use existing web-safe SVG icons and GitHub Explore topic images. Store local copies in assets/ so demos work offline.

Releases and packaged starters
Visit the release page to download ready-to-run bundles. Each release includes a zip with current slides, starters, and example apps. The release asset must be downloaded and executed locally to run the demos. See the releases page to pick the right asset. https://github.com/Yanag1-san/tutorial-html-css-js-2sem-2025/releases

How to contribute
- Open an issue for bugs or content requests
- Fork the repo and make a branch for changes
- Keep commits small and descriptive
- Add tests or examples for code changes
- Send a pull request with clear description and linked issue

Contribution workflow
1. Fork the repo
2. Create a branch: feature/lesson-10
3. Make changes and run local checks
4. Open PR with summary and files changed
5. Wait for review and respond to comments

Standards for contributions
- Use clear language in slides and README
- Keep code simple and well commented
- Provide runnable examples
- Add tests or steps to reproduce issues

License
This project uses the MIT License. See LICENSE for details.

Contact
- Issues and PRs via the GitHub repo
- For class scheduling or reuse, open an issue and label it "class-request"

Appendix A — Example exercises (expanded)
Exercise: Build a responsive card grid
Goal: Create a grid of cards that adapts to screen size
Steps:
1. Create a grid container with CSS Grid
2. Use repeat(auto-fit, minmax(220px, 1fr)) for responsive columns
3. Each card must include an image, title, and description
4. Add a hover state that raises the card and shows a subtle shadow
Requirements:
- Use semantic HTML for content
- Images must have alt attributes
- Cards must be keyboard accessible (tab focus)

Exercise: Fetch and render API data
Goal: Use fetch to load data and render it
Steps:
1. Use fetch to call a public JSON endpoint or local JSON file
2. Map the data to DOM nodes
3. Add loading and error states
4. Cache results in localStorage to reduce requests
Requirements:
- Use async/await
- Show a spinner while loading
- Handle network errors with a user message

Appendix B — Teaching tips by topic
HTML
- Emphasize document outline and heading order
- Teach forms early; they link to real tasks

CSS
- Start with layout basics, then move to Flexbox and Grid
- Use visual demos that compare methods

JavaScript
- Start with console, variables, and functions
- Move to DOM and events with small demos
- Show network calls and parsing JSON late in sequence

Appendix C — Common commands
Start a simple server (Node)
npx http-server ./examples/basic -p 8080

Start a simple server (Python)
python -m http.server 8080

Run linter (example)
npm run lint

Appendix D — Useful links and resources
- MDN Web Docs: https://developer.mozilla.org
- CSS-Tricks guides: https://css-tricks.com
- Can I use: https://caniuse.com
- WebAIM color contrast checker: https://webaim.org/resources/contrastchecker/

End of README content.