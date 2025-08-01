---
title: "Create and Link a Module, Outcome, and Reading"
published: true
morea_id: experience-authoring
morea_type: experience
morea_summary: "Create and validate a set of linked content files using DESCARTES metadata rules"
morea_start_date:
morea_labels:
---

## Task: Author a Module, Outcome, and Reading

---

### 1. Create Three Files in `_morea/`:

**a. `module-test.md` (in `_morea/module-test/`)**

```markdown
---
title: "Test Module for Authoring"
published: true
morea_id: module-test
morea_type: module
morea_summary: "Test module for practicing content linking"
morea_sort_order: 0
morea_outcomes:
  - outcome-test
morea_readings:
  - reading-test
---
````

**b. `outcome-authoring.md` (in `_morea/outcome/`)**

```markdown
---
title: "Understand how to create content files"
published: true
morea_id: outcome-test
morea_type: outcome
morea_sort_order: 10
---
* You can define valid front matter for module content
```

**c. `reading-authoring-test.md` (in `_morea/reading/`)**

```markdown
---
title: "Authoring DESCARTES MOREA Files"
published: true
morea_id: reading-test
morea_type: reading
morea_summary: "How to structure and link content using front matter"
---
## Authoring Files

This reading provides a step-by-step walkthrough of content creation.
```

---

### 2. Serve and Verify

Run:

```bash
bundle exec jekyll serve
```

Then open:

```
http://127.0.0.1:4000/<baseurl>/morea/module-authoring-test/
```

Ensure the module displays both the outcome and reading links.

---
