---
title: "Version Control and Collaboration in DESCARTES MOREA"
published: true
morea_id: reading-version-control-collaboration
morea_summary: "Overview of Git workflows for collaborative module development in DESCARTES, with both command line and GitHub Desktop."
morea_type: reading
morea_labels:
  - git
  - branching
  - pull-requests
  - merge-conflicts
  - github-desktop
---

## Git Collaboration for DESCARTES

---

### Branching

Each feature or fix should be developed in its own branch.

**Command line:**  
Use `git checkout -b branch-name`.

**GitHub Desktop:**  
Use **Branch > New Branch**, enter the name, and click **Create Branch**.

---

### Pull Requests

Used to integrate branch changes into `main`.

- Opened from GitHub web interface.
- Reviewed by at least one collaborator before merging.

---

### Merge Conflicts

Occur when two commits modify the same lines.

**Command line:**  
Merge the branch, edit conflicts, stage, and commit.

**GitHub Desktop:**  
Conflicts appear in the **Changes** tab. Choose changes in editor, mark as resolved, commit.

---

### Branch Protection

Configure in GitHub repository settings to:

- Require pull request review.
- Prevent direct pushes to `main`.
- Enforce status checks before merge.

---

### Tools

- **Command line Git** for full control and scripting.
- **GitHub Desktop** for a GUI-based workflow.

---

### References

- [Git Branching](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell)
- [About Pull Requests](https://docs.github.com/en/pull-requests)
- [Resolving Merge Conflicts](https://docs.github.com/en/get-started/using-git/resolving-merge-conflicts)
- [GitHub Desktop](https://desktop.github.com/)