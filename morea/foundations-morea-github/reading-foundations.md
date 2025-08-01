---
title: "Introduction to GitHub, Git, and Static Site Generation"
published: true
morea_id: reading-foundations
morea_summary: "Foundational reading on Git, GitHub, and how static sites like MOREA are generated and hosted."
morea_url:
morea_type: reading
morea_labels:
---

## Introduction to GitHub, Git, and Static Site Generation

This guide explains the core tools used in MOREA websites. You’ll learn what Git is, what GitHub does, and how static websites work using Jekyll.

---

### 1. What is Git?

Git is software that tracks changes in files.

* **Local version control**: Git runs on your computer. It remembers what you changed and when.
* **Key commands**:

  * `git init`: Start using Git in a folder.
  * `git add`: Tell Git which files to track.
  * `git commit`: Save a version of your files with a message.
  * `git log`: See all past versions.
* **Distributed system**: Each person has their own full copy of the code. Changes can be shared between copies.

---

### 2. What is GitHub?

GitHub is a website that stores Git repositories (projects) online.

* **Remote storage**: Your code lives in the cloud so others can see or edit it.
* **Accounts and permissions**: You need an account. You control who can edit your code.
* **Common actions**:

  * **Forking**: Make your own copy of someone else’s project.
  * **Cloning**: Download a copy to your computer.
  * **Pull requests**: Ask to merge your changes into another copy.

---

### 3. What is a Static Site?

A static site shows fixed content. There is no database or live server code.

* **How it works**: Pages are written ahead of time and stored as files.
* **Jekyll**: A tool that turns text files into a website.
* **Why use static sites**:

  * Easy to track with Git.
  * Can live on GitHub Pages for free.
  * Fast and secure. No backend to break.

---

### Resources

- [Git - The Simple Guide](https://rogerdudler.github.io/git-guide/)
- [GitHub Docs: Get Started](https://docs.github.com/en/get-started)
- [What is Jekyll](https://jekyllrb.com/docs/)
- [Static site vs. dynamic site](https://blog.hubspot.com/website/static-vs-dynamic-website)

This knowledge is foundational for understanding how MOREA content is versioned, structured, and served on the web. In DESCARTES, this model enables modular, and verifiable course resources.
