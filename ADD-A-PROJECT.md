# Add a project to the portfolio

This site is a small, static website. Each project has its own page, so you can add a proper case study with a video, photos, and a written explanation. No account or publishing tool is needed to edit the files. When the site is hosted later, include the new page and its media in the same site folder.

## 1. Make a project page

1. Copy `projects/project-template.html` and give the copy a short file name, such as `projects/inductive-sensor.html`.
2. Open the new file in a text editor.
3. Replace the square-bracket prompts with your project title, date, role, tools, challenge, approach, key decisions, results, and what you learned.
4. Update the page title, description, and links near the top and bottom.

The template already has sections for an overview, problem, approach, video, image gallery, outcome, reflection, and references. Remove any section that does not fit your project.

## 2. Add a video

1. Create or use the `assets/videos/` folder.
2. Copy your MP4 video there, for example `assets/videos/inductive-sensor-demo.mp4`.
3. In the new project page, replace the video-slot placeholder with this player and update the file name:

```html
<video controls preload="metadata" poster="../assets/images/inductive-sensor-poster.jpg">
  <source src="../assets/videos/inductive-sensor-demo.mp4" type="video/mp4">
  Your browser does not support embedded video.
</video>
```

The `poster` image is optional. A compressed MP4 keeps the page quicker to load. The site displays the video; it does not upload or store it for you, so keep the video file in the site folder when you publish.

## 3. Add photos or diagrams

1. Copy images into `assets/images/`.
2. In the project page, replace a `gallery-slot` with an image and a caption:

```html
<figure>
  <img src="../assets/images/inductive-sensor-board.jpg" alt="Inductive sensor board on the test bench">
  <figcaption>Prototype board during sensor testing.</figcaption>
</figure>
```

Write alt text that explains what the image shows. Use a useful caption to give context.

## 4. Add it to the portfolio page

In `portfolio.html`, copy one `<article class="portfolio-card">` entry. Change its title, summary, tags, category list, artwork label, and links to point to your new file. Use one or more of these categories in `data-categories` so the filters work:

- `embedded`
- `electronics`
- `research`
- `biomedical`

For example: `data-categories="embedded electronics"`.

You can also update the three featured links on `index.html` when you want the new project on the home page.

## 5. Add a field note

In `journal.html`, copy one `<article class="journal-entry">` and replace the heading and paragraphs. Link the note to your project page so readers can go from the lesson to the full case study.

## File layout

- `index.html` — home page
- `portfolio.html` — categorized project library
- `about.html` — profile, skills, experience, and education
- `journal.html` — written field notes
- `contact.html` — contact links and CV
- `projects/` — individual project case studies and the reusable template
- `assets/videos/` — project videos
- `assets/images/` — project photos, diagrams, and poster frames
