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

## Deploy to GitHub Pages

 GitHub URL
   ```
   https://mjin8.github.io/pupvision/
   ```

That's it — no build process, since it's already plain HTML/CSS/JS.

## Editing

- To change or reorder channels, edit the `CHANNELS` array near the bottom of `index.html`. Each entry is `{ "title": "...", "src": "images/filename.jpg" }`.
- To add a channel: drop a new image into `images/` and add a matching entry to the array.
- Channel titles that are very long may get truncated on the VFD readout on small screens — keep them under ~20 characters if possible.
