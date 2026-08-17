# TAPAS PCE — Meditation & Wellness Club Website

Official frontend website for **TAPAS PCE** (Pillai College of Engineering), a student-led campus community dedicated to Heartfulness relaxation, guided meditation, stress management, and holistic personal wellness.

---

## 🌟 Project Architecture & Technologies

* **Structure**: Semantic HTML5 with accessibility attributes (`aria-*`, `role`).
* **Styling**: Vanilla CSS3 using custom CSS variables (Design Tokens), smooth micro-animations, and fluid responsive breakpoints (no CSS frameworks required).
* **Scripting**: Modular Vanilla JavaScript (ES6+) with zero external JS libraries, frameworks, or backend dependencies.
* **Branding**: Official unedited TAPAS PCE logo with brand colors:
  * Primary Orange: `#F59E0B`
  * Primary Blue: `#249BC3`
  * Accent Green: `#22C55E`
  * Dark Text: `#1F2937` (Light Mode) / `#F8FAFC` (Dark Mode)
  * Background: `#FFFDF7` (Light Mode) / `#0F172A` (Dark Mode)

---

## 📁 Project Directory Structure

```text
tapas-website/
├── index.html          # Homepage (Hero, Countdown, Offers, Breathing, Testimonials, CTA)
├── about.html          # About Club, Vision, Mission, 6 Values, and Visual Timeline
├── events.html         # Event search, filters, dynamic cards, details modal, and registration system
├── meditation.html     # Interactive breathing exercise studio, 1/5/10 min timer, and wellness tips
├── gallery.html        # Moments gallery with category filters and fullscreen lightbox
├── team.html           # Core Team, Coordinators, and Volunteers showcase
├── contact.html        # 2-column contact info, accessible form validation, and feedback view
├── css/
│   ├── style.css       # Global design system tokens, typography, components, and dark theme
│   └── responsive.css  # 5-tier responsive layout rules (360px, 480px, 768px, 1024px, 1440px)
├── js/
│   ├── main.js         # Theme toggle (☀️/🌙), mobile drawer, countdown timer, contact validation
│   ├── events.js       # Event data array, rendering, search/filters, registration modal & localStorage demo
│   ├── meditation.js   # Breathing studio state machine & meditation timer with Web Audio API chime
│   └── gallery.js      # Gallery data array, dynamic grid, category filters, and lightbox controls
├── images/
│   ├── tapas-logo.png  # Official unedited TAPAS PCE logo
│   ├── hero/           # Hero visual placeholders
│   ├── events/         # Event photos
│   ├── gallery/        # Gallery captures
│   └── team/           # Team member avatars
└── README.md           # Project documentation
```

---

## 🚀 Key Features Implemented

1. **Theme Mode (☀️ / 🌙)**:
   * Instant toggle in the sticky navbar.
   * Uses CSS variables in `[data-theme="dark"]`.
   * Preserves user preference in `localStorage.setItem('tapas_theme', ...)`.
   * Zero flash of unstyled theme on page refresh.

2. **Interactive Breathing Exercise Studio** ([`meditation.html`](file:///c:/Users/Asus/OneDrive/Documents/tapas/tapas-website/meditation.html)):
   * Large animated expanding/contracting circle with 3 distinct phases (*Breathe In*, *Hold*, *Breathe Out*).
   * Full controls: `Start`, `Pause`, `Reset`.

3. **Meditation Timer** ([`meditation.html`](file:///c:/Users/Asus/OneDrive/Documents/tapas/tapas-website/meditation.html)):
   * Presets for 1 Min, 5 Min, and 10 Min.
   * Accurate countdown, pause, resume, reset.
   * Built-in singing bowl audio chime synthesized procedurally via Web Audio API (zero audio file dependencies).

4. **Events & Registration System** ([`events.html`](file:///c:/Users/Asus/OneDrive/Documents/tapas/tapas-website/events.html)):
   * Real-time live search across titles, descriptions, and venues.
   * Category filter pills (*All, Meditation, Wellness, Workshop, Community, Other*).
   * Event details modal and interactive registration modal.
   * Input validation for name, email, department, year, and phone number.
   * Saves registrations to browser `localStorage` (`tapas_event_registrations`) with immediate success screen.

5. **Gallery & Fullscreen Lightbox** ([`gallery.html`](file:///c:/Users/Asus/OneDrive/Documents/tapas/tapas-website/gallery.html)):
   * Filter photos by category (*All, Meditation, Workshops, Events, Community*).
   * Fullscreen lightbox modal with `Previous`, `Next`, image counter (`1 / 8`), and full keyboard support (`Escape`, `ArrowLeft`, `ArrowRight`).

6. **Contact Form & Client Validation** ([`contact.html`](file:///c:/Users/Asus/OneDrive/Documents/tapas/tapas-website/contact.html)):
   * Name, email format, subject, and message length verification.
   * Summary confirmation view upon submission with clear demo notice.

7. **5-Tier Responsive System** ([`css/responsive.css`](file:///c:/Users/Asus/OneDrive/Documents/tapas/tapas-website/css/responsive.css)):
   * Fully tested for `360px`, `480px`, `768px`, `1024px`, and `1440px+`.
   * Zero horizontal overflow.
   * Mobile hamburger drawer navigation.
   * Accessibility support for `prefers-reduced-motion: reduce`.

---

## 📝 Placeholders to Customize with Real Information

When ready to populate the website with live club data, update these clearly marked placeholders:

### 1. Contact & Social Links
* **Instagram**: Replace `[Add TAPAS Instagram]` with your actual handle (e.g. `@tapas_pce`).
* **Email**: Replace `[Add TAPAS Email]` with the official email (e.g. `tapas@pce.ac.in`).
* **Location**: Replace `[Add PCE location]` with specific hall numbers or campus spots (e.g. *Seminar Hall, 4th Floor, PCE*).

### 2. Team Members ([`team.html`](file:///c:/Users/Asus/OneDrive/Documents/tapas/tapas-website/team.html))
* Replace `[Team Member Name]`, `[Position]`, and social links (`[Add Instagram]`, `[Add LinkedIn]`) in the Core Team, Coordinators, and Volunteers sections.

### 3. Events ([`js/events.js`](file:///c:/Users/Asus/OneDrive/Documents/tapas/tapas-website/js/events.js))
* Update the `events` array with actual dates, times, venues, and descriptions.

### 4. About History ([`about.html`](file:///c:/Users/Asus/OneDrive/Documents/tapas/tapas-website/about.html))
* Replace `[Add actual year]` and `[Add actual TAPAS history]` in the timeline section.

---

## 🖼️ Images to Replace Later

Place your high-resolution images in the following folders:
1. **Hero**: `images/hero/`
2. **Events**: `images/events/`
3. **Gallery**: `images/gallery/`
4. **Team Avatars**: `images/team/`

---

## 💻 Running the Website Locally

Double-click `index.html` in any web browser (Chrome, Firefox, Edge, Safari) or run a local server:

```bash
# Optional: Using Python built-in server
python -m http.server 8000
```
Visit `http://localhost:8000` in your browser.
