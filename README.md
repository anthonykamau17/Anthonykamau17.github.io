# Anthony Kamau — Portfolio

Personal portfolio: full-stack web platforms (PHP/MySQL) and Android apps (Kotlin).
Plain HTML, CSS and JavaScript — no build step.

| File | What it holds |
|---|---|
| `index.html` | All page content (project write-ups, about, skills) |
| `style.css` | All styling — colours live in the `:root` block at the top |
| `script.js` | **Your links** (top of file) + site behaviour |
| `favicon.svg` / `favicon.ico` | Browser tab icon |

---

## 1. Add your links (2 minutes)

Open `script.js`. At the very top there are two blocks, `LINKS` and `CONTACT`.
Paste each link between the quotes:

```js
foodchap: {
  video: 'https://youtube.com/shorts/AbC123xYz00',
  portrait: true,
  apk: '',
  code: 'https://github.com/USERNAME/foodchap',
},
```

- **Demo videos:** YouTube, Google Drive or Loom share links all work.
  Upload to YouTube as **Unlisted** for the best result — the card then shows the video's thumbnail automatically.
- `portrait: true` is for phone screen recordings (tall video). Use `false` for laptop recordings.
- Leave anything as `''` and its button is hidden, so you never publish a dead link.

## 2. Host it free on GitHub Pages

1. Sign in at github.com → **New repository**.
2. Name it exactly **`USERNAME.github.io`** (your GitHub username) → Public → **Create repository**.
3. On the new repo page click **uploading an existing file**.
4. Drag in **the files inside this folder** (`index.html`, `style.css`, `script.js`, `favicon.svg`, `favicon.ico`, `README.md`) — not the folder itself.
5. Click **Commit changes**.
6. Go to **Settings → Pages**. Under *Build and deployment* set Source = **Deploy from a branch**, Branch = **main**, folder **/ (root)** → **Save**.
7. Wait 1–2 minutes, then open **https://USERNAME.github.io** — that's your live portfolio.

**Updating later:** open the file on GitHub → pencil icon (Edit) → change → **Commit changes**. The site updates in about a minute.

## 3. Optional upgrades

- **Live PHP demos:** GitHub Pages can't run PHP/MySQL. To make CertsVerify or TrailHire clickable,
  host them free on InfinityFree (PHP + MySQL) and paste the URL into `live:`.
- **APK downloads:** in each app's GitHub repo → *Releases* → *Draft a new release* → attach the `.apk` →
  publish, then paste the release link into `apk:`.
- **CV:** put `cv.pdf` in this folder and set `cv: 'cv.pdf'`.
- Put the portfolio link in your GitHub profile, LinkedIn "Featured" section and CV header.

## Adding your project screenshots

The project cards now include labelled screenshot placeholders. To add an image:

1. Put your screenshot files in this `portfolio-final` folder (for example, `images/foodchap-home.png`).
2. In `index.html`, find the relevant `screenshot-placeholder` block.
3. Replace the `<div class="screenshot-placeholder">...</div>` with an image element, for example:

   `<img class="project-shot" src="images/foodchap-home.png" alt="FoodChap home page">`

4. Keep the existing `<figcaption>` text below it, or change it to describe the screenshot accurately.
5. Add the matching `.project-shot` style to `style.css`:

   `.project-shot { display:block; width:100%; aspect-ratio:16/9; object-fit:cover; border-radius:10px; border:1px solid var(--line); }`

Use screenshots from your actual applications. Avoid including real personal data, passwords, private email addresses or confidential records in screenshots.

## Adding your CV

Export your latest CV as a PDF, place it in this folder (for example `Anthony_Kamau_CV.pdf`), then set the `cv` value in the `CONTACT` block near the top of `script.js` to `'Anthony_Kamau_CV.pdf'`.

## Project links

Edit the `LINKS` block near the top of `script.js`. Leave unavailable links as empty strings; the page hides them rather than showing broken buttons. The Android demo videos and GitHub links already present have been retained. The web projects intentionally use screenshots instead of demo-video buttons.


## Adding your Android YouTube demo links

Open `script.js` and find the `LINKS` section near the top. Paste each YouTube URL into the `video` field:

- `foodchap.video` — FoodChap YouTube demo
- `budget.video` — BudgetApp YouTube demo

The “Watch YouTube demo” link appears automatically when a URL is supplied. If the field is empty, it stays hidden. You can use a normal YouTube link, a `youtu.be` link, or a YouTube Shorts link.

## Adding Android app screenshots

Each Android project has two portrait screenshot placeholders:

- FoodChap: Home page; Recipe details
- BudgetApp: Home dashboard; Expense tracking / analytics

Replace each `<div class="screenshot-placeholder">...</div>` in `index.html` with an image element, for example:

`<img class="project-shot" src="images/foodchap-home.png" alt="FoodChap home page">`

Create an `images` folder inside `portfolio-final` and put your screenshot files there. Update the filename and alt text for each image. Keep the existing `<figcaption>` text below each image.

## Adding your profile photo

In `index.html`, find the `profile-photo-slot` inside the **Off the Pitch** section. Replace the `profile-photo-placeholder` div with:

`<img class="profile-photo" src="images/anthony-profile.jpg" alt="Portrait of Anthony Kamau">`

Add your image to the `images` folder using that filename, or change the `src` to match your filename. For best results, use a clear, professional portrait with good lighting and a simple background.

Add this CSS class to `style.css` if you use the image:

`.profile-photo { display:block; width:100%; max-width:260px; aspect-ratio:4/5; object-fit:cover; border-radius:12px; border:1px solid var(--line); }`

## What “Source code” means

“Source code” means the actual project files — for example, the Kotlin/PHP/JavaScript code, layouts, database scripts and other files used to build the application. A GitHub repository link is normally the correct link to share. It lets an employer inspect the code. Your general GitHub profile link is useful too, but ideally each project’s Source code link should point directly to that project's own repository.

## Project screenshots

The project galleries now use consistent framed previews. Website screenshots are shown in landscape frames without cropping, while Android screenshots keep their full portrait shape side by side. To replace an image, keep the filename referenced in `index.html` or update the corresponding `src` path. Captions are editable directly below each image in `index.html`.
