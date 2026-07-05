# Jordan Chu — Portfolio Website

A fast, ad-free personal portfolio built with plain HTML and CSS. No frameworks, no build step. Each page is fully self-contained (styling is embedded at the top of every file), so any page looks right even if you open it by itself.

## Files

| File | What it is |
|---|---|
| `index.html` | Main page: about, experience, education, skills, projects, contact |
| `project-brake-caliper.html` | Bike brake caliper project page |
| `project-jack-in-a-box.html` | Jack-in-a-Box simulator project page |
| `project-fsae-undertray.html` | FSAE undertray project page |
| `project-camera-clamp.html` | MRD camera clamp project page |

## How to publish on GitHub Pages (one-time setup, ~10 minutes)

1. Create a free account at **github.com** (if you don't have one).
2. Click the **+** in the top right → **New repository**.
   - Name it exactly: `YOURUSERNAME.github.io` (e.g. `jordanchu.github.io`). Using this name makes your site URL clean.
   - Set it to **Public**, then click **Create repository**.
3. On the new repo page, click **uploading an existing file**, drag in ALL the HTML files from this folder (and this README if you like), and click **Commit changes**.
4. Go to the repo's **Settings → Pages**. Under "Branch," select `main` and click **Save**. (If you named the repo `YOURUSERNAME.github.io`, this may already be enabled.)
5. Wait 1–2 minutes. Your site is live at **https://YOURUSERNAME.github.io** — that's the link for your resume.

## How to make edits later

1. Go to your repository on github.com.
2. Click the file you want to change (e.g. `index.html`).
3. Click the **pencil icon** (top right of the file view).
4. Edit the text — everything on the page is plain, readable text between HTML tags. For example, to update your GE dates, find `Aug 2025 – Present` and change it.
5. Click **Commit changes**. The live site updates in about a minute.

Common edits:
- **Change any text:** just find it in the HTML and type over it.
- **Change the accent color:** each HTML file has the styling embedded near the top inside a `<style>` block — edit `--blue: #235789;` (do it in each of the 5 files, or ask Claude to do it for you).
- **Add a project:** duplicate one of the `project-*.html` files, edit its content, then copy one of the `<a class="card" ...>` blocks in `index.html` and point it at your new file.
- **Add a skill:** in `index.html`, copy a `<span class="skill">...</span>` line and change the name.

## Important: images and resume PDF

The images and resume PDF currently load from your **existing Wix site's storage**. This works fine as long as the Wix site (or at least the Wix account) still exists.

**Before you delete your Wix site**, do this so nothing breaks:
1. Save each image to your computer (right-click → Save Image on your live new site).
2. Create a folder called `images` in your GitHub repository and upload them there.
3. In each HTML file, replace the long `https://static.wixstatic.com/...` URLs with `images/your-file-name.jpg`.
4. Upload your resume as `resume.pdf` to the repository, and in `index.html` change the resume button link to `resume.pdf`.

(You can also ask Claude to do this swap for you — just upload the HTML files and images.)

## Note on the phone number

Your phone number is listed in the contact section (matching your current Wix site). Since this site will be public and linked from your resume, consider whether you want it there — removing it is one line in `index.html`.
