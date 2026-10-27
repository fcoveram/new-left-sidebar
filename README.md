# New Left Sidebar

**Try it without installing:** <https://prototypes.fvm.house/new-left-sidebar/> opens a WordPress Playground site with the plugin already active.

A WordPress admin plugin that replaces the default wp-admin sidebar with a cleaner, Site Editor-inspired navigation. The layout mirrors the look of the Gutenberg site editor — dark background, 300px fixed sidebar, white rounded content card — bringing visual consistency to the entire admin experience.

The menu is reorganized into a logical hierarchy: primary content items (Dashboard, Posts, Pages, Comments, Media) sit at the top, followed by a **Design** folder grouping Themes, Styles, Navigation, Templates, and Patterns. Plugins, Users, and Tools come next, and Settings is separated into its own drilldown section. Design items are shown only when a block theme is active, so the sidebar adapts to the site's capabilities without cluttering the menu.

The Settings section uses a drilldown pattern: clicking Settings replaces the entire menu with a focused sub-navigation (General, Writing, Reading, Discussion, Media, Permalinks, Privacy) plus a Back button to return to the main menu. This keeps the sidebar uncluttered and mirrors the nested navigation patterns common in modern app UIs. The drilldown activates automatically when the user is already on a Settings sub-page.

All icons are sourced from the official `@wordpress/icons` package and rendered as inline SVG data URIs, so they match the icon language used throughout the block editor. The plugin is a single-file PHP drop-in with a companion CSS and JS file — no build step, no dependencies, no database writes.

---

## Installation

### Option A — Upload via WordPress admin (recommended)

1. Go to the [Releases page](https://github.com/fcoveram/new-left-sidebar/releases) and download the latest `new-left-sidebar.zip`.
2. In your WordPress admin, go to **Plugins → Add New Plugin**.
3. Click **Upload Plugin**, choose the zip file, and click **Install Now**.
4. Click **Activate Plugin**.

### Option B — Manual upload via FTP / file manager

1. Download and unzip `new-left-sidebar.zip`.
2. Upload the `new-left-sidebar` folder to `/wp-content/plugins/` on your server.
3. In your WordPress admin, go to **Plugins** and activate **New Left Sidebar**.

### Requirements

| | Minimum | Recommended |
|---|---|---|
| WordPress | 6.0 | Latest |
| PHP | 7.4 | 8.2+ |

---

## File structure

```
new-left-sidebar/
├── new-left-sidebar.php   # Plugin bootstrap and menu reorganization
├── css/
│   └── style.css          # Admin layout and sidebar styles
├── js/
│   └── sidebar.js         # Settings drilldown behaviour
├── readme.txt             # WordPress.org-format readme
└── README.md              # This file
```

---

## License

[GPL-2.0-or-later](https://www.gnu.org/licenses/gpl-2.0.html)
