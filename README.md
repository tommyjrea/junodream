[README.md](https://github.com/user-attachments/files/26375662/README.md)
# junodream website

Official website for junodream. Static site hosted on GitHub Pages.

## Setup

1. Create a new GitHub repository (e.g. `junodream.github.io` or `junodreamband.com`)
2. Push all files from this folder to the repository
3. Go to **Settings → Pages** and set source to `main` branch
4. If using a custom domain (`junodreamband.com`), add it in the Pages settings and create a `CNAME` file or configure your DNS

## Adding Album Artwork

Replace the placeholder SVG files in `images/artwork/` with your actual artwork images (JPG or PNG recommended). Update the file extensions in `music.html` accordingly:

- `images/artwork/pools-of-colour.jpg`
- `images/artwork/the-beach-20.jpg`
- `images/artwork/death-drive-20.jpg`
- `images/artwork/travel-guide.jpg`
- `images/artwork/isnt-it-lovely.jpg`
- `images/artwork/galactica.jpg`
- `images/artwork/to-the-moon.jpg`

When replacing, update the `.svg` extension to `.jpg` (or `.png`) in `music.html`.

## Custom Domain (DNS)

To point `junodreamband.com` to GitHub Pages:

1. Add a `CNAME` file to the repo root containing: `junodreamband.com`
2. At your domain registrar, add these DNS records:
   - `A` record → `185.199.108.153`
   - `A` record → `185.199.109.153`
   - `A` record → `185.199.110.153`
   - `A` record → `185.199.111.153`
   - `CNAME` for `www` → `yourusername.github.io`

## Structure

```
├── index.html          # Homepage (background image + nav)
├── live.html           # Tour dates via Songkick embed
├── music.html          # Album artworks + listen links
├── videos.html         # YouTube video embeds
├── store.html          # Coming soon placeholder
├── signup.html         # Drip mailing list signup form
├── style.css           # All styles
├── fonts/
│   └── Alte-Haas-Grotesk.woff
├── images/
│   ├── bg-desktop.png  # Homepage background (desktop)
│   ├── bg-mobile.png   # Homepage background (mobile)
│   └── artwork/        # Album artwork images
└── CNAME               # Custom domain config
```
