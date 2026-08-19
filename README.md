# Pupvision 📺

A retro CRT-TV web app that "changes channels" through a set of AI-generated dog VHS covers.

## Files

```
pupvision/
├── index.html
├── images/
│   ├── jaws.jpg
│   ├── the-dogfather.jpg
│   ├── e-t.jpg
│   ├── bark-to-the-future.jpg
│   ├── star-paws.jpg
│   ├── home-alone.jpg
│   ├── spider-pup.jpg
│   ├── titanic.jpg
│   ├── jurassic-bark.jpg
│   ├── ghostbusters.jpg
│   ├── indiana-bones.jpg
│   ├── the-muttrix.jpg
│   ├── pup-fiction.jpg
│   ├── top-gun.jpg
│   └── mission-impawsible.jpg
└── README.md
```

Everything is plain static HTML/CSS/JS — no build step, no dependencies to install.

## Deploy to GitHub Pages (free)

1. Create a new repository on GitHub (e.g. `pupvision`).
2. Upload the contents of this folder to the repo root — `index.html`, the `images/` folder, and this README all need to sit at the top level (not nested inside another folder).
   - Easiest way: on the repo page, click **Add file → Upload files**, then drag in `index.html` and the whole `images` folder.
3. Go to **Settings → Pages** in the repo.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
6. Wait a minute or two — GitHub will give you a URL like:
   ```
   https://yourusername.github.io/pupvision/
   ```

That's it — no build process, since it's already plain HTML/CSS/JS.

## Other free hosting options

If you'd rather not use GitHub Pages, any of these work the same way (just drag-and-drop the folder, no config needed):

- **Netlify Drop** — https://app.netlify.com/drop (literally drag the folder onto the page)
- **Vercel** — https://vercel.com (import the GitHub repo, or drag-and-drop via their dashboard)
- **Cloudflare Pages** — https://pages.cloudflare.com (connect the GitHub repo)

## Editing

- To change or reorder channels, edit the `CHANNELS` array near the bottom of `index.html`. Each entry is `{ "title": "...", "src": "images/filename.jpg" }`.
- To add a channel: drop a new image into `images/` and add a matching entry to the array.
- Channel titles that are very long may get truncated on the VFD readout on small screens — keep them under ~20 characters if possible.
