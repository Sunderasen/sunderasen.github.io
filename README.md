# Sunderasen — Cloud Operations Portfolio

A responsive, single-page portfolio for Cloud Operations, SRE, DevOps, and Platform Engineering opportunities.

The website is intentionally built as one self-contained `index.html` file. No framework, package installation, or build command is required.

## Files to upload to GitHub

```text
index.html
README.md
favicon.svg
Sunderasen_Resume.pdf
```

- `index.html` contains the complete website, styling, and interactions.
- `README.md` is this editing guide.
- `favicon.svg` is the small portfolio icon shown in browser tabs.
- `Sunderasen_Resume.pdf` is the resume opened by the Resume links.

## Quick editing workflow

1. Open `index.html` in VS Code or another text editor.
2. Use **Find** (`Ctrl+F` on Windows/Linux or `Cmd+F` on macOS).
3. Search for the existing text or URL shown in the tables below.
4. Replace only the value you want to change.
5. Save the file and open `index.html` in a browser to verify it.
6. Commit and push the updated file to GitHub.

You can also edit through GitHub: open `index.html` in the repository, click the pencil icon, make the change, and commit it.

## Clickable links

Search for the current URL or email in `index.html` and replace every relevant occurrence.

| Item | Search for | Replace with |
| --- | --- | --- |
| Resume | `https://sunderasen.github.io/Sunderasen_Resume.pdf` | The URL or filename of your new PDF |
| LinkedIn | `https://www.linkedin.com/in/sunderasen2002/` | Your updated LinkedIn URL |
| GitHub | `https://github.com/Sunderasen` | Your updated GitHub profile URL |
| Email address | `sunderasen.p@zohomail.in` | Your new email address |

The resume URL currently appears in the navigation, hero section, and Career Opportunities section. Replace all occurrences if the resume location changes.

### Updating the resume PDF

The easiest option is to keep the same filename:

```text
Sunderasen_Resume.pdf
```

Replace the old PDF in the repository with the updated PDF. If you rename it, update all resume URLs in `index.html` too. Filenames are case-sensitive on GitHub Pages.

### Adding a new button or link

Use this pattern for a link that opens in a new tab:

```html
<a class="btn"
   href="https://example.com"
   target="_blank"
   rel="noopener noreferrer">
  Button text ↗
</a>
```

Use this pattern for a page section link:

```html
<a href="#experience">Experience</a>
```

The value after `#` must match a section's `id`, such as:

```html
<section id="experience">
```

## Common content changes

### Hero introduction

Search for:

```text
Keeping systems available when it matters.
```

The paragraph immediately after it is the main professional introduction.

### Operations console

Search for any of these unique phrases:

```text
focus --production
objective --next-role
20K+
K8s
AWS
200+
```

Edit the visible text between the HTML tags. Avoid removing the surrounding tags and class names.

### Experience

Search for:

```text
Zoho Corporation
Tabtree IT Consulting
```

Each experience entry contains the role, company, dates, summary, and responsibility cards.

### Skills

Search for the skill name you want to change, such as:

```text
GitHub Actions
Kubernetes
Prometheus
Nginx
```

Individual skill labels use this structure:

```html
<span>Kubernetes</span>
```

To add a skill, copy one complete `<span>...</span>` item and change its text.

### Career Opportunities section

Search for:

```text
05 / Career opportunities
```

This section contains the email, View Resume, LinkedIn, and GitHub actions.

## Colors and themes

The dark-theme colors are defined near the top of `index.html` in the first `:root` block.

The light-theme colors are defined in:

```css
html[data-theme="light"] { ... }
```

Important color variables:

| Variable | Purpose |
| --- | --- |
| `--bg` | Main page background |
| `--surface` | Cards and panels |
| `--surface2` | Nested cards |
| `--line` | Borders and dividers |
| `--text` | Main text |
| `--muted` | Secondary text |
| `--accent` | Green highlights and primary buttons |
| `--teal` | Secondary highlight color |

Change the color values, but keep the variable names. Test both themes after editing.

## Page title and search description

Search near the top of `index.html` for:

```html
<title>Sunderasen | Cloud Operations · SRE · DevOps</title>
```

The `<meta name="description">` line controls the summary that search engines and link previews may use.

## Favicon

The browser-tab icon is stored in:

```text
favicon.svg
```

To replace it, keep the new file in the same folder as `index.html`. If you use a different filename or file format, update this line in `index.html`:

```html
<link rel="icon" type="image/svg+xml" href="favicon.svg">
```

For example, a PNG favicon would use:

```html
<link rel="icon" type="image/png" href="favicon.png">
```

Favicons are often cached strongly by browsers. After replacing one, hard-refresh the site or test in a private window.

## Preview before publishing

For simple edits, double-click `index.html` to open it in a browser. Check:

- Desktop and mobile widths.
- Dark and light modes.
- Resume, LinkedIn, GitHub, and email links.
- Spelling and employment dates.
- Long text for wrapping or overflow.

Browser developer tools can simulate mobile screens. In Chrome or Edge, press `F12` and select the device toolbar.

## Publish with GitHub Pages

1. Upload or commit `index.html`, `README.md`, `favicon.svg`, and `Sunderasen_Resume.pdf` to the root of the `Sunderasen/sunderasen.github.io` repository.
2. Open the repository's **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Choose the `main` branch and the `/ (root)` folder.
5. Save and wait for the GitHub Pages deployment to finish.
6. Open `https://sunderasen.github.io/` and hard-refresh the page.

GitHub Pages updates can take a few minutes. If an old version remains visible, use `Ctrl+Shift+R` or `Cmd+Shift+R`.

## Safe-editing tips

- Keep a backup before larger changes.
- Change visible text and URLs without deleting surrounding HTML tags.
- Keep quotation marks around every `href` value.
- Do not remove the `<style>` or `<script>` blocks.
- Avoid pasting formatted text from Word; use plain text.
- Test both themes and all links after every change.

## Current contact links

- Email: [sunderasen.p@zohomail.in](mailto:sunderasen.p@zohomail.in)
- LinkedIn: [linkedin.com/in/sunderasen2002](https://www.linkedin.com/in/sunderasen2002/)
- GitHub: [github.com/Sunderasen](https://github.com/Sunderasen)
- Portfolio: [sunderasen.github.io](https://sunderasen.github.io/)

