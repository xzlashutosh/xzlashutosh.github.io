# Ashutosh Sharma — Portfolio

A static, multi-page engineering portfolio built with HTML, CSS, and a small amount of JavaScript. It is prepared for free hosting with GitHub Pages.

## Pages

- `index.html` — Home
- `portfolio.html` — Project library and category filters
- `about.html` — Profile, skills, experience, education, and awards
- `journal.html` — Field notes and engineering write-ups
- `contact.html` — Contact links and CV
- `projects/` — Individual project case studies and the reusable case-study template

## Publish at `xzlashutosh.github.io`

The GitHub profile linked from the site is `xzlashutosh`, so the matching Pages repository name is `xzlashutosh.github.io`.

1. Create a **public** GitHub repository named `xzlashutosh.github.io`. Leave the “Add a README” option unchecked because this local repository already has one.
2. In the repository settings, open **Pages** and choose **GitHub Actions** under the build and deployment source.
3. From this folder, connect and push the repository:

   ```sh
   git remote add origin https://github.com/xzlashutosh/xzlashutosh.github.io.git
   git push -u origin main
   ```

4. The included workflow publishes the site after each push to `main`. GitHub shows the live address and deployment status under **Settings → Pages** and **Actions**.

GitHub Pages is free for public repositories. Publishing makes the site files public on the internet; review the CV and project media before pushing. See [GitHub’s Pages documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site).

## Add project pages, video, and writing

See [ADD-A-PROJECT.md](ADD-A-PROJECT.md) for the steps to duplicate the project template, add a video and photos, add a project card, and write a field note. Keep large media optimized before adding it to the repository.
