---
title: "Customize Layout and Style for DESCARTES MOREA"
published: true
morea_id: experience-custom-layout-style
morea_type: experience
morea_summary: "Modify layouts, includes, and select a theme from css/themes to match DESCARTES branding and adjust navigation structure."
morea_start_date:
morea_labels:
  - jekyll
  - layout
  - css
  - themes
  - customization
---

## Customize Layout and Style

This experience covers editing `_layouts`, `_includes`, and changing the site theme to align appearance and navigation with DESCARTES specifications.

---

### 1. Locate Layout Files

Open `_layouts/` in the project root. Identify:

- `morea-home.html` (homepage layout)
- `morea-page.html` (standard page layout)
- `default.html` (base HTML structure)

---

### 2. Modify Header and Footer

Edit `_includes/header.html` and `_includes/footer.html`:

- Replace placeholder logos with DESCARTES/UH Mānoa logos stored in `images/`.
- Update navigation links to reflect intended course structure.
- Remove unused menu items.

---

### 3. Adjust Sidebar

If `_includes/sidebar.html` exists:

- Add links to related DESCARTES modules.
- Organize navigation into logical sections.
- Remove irrelevant links from template defaults.

---

### 4. Change Theme

The template provides pre-defined CSS themes located in `css/themes/`:

- `cerulean`
- `cerulean-green`
- `cerulean-purple`
- `cerulean-red`
- `darkly` 
- `spacelab`

To change the active theme, edit `_config.yml`, change the `morea_theme` to any of the above. [Explore more about morea themes here](https://morea-framework.github.io/docs/instructors/themes).

```yaml
morea_theme: cerulean
````

---

### 5. Test Changes Locally

Run:

```bash
bundle exec jekyll serve
```

Check:

* Homepage branding reflects selected theme.
* Navigation structure matches intended module organization.
* Theme styles apply correctly on desktop and mobile.

---

### 6. Troubleshooting

* Theme changes not applied: Confirm `morea_theme` path in `_config.yml` matches an existing file in `css/themes/`.
* Layout not updating: Clear Jekyll cache with `bundle exec jekyll clean` then rebuild.
* Logo not displaying: Verify correct file name and path in `_module-icons/`.
