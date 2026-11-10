# AGENTS.md

# F1 Insider — Project Development Guidelines

## 1. Project Overview
F1 Insider is a Formula 1 knowledge website designed for beginners and motorsport fans.
The website provides organized information about Formula 1 drivers, teams, circuits, and racing knowledge.

### Project Goals
- Introduce Formula 1 to beginners.
- Provide clear and accessible motorsport information.
- Cover the expanded starting grid: 11 teams and 22 full-time drivers (including Cadillac F1 Team).
- Organize F1 knowledge into different categories with in-page instant exploration and standalone pages.
- Maintain a consistent design and structure across all pages.
- Allow new content and pages to be added easily.

### Target Audience
- People who are new to Formula 1.
- Formula 1 fans who want to learn more about drivers and teams.
- Readers interested in racing circuits, race strategies, flags, and telemetry.

### Language
- Traditional Chinese (繁體中文) is the primary language.
- English names and official F1 terminology should be preserved when appropriate.

---

## 2. Technology Stack
- HTML5: Website structure and content.
- CSS3: Layout, styling, responsive design, and animations.
- Vanilla JavaScript: Interactive elements, tabs, filters, and API connections.

### Development Restrictions
- Do not use React, Vue, or other JavaScript frameworks.
- Do not require a backend or database.
- Keep the website compatible with GitHub Pages.
- Prefer simple, readable, and maintainable code.

---

## 3. Design Guidelines

### Visual Identity
The website follows a modern Formula 1 editorial and motorsport magazine style.
The overall appearance should be professional, bold, dynamic, and easy to navigate.

### Color Palette
- Primary Background: #111111
- Secondary Background: #1C1C1C
- Brand Red: #D71920
- Primary Text: #F5F5F5
- Secondary Text: #999999
- Border: #333333

### Typography
- Display font: Barlow Condensed (bold/black, uppercase for labels/meta).
- Body text font: Noto Sans TC.
- Consistent font sizes, hierarchy, and line heights.

### Responsive Design
- Support desktop, tablet, and mobile screens.
- Navigation collapses into a mobile hamburger menu under 700px.
- Avoid horizontal scrolling.

---

## 4. Website Structure
The website contains five main sections:
1. Home (`index.html`) with in-page category explorer & real-time API sync.
2. Drivers (`pages/drivers.html` & Hub): Full 22-driver roster across 11 teams.
3. Teams (`pages/teams.html` & Hub): Full 11 constructor teams including Cadillac F1 Team.
4. Circuits (`pages/circuits.html` & Hub): Grand Prix circuit profiles.
5. Racing Guide (`pages/racing-guide.html` & Hub): Comprehensive racing guide (tires, DRS, undercut/overcut, flags, sprint format, penalties).

---

## 5. Standings & Guide Feature Rules
- **Standings**: Support switching between Drivers Championship and Constructors Championship. Support toggling between Top 8/10 and Full Grid. Maintain live API fetching with graceful fallback.
- **Racing Guide**: Must cover at least 6 core modules:
  1. Tire Specifications (C1-C5, Soft, Medium, Hard, Inters, Wet)
  2. DRS & Active Aerodynamics
  3. Pit Strategy Matrix (Undercut vs Overcut)
  4. Track Safety & Flag Legend (Green, Yellow, Red, Blue, Black & White, Black)
  5. Knockout Qualifying & Sprint Weekend
  6. Stewards, Penalties, and Super License Points

---

## 6. AI Development Rules
1. **Preserve Design System**: Always reuse existing CSS variables (`--bg`, `--surface`, `--red`, `--text`, `--border`).
2. **Dual Maintenance**: Whenever updating driver or team entries, update both `index.html` (interactive hub) and the corresponding files in `pages/`.
3. **Accuracy**: Use genuine F1 driver names, numbers, team engines, and circuit characteristics.
