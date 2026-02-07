# Minimalist AI/Robotics Portfolio Template

A clean, single-page portfolio website designed for AI Researchers and Roboticists. It features a responsive grid layout, a dedicated list view for publications and blogs, and a client-side search engine—all contained within a **single HTML file**.

**Live Demo:** [Link to your github.io page]

---

## 🚀 Features

* **Single File:** No frameworks, no build steps (React/Vue/Jekyll), just one `index.html`.
* **Instant Search:** Filter projects, papers, videos, and blogs in real-time.
* **Smart "See All" Logic:** Automatically handles expanding/collapsing lists based on custom item limits.
* **Academic Focused:** Specialized layouts for "Projects" (Grid), "Papers" (List), and "Blogs" (Date-aligned List).
* **Responsive:** Looks great on mobile, tablet, and desktop.
* **Zero Maintenance:** Host for free on GitHub Pages.

---

## 🚀 How to Host (Free via GitHub Pages)

1.  **Create a Repository:**
    * Go to GitHub and create a new repository named `username.github.io` (replace `username` with your actual GitHub username).
    * *Note: If you name it something else (e.g., `my-portfolio`), your site will be at `username.github.io/my-portfolio`.*

2.  **Upload Files:**
    * Upload the `index.html` file to this repository.
    * (Optional) Create a folder named `assets` or `images` and upload your profile picture and project thumbnails there.

3.  **Activate Pages:**
    * Go to Repository **Settings** > **Pages** (in the sidebar).
    * Under **Build and deployment**, ensure **Source** is set to "Deploy from a branch".
    * Select **main** (or master) branch and `/ (root)` folder.
    * Click **Save**.

4.  **Live:** Wait about 1-2 minutes. Your site will be live at `https://username.github.io`.

---

## 🛠 Quick Start

1.  **Download:** Save the `index.html` file to a folder on your computer.
2.  **Images:** Create a folder named `images` next to it. Add your profile photo (e.g., `me.jpg`).
3.  **Run:** Double-click `index.html` to open it in your browser. That's it!

---

## 📝 Content Management

Since there is no database, you manage content by editing the HTML tags directly.

### 1. Profile & Bio
Look for the `` section.
* **Photo:** Change `<img src="...">` to your file path.
* **Name/Role:** Edit the text inside `<h1>` and `<span class="role">`.
* **Socials:** Update the `href="#"` links in the `.socials` div.

### 2. Adding a New Project / Video
Copy the code block below and paste it inside `<div class="grid" id="grid-projects">` (or `#grid-videos`).
**Important:** You must include the class `search-target` for the search bar to find it.

```html
<a href="LINK_TO_PROJECT" class="card search-target">
    <div class="thumbnail">
        <img src="path/to/image.jpg" alt="Project Name">
    </div>
    <div class="card-content">
        <span class="card-title">Project Title</span>
        <p class="card-meta">Tech Stack / Year</p>
        <p class="card-desc">Short description of what you built.</p>
    </div>
</a>