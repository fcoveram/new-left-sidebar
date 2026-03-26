# New Left Sidebar

A WordPress admin plugin that replaces the default wp-admin sidebar with a cleaner, Site Editor-inspired navigation. The layout mirrors the look of the Gutenberg site editor — dark background, 300px fixed sidebar, white rounded content card — bringing visual consistency to the entire admin experience.

The menu is reorganized into a logical hierarchy: primary content items (Dashboard, Posts, Pages, Comments, Media) sit at the top, followed by a **Design** folder grouping Themes, Styles, Navigation, Templates, and Patterns. Plugins, Users, and Tools come next, and Settings is separated into its own drilldown section. Design items are shown only when a block theme is active, so the sidebar adapts to the site's capabilities without cluttering the menu.

The Settings section uses a drilldown pattern: clicking Settings replaces the entire menu with a focused sub-navigation (General, Writing, Reading, Discussion, Media, Permalinks, Privacy) plus a Back button to return to the main menu. This keeps the sidebar uncluttered and mirrors the nested navigation patterns common in modern app UIs. The drilldown activates automatically when the user is already on a Settings sub-page.

All icons are sourced from the official `@wordpress/icons` package and rendered as inline SVG data URIs, so they match the icon language used throughout the block editor. The plugin is a single-file PHP drop-in with a companion CSS and JS file — no build step, no dependencies, no database writes.
