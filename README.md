# Joshua Foo — research website

A static research website using the compiled stylesheet from
[AcademicPages](https://github.com/academicpages/academicpages.github.io),
with a small custom layout stylesheet. It does not require Jekyll, a package
manager, or a build step.

## Preview and edit

Open `index.html` in a browser. The site's content is in four HTML files:

- **Biography:** edit the text in `<section class="intro">`.
- **Selected publications:** add or edit a `<p>...</p>` entry in the
  `<section class="publications">` section. The Google Scholar link provides
  the complete list.
- **News (`news.html`):** add an `<li><p>...</p></li>` inside the appropriate
  year's list. For a new year, copy a `<details class="news-year">` block,
  change its `<summary>` year, and replace its list entries. The `open`
  attribute makes a year expanded when the page loads.
- **Team (`team.html`):** add or edit a `<figure>` inside the relevant category in
  `<section id="team">`. Place new photos in `assets/images/` and point the
  image's `src` to the new file.
- **Gallery (`gallery.html`):** add a `<figure>` in `<section id="gallery">`.
  Each rectangular preview links to the full photo.
- **Contact:** edit the links in `<section id="contact">`.

The easiest way to add an item is to copy an existing similar entry and
change its text and links. Keep the HTML tags around it. Layout and typography
are in `assets/css/site.css`. After editing, refresh the local page to check
the result; changes do not become public until you upload them to your host.
The source Carrd site was last updated on 21 August 2026.

## Publish with GitHub Pages

1. Create a GitHub repository named `<username>.github.io` for a site at
   `https://<username>.github.io/`, or use a repository of any name for a
   project site.
2. Upload the contents of this folder to the repository root, including
   `index.html`, `assets/`, and `LICENSE-AcademicPages.txt`.
3. In repository Settings → Pages, select **Deploy from a branch**, select
   the default branch and `/ (root)`, and save. GitHub will display the URL
   after the deployment completes.

After publishing, you can update text directly on GitHub: open `index.html`
in the repository, click the pencil icon, make your changes, then choose
**Commit changes**. GitHub Pages will rebuild automatically. To add photos,
use **Add file → Upload files** in the `assets/images` folder, then update
the relevant image path in `team.html` or `gallery.html`. Allow a few minutes for changes to
appear, and refresh the published page.

The navigation and profile sidebar appear in each HTML file. If you change
their content, update all four files to keep the pages consistent. The social
logos in `assets/icons/` are Simple Icons, distributed under the license in
that folder.

The AcademicPages/Minimal Mistakes stylesheet is distributed under the MIT
license in `LICENSE-AcademicPages.txt`. Photographs and biographical content
were migrated from the existing Carrd site and are not covered by that
stylesheet license.
