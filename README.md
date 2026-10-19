# Yumi Zhao – personal website

Files: `index.html` (the whole site), `data/site.json` (your editable content), `uploads/` (created automatically when you upload a resume, photo or portfolio file).

## 1. Put it on GitHub (about 5 minutes, no git commands)
1. github.com → **New repository**. Name it exactly `yumi-z.github.io`, set it to **Public**, tick **Add a README**, click Create.
2. In the repo: **Add file → Upload files**. Drag in `index.html` and the `data` folder from the unzipped package (if folders don't drag, upload `index.html` first, then create `data/site.json` with **Add file → Create new file**, name `data/site.json`, paste the contents).
3. Click **Commit changes**.
4. When you are ready to go live: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main / (root) → Save**. After about 1 minute the site is at https://yumi-z.github.io

Until you enable Pages the site is not online. `index.html` contains a `noindex` line that asks search engines to skip it; delete that line when you want to be found on Google.

## 2. Make an editing token (once)
1. GitHub → profile picture → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. Name: `website`. Expiration: the longest allowed. **Repository access → Only select repositories → yumi-z.github.io**.
3. **Permissions → Repository permissions → Contents: Read and write**. Generate, then copy the token (shown only once). Saving it in a password manager or notes app is a good idea; if you lose it, just make a new one.

## 3. Edit your site
Open your site → **🔒 Edit** → paste the token (tick "Remember on this device" if you like) → editing controls appear for: intro text, photo, email, skills, coursework, interests, resume, portfolio. Every change is saved as a commit to your repo; the live site updates after about 1 minute. **🔓 Lock** signs you out and forgets the token.

## Good to know
- The repo is public, so everything you upload (resume, portfolio files) is publicly downloadable. Remove phone number and address from your resume first.
- Keep uploads under about 20 MB. For long videos, upload to YouTube/Bilibili and add the link instead.
- Newly uploaded files may look broken for the first minute while GitHub rebuilds the site.
- Never paste your token into a chat or commit it to the repo.
- To change your name, tagline, GitHub/LinkedIn links or MyAnimeList link, ask Claude to edit `index.html` (the `SITE` block at the top), then upload the new file over the old one.
