---
title: "DESCARTES MOREA Layout and Style Customization"
published: true
morea_id: reading-custom-layout-style
morea_summary: "Overview of Jekyll layouts, includes, and theme selection in the DESCARTES MOREA template."
morea_type: reading
morea_labels:
  - jekyll
  - layout
  - css
  - themes
---

## Layout and Style Customization

The DESCARTES MOREA template uses Jekyll layouts, includes, and selectable themes to control structure and styling.

---

### Layouts

Stored in `_layouts/`. Define page-level HTML structure:

- `morea-home.html`: Homepage with module list.
- `morea-page.html`: Standard content layout.
- `default.html`: Base wrapper for all layouts.

---

### Includes

Stored in `_includes/`. Contain reusable HTML fragments:

- `header.html` and `footer.html`: Branding and navigation.
- `sidebar.html`: Contextual navigation if present.

---

### Themes

The template provides pre-defined CSS themes located in `css/themes/`:

- `cerulean`
- `cerulean-green`
- `cerulean-purple`
- `cerulean-red`
- `darkly`
- `spacelab`

Change the active theme by editing `_config.yml` and setting:

```yaml
morea_theme: cerulean
````

Replace `cerulean` with the desired theme name. The value must match an existing file in `css/themes/` without the `.css` extension.

Theme changes update colors, typography, and visual style without manual CSS edits.
Reference: [Morea Themes Documentation](https://morea-framework.github.io/docs/instructors/themes)

---

### Branding Changes

* Replace logo images in `_module-icons/` and update references in `_includes/header.html`.
* Adjust navigation text and structure in `header.html` and `sidebar.html` to align with course organization.

---

### Navigation Adjustments

Edit `_includes/sidebar.html` and `_includes/header.html` to:

* Link to related modules.
* Organize menu items by category.
* Remove unused or irrelevant links.

---

### References

* [Jekyll Layouts](https://jekyllrb.com/docs/layouts/)
* [Jekyll Includes](https://jekyllrb.com/docs/includes/)
* [Morea Themes](https://morea-framework.github.io/docs/instructors/themes)
