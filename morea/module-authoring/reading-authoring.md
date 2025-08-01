---
title: "Structure and Metadata of DESCARTES MOREA Content"
published: true
morea_id: reading-authoring
morea_summary: "Metadata, structure, and linking logic for all MOREA content types"
morea_url:
morea_type: reading
morea_labels:
---

## DESCARTES MOREA Content Structure

---

### 1. Directory Structure

DESCARTES MOREA sites organize all course content under the `_morea/` directory using a nested folder structure:

```
root/
_morea/
module-name/
module-name-module.md
module-name-outcome.md
module-name-reading.md
module-name-experience.md
module-name-assessment.md
````

All files related to a single instructional unit (module) are grouped within the same folder. File names must begin with the module's `morea_id` and end with their content type.

---

### 2. Content Types

- `*-module.md` — groups related outcomes, readings, experiences, and assessments  
- `*-outcome.md` — defines a specific, assessable learning goal  
- `*-reading.md` — provides conceptual or reference material  
- `*-experience.md` — describes a hands-on or task-based activity  
- `*-assessment.md` — evaluates understanding and links to one or more outcomes

---

### 3. Required Front Matter Fields

All files must include:

- `morea_id`: unique, lowercase, hyphenated identifier
- `morea_type`: one of `module`, `outcome`, `reading`, `experience`, `assessment`
- `title`: descriptive title
- `published`: must be `true` for the file to render
- `morea_summary`: (except for outcomes) short description for display in module view
- `morea_sort_order`: numeric ordering value for display sequence

Modules must also include arrays like:

- `morea_outcomes`
- `morea_readings`
- `morea_experiences`
- `morea_assessments`

Assessments must include:

- `morea_outcomes_assessed`: a list of outcome `morea_id`s

---

### 4. Linking Logic

All relationships between files are declared using `morea_id` values. Jekyll and the DESCARTES MOREA plugin use these references to generate cross-linked module pages.

Example `*-module.md` file:

```yaml
morea_outcomes:
  - foundations-outcome
morea_readings:
  - foundations-reading
morea_experiences:
  - foundations-experience
morea_assessments:
  - foundations-assessment
````

---

### 5. Summary

A DESCARTES MOREA site is structured by module directories inside `_morea/`, with filenames and `morea_id`s aligned per content type. Metadata consistency, naming alignment, and valid linking are mandatory for site functionality and modular reuse.

