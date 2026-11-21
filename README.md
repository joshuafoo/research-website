# Joshua Foo — research website

A static research website using the compiled stylesheet from
[AcademicPages](https://github.com/academicpages/academicpages.github.io),
with a small custom layout stylesheet. It does not require Jekyll, a package
manager, or a build step.

## Preview and edit

Open `index.html` in a browser. It contains the site's content:

- **Biography:** edit the text in `<section class="intro">`.
- **Selected publications:** add or edit a `<p>...</p>` entry in the
  `<section class="publications">` section. The Google Scholar link provides
  the complete list.
- **News:** add an `<li><p>...</p></li>` inside the appropriate year's list in
  `<section id="news">`; add a new year heading and list when needed.
- **Team:** add or edit a `<figure>` inside the relevant category in
  `<section id="team">`. Place new photos in `assets/images/` and point the
  image's `src` to the new file.
- **Gallery:** add a `<figure>` in `<section id="gallery">`. Each circular
  preview links to the full photo, so readers can see the uncropped image.
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
the relevant image path in `index.html`. Allow a few minutes for changes to
appear, and refresh the published page.

The AcademicPages/Minimal Mistakes stylesheet is distributed under the MIT
license in `LICENSE-AcademicPages.txt`. Photographs and biographical content
were migrated from the existing Carrd site and are not covered by that
stylesheet license.
