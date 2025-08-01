---
title: "Clone and Run the DESCARTES MOREA Template"
published: true
morea_id: experience-clone-template
morea_type: experience
morea_summary: "Create a course repository from the DESCARTES template, inspect, and serve it using Jekyll"
morea_start_date: 
morea_labels:
---

## Clone and Run the DESCARTES MOREA Template (GitHub Desktop)

This experience uses GitHub Desktop to create a new repository from the DESCARTES MOREA template. You will clone it to your machine, install dependencies, and serve the site locally using Jekyll.

---

### 1. Create a Repository Using the DESCARTES Template

* Go to: [https://github.com/uhm-descartes/morea](https://github.com/uhm-descartes/morea)
* Click **Use this template** (green button)
* Set repository name (e.g., `course-name`)
* Set visibility to **Public**
* Click **Create repository from template**

---

### 2. Clone Using GitHub Desktop

* Open GitHub Desktop
* Go to **File > Clone repository**
* Select your new `course-name` repo from the GitHub.com tab
* Choose a local folder (e.g., `Documents/descartes-course`)
* Click **Clone**

---

### 3. Inspect Project Structure

Open the cloned folder. Confirm presence of:

- `_morea/` → contains markdown content files
- `_layouts/` → must include `morea-home.html`
- `index.md` → homepage for the course
- `_config.yml` → site configuration

If `_layouts/morea-home.html` is missing, copy it from the DESCARTES template.

---

### 4. Install Ruby, Bundler, and Jekyll

* Install Ruby ≥ 2.7 from [https://www.ruby-lang.org/en/documentation/installation/](https://www.ruby-lang.org/en/documentation/installation/)
* Open a terminal:

```bash
ruby -v
gem install bundler
````

* Navigate to the project directory:

```bash
cd path/to/course-name
bundle install
```

---

### 5. Serve the Site Locally

Run the Jekyll server:

```bash
bundle exec jekyll serve
```

Check terminal for:

```
Server address: http://127.0.0.1:4000/
```

Then check `_config.yml` for the `baseurl` setting:

* If `baseurl: ""`, open:

  ```
  http://127.0.0.1:4000/
  ```

* If `baseurl: "/course-name"`, open:

  ```
  http://127.0.0.1:4000/descartes-course/
  ```

You can also load specific pages directly:

```
http://127.0.0.1:4000<baseurl>/morea/<module-id>/<content-id>.html
```

Example:

```
http://127.0.0.1:4000/descartes-course/morea/foundations-morea-github/reading-foundations.html
```

---

### 6. Troubleshooting

* `Layout 'morea-home' does not exist` → Add from DESCARTES template `_layouts/`
* Site loads but shows 404 → Use `baseurl`-adjusted path
* `bundle install` fails → Ensure correct Ruby version and path

---
