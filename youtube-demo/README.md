# Nova — AI Mentor (demo site)

Public landing page for the YouTube → Patreon funnel. Shows the feature, embeds
the build video, and sends people to Patreon to get the copy-paste prompt.

**Static. No API keys. Safe to be public.**

## Set it up (5 min)

1. Create a **new, empty GitHub repo** (e.g. `nova-demo`).
2. Copy the files from this folder into it.
3. Open `index.html` and edit the three lines at the bottom:
   ```js
   const PATREON_URL = 'https://www.patreon.com/YOUR_HANDLE';
   const YOUTUBE_URL = 'https://youtu.be/YOUR_VIDEO_ID';
   const YOUTUBE_ID  = 'YOUR_VIDEO_ID';
   ```
4. `git push`.
5. On [vercel.com](https://vercel.com) → **Add New → Project** → import the repo → Deploy.
   No build step, no env vars — it's a static site.

## The funnel

```
YouTube video  →  this landing page  →  Patreon (the paid copy-paste prompt)
```

- **Free / public:** this page + the video. It shows the feature and the wow.
- **Paid (Patreon):** the actual prompt (see `PATREON-EP-*.md` in the main repo)
  that builds the feature in one paste.

## Filming tip

Film against your **real** deployed app (the private repo) so the AI actually
talks. This public repo is only the sales page — keep it static so you never
leak an API key.
