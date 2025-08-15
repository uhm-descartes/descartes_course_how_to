---
title: "Deploy and Maintain DESCARTES MOREA Sites"
published: true
morea_id: experience-deployment-maintenance
morea_type: experience
morea_summary: "Use GitHub Pages to deploy DESCARTES MOREA sites, maintain live content, and approve updates from the template repository."
morea_start_date:
morea_labels:
  - github-pages
  - deployment
  - maintenance
  - dns
  - versioning
---

## Deploy and Maintain DESCARTES MOREA Sites

---

### 1. Configure GitHub Pages

In repository settings:

- Go to **Settings > Pages**.
- Under **Source**, select branch `main` and `/ (root)` directory.
- Save settings and note the live site URL.

---

### 2. Deploy Using Included GitHub Actions

The DESCARTES MOREA template already contains a GitHub Actions workflow for automatic builds and deployment to Pages.  
No additional configuration is required beyond enabling Pages in settings.

---

### 3. Update Live Content

- Edit `.md` files in `_morea/` or other source directories.
- Commit and push changes to `main`.
- GitHub Actions will rebuild and deploy automatically.

---

### 4. Troubleshoot Build Errors

- Review GitHub Actions logs in the **Actions** tab.
- Verify Ruby and gem versions match those in the template `Gemfile`.
- Fix YAML syntax errors in front matter blocks.
- Ensure required layouts and includes are present.

---

### 5. Configure Custom Domain (Optional)

In **Settings > Pages**:

- Enter domain name (e.g., `course.example.edu`).
- Add corresponding CNAME record to your DNS.
- Enable HTTPS.

---

### 6. Approve Pull Requests from Template

The template may issue automated pull requests to update workflows or configuration:

- Navigate to the **Pull Requests** tab.
- Review the changes for impact.
- Approve and merge if they align with your site’s needs.

---

### 7. Routine Maintenance

- Test local builds periodically using `bundle exec jekyll serve`.
- Update Ruby gems with `bundle update` when needed.
- Remove outdated or unused content to keep repository clean.
