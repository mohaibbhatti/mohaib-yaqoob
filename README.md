# Mohaib Yaqoob – Portfolio

A static site (plain HTML, CSS and JavaScript). There is no build step.

## Files in this folder

| File | What it does |
|---|---|
| `index.html` | The whole portfolio |
| `Mohaib_Yaqoob_CV.pdf` | Your CV. The "Download CV" button points to this exact file name |
| `og-image.png` | Preview image shown when the link is shared on LinkedIn, WhatsApp, X |
| `vercel.json` | Security headers and clean URLs |
| `robots.txt`, `sitemap.xml` | Help Google find the page |

---

## Option A: GitHub + Vercel dashboard (recommended, no terminal needed)

1. **Create a GitHub repository.** Go to github.com/new. Name it `mohaib-yaqoob`, set it to Public, leave "Add a README" unticked, and click Create repository.
2. **Upload the files.** On the new empty repo page, click "uploading an existing file". Drag in all six files from this folder (not the folder itself). Click Commit changes.
3. **Sign in to Vercel.** Go to vercel.com and choose Continue with GitHub.
4. **Import the repo.** Click Add New > Project. Under Import Git Repository, find `mohaib-yaqoob` and click Import. If it is not listed, click "Adjust GitHub App Permissions" and allow access to that repository.
5. **Set the project name.** On the configure screen, set Project Name to `mohaib-yaqoob`. This gives you `https://mohaib-yaqoob.vercel.app`.
6. **Leave the build settings alone.** Framework Preset: Other. Build Command, Output Directory and Install Command stay empty. Root Directory stays `./`.
7. **Click Deploy.** It takes under a minute. Open the domain Vercel shows you.
8. **Test it.** Check the Download CV button, the contact buttons, dark mode, and press Ctrl+K (or Cmd+K on Mac).

### If your URL is different
Vercel may give you another address (for example if the name is taken). Then:
1. Use find and replace for `mohaib-yaqoob.vercel.app` in `index.html`, `robots.txt` and `sitemap.xml`.
2. Commit the changes on GitHub. Vercel redeploys automatically.
3. Update the portfolio link in your CV to the same address.

### Updating the site later
Edit a file on GitHub (pencil icon) or upload a new version, then commit. Vercel redeploys within a minute. To change the CV, upload a new PDF with the same name `Mohaib_Yaqoob_CV.pdf`.

---

## Option B: Vercel CLI (terminal)

```bash
npm install -g vercel
cd path/to/this/folder
vercel login
vercel          # first run: accept the defaults; name the project mohaib-yaqoob
vercel --prod   # publish to your production URL
```

---

## After it is live

- Add the link to your LinkedIn profile (Contact info > Website) and to your GitHub profile.
- Paste the link into LinkedIn's Post Inspector (linkedin.com/post-inspector) to refresh the preview card.
- Optional: connect your own domain in Vercel under Project > Settings > Domains.
