# AGENTS.md

# F1 Insider — Project Development Guidelines

## 1. Project Overview

F1 Insider is a Formula 1 knowledge website designed for beginners and motorsport fans.

The website provides organized information about Formula 1 drivers, teams, circuits, and racing knowledge.

### Project Goals
- Introduce Formula 1 to beginners.
- Provide clear and accessible motorsport information.
- Organize F1 knowledge into different categories.
- Maintain a consistent design and structure across all pages.
- Allow new content and pages to be added easily.

### Target Audience
- People who are new to Formula 1.
- Formula 1 fans who want to learn more about drivers and teams.
- Readers interested in racing circuits and race strategies.

### Language
- Traditional Chinese (繁體中文) is the primary language.
- English names and official F1 terminology should be preserved when appropriate.

---

## 2. Technology Stack

Use the following technologies:

- HTML5: Website structure and content.
- CSS3: Layout, styling, responsive design, and animations.
- Vanilla JavaScript: Interactive elements and navigation.

### Development Restrictions
- Do not use React, Vue, or other JavaScript frameworks.
- Do not require a backend or database.
- Keep the website compatible with GitHub Pages.
- Prefer simple, readable, and maintainable code.

---

## 3. Design Guidelines

### Visual Identity

The website should follow a modern Formula 1 editorial and motorsport magazine style.

The overall appearance should be professional, bold, dynamic, and easy to navigate.

### Color Palette

- Primary Background: #111111
- Secondary Background: #1C1C1C
- Brand Red: #D71920
- Primary Text: #F5F5F5
- Secondary Text: #999999
- Border: #333333

### Typography
- Use bold and large headings for important titles.
- Use clean and readable fonts for body text.
- English titles can use uppercase lettering.
- Maintain consistent font sizes and spacing.

### Layout
- Use a consistent navigation bar across all pages.
- Use large images and editorial-style layouts.
- Use cards to organize information.
- Use clear visual hierarchy.
- Keep sufficient spacing between sections.

### Responsive Design
- Support desktop, tablet, and mobile screens.
- Navigation and content layouts must adapt to smaller screens.
- Images must scale without distortion.
- Avoid horizontal scrolling.

---

## 4. Website Structure

The website contains five main sections.

### 4.1 Home (index.html)
The homepage should include:
- Website logo and navigation bar.
- Hero section introducing F1 Insider.
- Featured F1 content.
- Category cards linking to other pages.
- Footer with basic website information.

### 4.2 Drivers (pages/drivers.html)
The driver page should include:
- Driver name.
- Driver portrait.
- Nationality.
- Current or relevant team information.
- Short biography.
- Career highlights.

### 4.3 Teams (pages/teams.html)
The team page should include:
- Team name.
- Team logo or related image.
- Team nationality.
- Team introduction.
- Team history and characteristics.

### 4.4 Circuits (pages/circuits.html)
The circuit page should include:
- Grand Prix name.
- Country and location.
- Circuit image or track map.
- Circuit characteristics.
- Important corners and overtaking opportunities.

### 4.5 Racing Guide (pages/racing-guide.html)
The racing guide should introduce:
- Tire compounds.
- Pit stops.
- DRS.
- Qualifying.
- Basic race rules and terminology.

---

## 5. Content Guidelines

All new content must follow the existing website style and structure.

### Driver Content Format
Each driver introduction should contain:
1. Driver name (Chinese and English when available).
2. Nationality.
3. Team.
4. Profile image.
5. Short introduction.
6. Career highlights.

### Team Content Format
Each team introduction should contain:
1. Team name.
2. Nationality.
3. Team image or logo.
4. Team background.
5. Team characteristics.

### Circuit Content Format
Each circuit introduction should contain:
1. Grand Prix name.
2. Country.
3. Circuit image or track map.
4. Track characteristics.
5. Important corners.
6. Overtaking opportunities.

### Content Accuracy
- Use reliable and verifiable information.
- Do not invent driver statistics, race results, or team records.
- Distinguish historical information from current-season information.
- Verify time-sensitive information before publishing.
- Keep descriptions concise and beginner-friendly.

---

## 6. File Organization and Naming

Follow the existing project structure:

```text
f1-insider/
├── AGENTS.md
├── README.md
├── index.html
├── pages/
│   ├── drivers.html
│   ├── teams.html
│   ├── circuits.html
│   └── racing-guide.html
├── css/
│   └── style.css
├── js/
│   └── main.js
└── assets/
    ├── images/
    └── icons/
```

### Naming Rules
- Use lowercase English filenames.
- Use hyphens to separate words.
- Use `.html` for webpage files.
- Use `.css` for stylesheets.
- Use `.js` for JavaScript files.
- Use descriptive names for images.

Examples:
- `charles-leclerc.jpg`
- `suzuka-circuit.jpg`
- `mclaren-logo.png`

### File Placement
- All additional webpages belong in `pages/`.
- All styles belong in `css/`.
- All JavaScript files belong in `js/`.
- All images belong in `assets/images/`.
- All icons belong in `assets/icons/`.

Do not place unrelated files in the project root.

---

## 7. AI Development Rules

AI assistants must read this file before creating or modifying project files.

### Before Making Changes
1. Inspect the existing project structure.
2. Read the relevant HTML, CSS, and JavaScript files.
3. Understand existing design patterns.
4. Identify which files need to be changed.

### When Adding New Pages
1. Follow the existing color palette and typography.
2. Reuse the existing navigation bar and footer.
3. Maintain consistent spacing and layout.
4. Follow the appropriate content format.
5. Use the existing CSS and JavaScript whenever possible.
6. Ensure all navigation links work correctly.

### When Modifying Existing Pages
- Preserve existing content and functionality unless changes are requested.
- Avoid unnecessary changes to unrelated files.
- Do not duplicate existing CSS rules or JavaScript functions.
- Keep the code organized and readable.
- Explain important changes when completing a task.

### When Fixing Errors
- Identify the cause before changing code.
- Fix the problem without breaking other pages.
- Check relative file paths and navigation links.
- Verify that the page still works on desktop and mobile.

### General Rules
- Do not introduce unnecessary libraries or dependencies.
- Do not create duplicate pages or files.
- Do not change the overall visual identity without permission.
- Do not use fabricated F1 information.
- Follow this AGENTS.md whenever developing the project.

---

## 8. Quality Checklist

Before completing any development task, verify:

- [ ] HTML structure is valid.
- [ ] CSS and JavaScript files load correctly.
- [ ] Navigation links work.
- [ ] Images display correctly.
- [ ] The design follows the F1 Insider style.
- [ ] Content follows the defined format.
- [ ] Desktop and mobile layouts work.
- [ ] No existing functionality is accidentally removed.
- [ ] The website is compatible with GitHub Pages.

---

## 9. GitHub Pages Compatibility

- The website must be deployable as a static website.
- Use relative paths for internal pages and local assets.
- Avoid absolute local computer paths.
- Ensure `index.html` is located in the project root.
- Test all internal links after deployment.

---

## 10. Final Development Principle

Every new page should feel like part of the same F1 Insider website.

AI assistants should prioritize consistency, accuracy, readability, and maintainability.

The purpose of this project is to establish a reusable development system that allows new F1 content and webpages to be created efficiently by following the same set of rules.