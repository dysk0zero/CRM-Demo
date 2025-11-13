# CRM Demo
CRM UI built with plain HTML, CSS and JS.

## Contents

* [What You Get](#what-you-get)
* [Project Structure](#project-structure)
* [Getting Started](#getting-started)
* [Design System](#design-system)
* [Layout & Components](#layout--components)
* [Responsive Behavior](#responsive-behavior)
* [Accessibility](#accessibility)
* [Browser Support](#browser-support)
* [Performance Notes](#performance-notes)
* [Customization](#customization)
* [Roadmap](#roadmap)
* [License](#license)

---

## What You Get

* Responsive shell: sidebar, top bar, main content area
* Four screens:

  * **Dashboard**: KPIs and overview cards
  * **Contacts**: searchable/sortable table layout
  * **Projects**: pipeline/board view with project cards
  * **Profile**: user or company profile page with detail sections
* Utility classes for spacing, grid, and text
* Dark mode support (prefers-color-scheme first, optional class override)

---

## Project Structure

```
crm-vanilla/
├─ index.html                 
├─ contacts.html              
├─ projects.html              
├─ profile.html               
├─ styles.css
├─ components/   
├─ assets/
│  ├─ logos/
│  ├─ icons/                  
│  └─ sample/
└─ README.md
```

---

## Getting Started

1. Clone or download the folder.
2. Open `index.html` in any modern browser.

Optional local server:

```bash
# Python 3
python -m http.server 8080

# Or Node
npx http-server -p 8080
```

---

## Design System

CSS variables, typography scale, spacing tokens, and dark mode rules are defined in `base.css` and `themes.css`.

See the original [Design System](#design-system) section for details.

---

## Layout & Components

### App Shell

* Sidebar navigation linking to Dashboard, Contacts, Projects, and Profile
* Top bar with search and user menu
* Main content area as responsive grid

### Components

* Buttons (`.btn`, `.btn--primary`, etc.)
* Cards (`.card`)
* Tables for contacts
* Project cards in grid/board layout
* Profile detail sections (two-column on desktop, stacked on mobile)
* Badges, avatars, breadcrumbs, tabs, etc.

### Utilities

Simple spacing, flex, grid, and text helpers defined in `utilities.css`.

---

## Responsive Behavior

* Sidebar collapses below `md` breakpoint
* Dashboard cards wrap into fewer columns
* Contacts table turns into stacked cards on small screens
* Projects board becomes a vertical stack of project cards
* Profile page switches from two columns → one column

---

## Accessibility

* Semantic HTML for nav, header, main, section, aside, footer
* Clear focus states
* Tables use proper `<th>` and `scope` attributes
* Sidebar toggle and dark mode respect `aria-expanded` / system preferences

---

## Browser Support

* Chrome, Edge, Firefox, Safari (latest two versions)
* No IE support
* Works without JS; add your own JS if needed

---

## Performance Notes

* Minimal selector depth
* Inline SVG icons recommended
* Responsive images with fixed `width`/`height` attributes
* System font stack by default

---

## Customization

* Update branding in `assets/logos/`
* Change theme colors in `themes.css`
* Edit sidebar links to match your routes
* Add JS for interactivity (modals, toasts, sorting) if required

---

## Roadmap

* Expand projects board with drag-and-drop (requires JS)
* Add skeleton loaders for Dashboard and Contacts
* Print styles for Profile and Contacts
* High-contrast theme option

---

## License

MIT. Free to use, modify, and distribute.

---

Do you want me to also **update the sidebar/navigation HTML** so it only includes these four screens (Dashboard, Contacts, Projects, Profile)?
