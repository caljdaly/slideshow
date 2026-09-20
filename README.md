# Neo-Futurism Board viewer

A photo viewer for Notion that pages through every image in the `images/` folder of this repo.

## One-time setup (about 5 minutes)

1. On github.com, click **New repository**. Name it something like `board-viewer`, keep it **Public**, and create it.
2. Click **Add file → Upload files**. Drag in `index.html`, `README.md`, and the `images` folder (with its `.gitkeep` inside). Click **Commit changes**.
3. Go to **Settings → Pages**. Under *Build and deployment*, set Source to **Deploy from a branch**, pick **main** and **/ (root)**, then **Save**.
4. After a minute or two the page is live at `https://YOUR-USERNAME.github.io/board-viewer/`. Open it once to check.
5. In Notion, type `/embed`, paste that URL, and drag the block to the size you want.

## Adding photos

Open the `images` folder on github.com, click **Add file → Upload files**, drop in the pictures, commit. The viewer picks them up the next time it opens (it checks the folder at most every 10 minutes).

Photos are shown in filename order, so name them `001.jpg`, `002.jpg`, … if you want a specific sequence. PNG, JPEG, GIF, WebP and AVIF work. Keep each file under a few MB so the embed loads fast.

## Saving pins from Pinterest

Open a pin, right-click the image, **Save image as…**. For a whole board at once, a bulk-download browser extension is much quicker than doing them one by one.

## If you use a custom domain

Open `index.html` and set `repo: 'YOUR-USERNAME/board-viewer'` in the `CONFIG` block near the top of the script.
