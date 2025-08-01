---
title: "Home"
morea_id: home
morea_type: home
published: true
---

## DESCARTES Module

<div class="alert alert-danger" role="alert" markdown="1">

  <i class="fa-solid fa-circle-exclamation fa-xl"></i> **Warning: this is not a website for a real course.**
  <hr/>
  
  It is actually the "demo" site for building DESCARTES Modules. 

  See the <a href="https://morea-framework.github.io">Morea Framework Project Site</a> for details.
</div>

This course guides educators at UH Mānoa, particularly within the DESCARTES initiative, through the process of designing, building, and deploying a MOREA-based course site using GitHub Pages. It emphasizes modular design, where each module is intended to be self-contained but integrable with other DESCARTES modules via defined prerequisites and relationships.

## Modules

### Module 1: Foundations of MOREA and GitHub

**Objectives**  
- Define the purpose and structure of MOREA (Modules, Outcomes, Readings, Experiences, Assessments)  
- Understand how DESCARTES uses MOREA modules to create modular, recombinable resources  
- Set up a GitHub account and install Git locally  
- Understand the role of static site generation in DESCARTES resource publishing

**Estimated Time**: 1 hour  
**Prerequisites**: None

---

### Module 2: Cloning and Running the MOREA Template

**Objectives**  
- Clone the DESCARTES-compliant MOREA GitHub template  
- Examine directory and file layout in context of DESCARTES metadata conventions  
- Run the site locally using Jekyll (`bundle install`, `bundle exec jekyll serve`)  
- Configure deployment through GitHub Pages and understand DNS considerations for UH hosting

**Estimated Time**: 1.5 hours  
**Prerequisites**: Module 1

---

### Module 3: Authoring Course Content in DESCARTES MOREA

**Objectives**  
- Create `module-`, `outcome-`, `reading-`, `experience-`, and `assessment-` files in the correct `_morea/module-name/` subdirectory  
- Populate required front matter fields for each content type, including `morea_id`, `morea_type`, and `morea_summary`  
- Use `morea_outcomes`, `morea_readings`, etc. arrays to link related content by ID  
- Use `morea_sort_order` to sequence content within a module  
- Link assessments to outcomes using `morea_outcomes_assessed`  
- Validate file structure and metadata through successful site build and rendering

**Estimated Time**: 2.5 hours  
**Prerequisites**: Module 2

---

### Module 4: Customizing Layout and Style

**Objectives**  
- Modify `_layouts`, `_includes`, and `assets` to reflect DESCARTES branding and UI needs  
- Customize the homepage and sidebar to emphasize modular course reuse and cross-linking 

**Estimated Time**: 1 hour  
**Prerequisites**: Module 3

---

### Module 5: Version Control and Collaboration

**Objectives**  
- Implement collaborative workflows using Git branches and pull requests  
- Manage issues and contributions from multiple DESCARTES collaborators  
- Resolve merge conflicts in a reproducible, minimal-downtime workflow

**Estimated Time**: 1 hour  
**Prerequisites**: Module 5

---

### Module 6: Deployment and Maintenance

**Objectives**  
- Understand GitHub Actions for automated deployment  
- Update and maintain live content during a term  
- Troubleshoot build errors and site issues  
- Archive and version past course iterations  
- Configure a custom domain via GitHub Pages DNS settings  

**Estimated Time**: 2 hours  
**Prerequisites**: Module 6

---

### Module 7: Extending with Integrations

**Objectives**  
- Embed Google Forms, videos, Jupyter Notebooks, or H5P where pedagogically relevant  
- Integrate DESCARTES modules with Lamaku or other UH-supported LMS platforms  
- Identify and document technical pain points where intelligent agents could support authoring

**Estimated Time**: 1 hour  
**Prerequisites**: Module 7