---
title: "Collaborative Version Control with Git"
published: true
morea_id: experience-version-control-collaboration
morea_type: experience
morea_summary: "Apply branching, pull requests, and conflict resolution for DESCARTES MOREA course development using Git or GitHub Desktop."
morea_start_date:
morea_labels:
  - git
  - branching
  - pull-requests
  - merge-conflicts
  - github-desktop
---

## Collaborative Version Control with Git

This experience covers branching, pull requests, and merge conflict resolution for DESCARTES MOREA course repositories, with instructions for both command line and GitHub Desktop.

---

### 1. Create and Switch to a Branch

**Command line:**
```bash
git checkout -b feature-module-update
````

**GitHub Desktop:**

* Go to **Branch > New Branch**.
* Enter branch name (e.g., `feature-module-update`).
* Click **Create Branch**.

---

### 2. Commit Changes

**Command line:**

```bash
git add .
git commit -m "Update module content"
```

**GitHub Desktop:**

* Review changes in the **Changes** tab.
* Enter summary in the **Summary** field.
* Click **Commit to feature-module-update**.

---

### 3. Push Branch to Remote

**Command line:**

```bash
git push origin feature-module-update
```

**GitHub Desktop:**

* Click **Publish branch** in the top bar.

---

### 4. Open Pull Request

In GitHub (web):

* Navigate to repository.
* Click **Compare & pull request**.
* Write concise description of changes.
* Assign reviewer.

---

### 5. Review and Merge

Reviewer:

* Reads file changes.
* Leaves comments or approves.

Merge:

**Command line:**

```bash
git checkout main
git pull
git branch -d feature-module-update
```

**GitHub Desktop:**

* Switch to `main` branch.
* Pull latest changes.
* Delete feature branch via **Branch > Delete**.

---

### 6. Resolve Merge Conflicts

If conflict occurs:

**Command line:**

```bash
git merge feature-module-update
```

Manually edit files, then:

```bash
git add .
git commit
```

**GitHub Desktop:**

* Conflicts appear in **Changes** tab.
* Open each conflicted file and choose changes.
* Mark as resolved, then commit.

---

### 7. Enforce Workflow

* Require at least one review before merge.
* Protect `main` branch via repository settings.
