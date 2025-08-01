---
title: "DESCARTES MOREA Template Concepts"
published: true
morea_id: reading-clone-template
morea_summary: "Conceptual overview of the DESCARTES MOREA GitHub template structure, metadata, and purpose."
morea_url:
morea_type: reading
morea_labels:
---

## DESCARTES MOREA Template Concepts

This reading introduces the design principles and metadata structure behind the DESCARTES MOREA template. It prepares you to understand how modular course content is organized, rendered, and deployed using static site generation.

---

### 1. What is the DESCARTES MOREA Template?

The template implements the MOREA (Modules, Outcomes, Readings, Experiences, Assessments) model using GitHub Pages and Jekyll. It provides a structured framework for defining modular course content with reproducible relationships and metadata.

---

### 2. Directory Structure and Purpose

The core content exists in the `_morea/` folder and is divided by content type:

- `module-*.md`: Defines a module and references its linked outcomes, readings, experiences, and assessments.
- `outcome-*.md`: Describes specific learning goals.
- `reading-*.md`: Provides conceptual content or linked external sources.
- `experience-*.md`: Describes tasks, labs, or exercises.
- `assessment-*.md`: Evaluates understanding or application.

Templates for layout are located in `_layouts/` and `_includes/`. Static assets (CSS, JS, images) are stored in `assets/`.

---

### 3. YAML Metadata

Each file begins with a YAML front matter block. The fields define how Jekyll processes content and how MOREA links components:

* `morea_id`: Globally unique identifier. Used to link across modules.
* `morea_type`: Specifies the content role (`module`, `outcome`, `reading`, `experience`, or `assessment`).
* `morea_summary`: Brief description shown on module overview pages.
* `morea_sort_order`: Numeric value for ordering content within a module.
* `morea_outcomes`, `morea_readings`, `morea_experiences`, `morea_assessments`: Lists of `morea_id`s that define the module’s components.

---

### 4. Static Site Generation with Jekyll

Jekyll processes all `.md` files into HTML using layout templates. It compiles the site locally or on GitHub Pages, transforming structured markdown into a full static website.

---

### Readings

- [MOREA Framework Overview](https://morea-framework.github.io/)
- [GitHub Pages and Jekyll](https://docs.github.com/en/pages)
- [YAML Front Matter](https://jekyllrb.com/docs/front-matter/)
- [DESCARTES Initiative](https://descartes.manoa.hawaii.edu/)

