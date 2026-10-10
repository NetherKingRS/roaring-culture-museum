# The Roaring Culture Museum

A portable, interactive museum based on the **Roaring Culture (12.7 / AP 21)** focus of the supplied assignment. Plain HTML, CSS, and JavaScript; no installation, build process, API keys, or database required.

## Open it

Open `index.html` in a modern browser. A local web server is preferable for testing YouTube and captions, because file URLs can restrict media integrations. On a published HTTPS website, use the same files without changes.

## What's included

- Six galleries and eighteen clickable exhibits, with evidence prompts and source links.
- Art Deco floor plan, responsive phone layout, keyboard-accessible dialogs, and reduced-motion support.
- Six room challenges, a chronology game, a primary/secondary source game, a passport, and an exportable reflection.
- A separate teacher reference tab with bibliography, objective coverage, WWI connections, and essential-question responses.
- An intentionally empty opening-video slot, completion-based museum entrance, transcript and caption support, and a Video Studio that exports settings.
- A historical photograph and links to genuine archival audio and film players. Archive access requires internet and may depend on school filters. These are linked archival media, not locally bundled recordings.

## Add YOUR video before submitting

1. Open **Video Studio**.
2. Paste a YouTube link (embedding must be permitted), a direct MP4/WebM URL, or `assets/intro.mp4` after putting that file in the assets folder. A Drive sharing page is not a direct video URL.
3. Add your transcript, optional captions (`assets/captions.vtt`), names, and optional student narration (`assets/narration.mp3`). A narrated intro also fulfills the student-narration component.
4. Choose **Preview entrance** to test it.
5. Choose **Download config.js**. Replace the original `config.js` in this folder/repository with the downloaded file, retaining that exact filename, then commit the change.

Preview changes affect only the current page. Downloading a file does not update a hosted website by itself. Do not publish credentials or private sharing tokens. Student names are optional and will be visible if supplied.

The video attempts autoplay. Browsers often require a click for playback with sound. A valid video opens the museum on its `ended` event; YouTube uses the IFrame Player API. After completion, the current browser session remembers that video. Blank configuration shows a labeled preview entrance. An explicit playback-trouble route permits recovery if a school blocks media. This is a learning flow, not anti-cheating enforcement. Seeking is not prevented.

## Upload to GitHub

1. Create an empty repository on GitHub, for example `roaring-culture-museum`.
2. Extract the ZIP. Open its `roaring-culture` folder.
3. Upload the **contents** of that folder into the repository. `index.html` must be at the repository root, alongside `app.js`, `content.js`, `styles.css`, and `config.js`—not inside an extra nested folder.
4. Include `assets`, `vercel.json`, and the hidden `.nojekyll` file (for Pages). Commit the files. This is a file upload, not GitHub's URL-based repository importer.

## Hosting option A: GitHub Pages (simplest for this project)

No second hosting account is needed. For a public repository on GitHub Free:

1. Open the repository's **Settings → Pages**.
2. Under Source, choose **Deploy from a branch**.
3. Choose **main** and **/(root)**, then Save.
4. GitHub displays the site address after deployment, normally `https://YOUR-USERNAME.github.io/roaring-culture-museum/`.

All asset paths are relative, so the repository subpath works. More: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Hosting option B: Vercel

1. Sign into Vercel and add/import a project from this GitHub repository.
2. Choose framework preset **Other**. Keep the repository root as Root Directory.
3. No build or install command is needed. Output Directory is `.` (the repository root); the supplied `vercel.json` declares this.
4. Deploy. Vercel supplies an HTTPS address and can redeploy new GitHub commits.

More: https://vercel.com/docs/git

## Content and assignment notes

`content.js` contains room labels, questions, icon drawings, and source records. All historical claims have exhibit-level citations. The teacher tab distinguishes primary objects from later descriptions and states the limits of historical evidence. Modern icons and the diagram are not represented as archival artifacts.

The original file supplied was a legacy Word `.doc`, despite being described as a PDF. Its focus section and museum requirements were extracted and used as project requirements. Team roles listed in the handout were not assigned automatically.

The site addresses the five culture objectives, at least five representations (18 included), WWI connections, and essential questions C2, A2, and D2. It includes text, subtle animation, games, and linked archival media. **You still need to supply your own introductory video / student narration** as requested, verify your teacher accepts linked archival media, and credit any new media you add. The script in Video Studio is a starting point for your own recording.

## Privacy and accessibility

No accounts, analytics, or server database. Passport and reflection data are stored locally when the browser permits it. Google Fonts, the Library of Congress image, and optionally YouTube contact their respective services. Fonts have local fallbacks. Use the reference tab's Print button for a clean teacher copy.

## Verification

See `VERIFICATION.md` for tested features and external-media limitations.
