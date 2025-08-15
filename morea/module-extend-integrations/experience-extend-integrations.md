---
title: "Extend DESCARTES MOREA with Integrations"
published: true
morea_id: experience-extend-integrations
morea_type: experience
morea_summary: "Embed interactive tools and integrate DESCARTES modules with UH-supported platforms."
morea_start_date:
morea_labels:
  - integrations
  - embeds
  - lms
  - h5p
  - jupyter
---

## Extend DESCARTES MOREA with Integrations

---

### 1. Embed External Media

In `.md` files, use HTML for embedding:

- YouTube video:

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>
````

* Google Form:

```html
<iframe src="https://docs.google.com/forms/d/e/FORM_ID/viewform?embedded=true" width="640" height="800" frameborder="0">Loading…</iframe>
```

---

### 2. Insert H5P Content

If H5P content is hosted:

```html
<iframe src="H5P_URL" width="1090" height="614" frameborder="0" allowfullscreen="allowfullscreen"></iframe>
```

---

### 3. Integrate Jupyter Notebooks

Convert `.ipynb` to HTML:

```bash
jupyter nbconvert notebook.ipynb --to html
```

Place in `morea/` and link from markdown.

---

### 4. Link to LMS (Lamaku or UH-supported)

* Identify course module in LMS.
* Provide deep link in DESCARTES content.
* Test for authentication requirements.

---

### 5. Document Integration Steps

Create or maintain `morea/notes-integrations.md` listing:

* Tool name
* Embed/link method
* Dependencies or permissions required

---

### 6. Test Compatibility

Serve locally and verify embeds load.
Confirm functionality on GitHub Pages.
