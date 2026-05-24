# Highland Laundromat — Website

A static website for Highland Laundromat at 283 Highland Ave, Malden, MA.

## File Structure

```
/
├── index.html          ← the main page
└── images/             ← all photos used on the site
    ├── interior-1.jpg
    ├── lg-washers.jpg
    ├── dryers.jpg
    ├── giant-washers.jpg
    ├── logo-window.jpg
    ├── storefront.jpg
    └── ... etc.
```

## How to deploy to GitHub Pages

1. Create a new repository on GitHub (you can name it anything, e.g. `highland-laundromat`).
2. Upload **every file in this folder** (the `index.html` AND the entire `images/` folder) to the repository.
3. Go to the repo **Settings → Pages**.
4. Under **Source**, select branch `main` and folder `/ (root)`. Click **Save**.
5. Wait a minute. GitHub will give you a live URL like `https://<your-username>.github.io/<repo-name>/`.

## Pointing your custom domain (highlandlaundromat.com or similar)

1. In **Settings → Pages**, scroll to **Custom domain**, enter your domain (e.g. `highlandlaundromat.com`), click **Save**.
2. At your domain registrar (where you bought the domain), add these DNS records:
   - **A records** pointing to GitHub Pages' IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - Or, if you want `www.highlandlaundromat.com`, add a **CNAME** record pointing to `<your-username>.github.io`.
3. Wait for DNS to propagate (anywhere from a few minutes to a couple hours).
4. Back in GitHub **Settings → Pages**, check the **Enforce HTTPS** box once it becomes available.

## Editing the site

- Open `index.html` in any text editor (VS Code, Notepad++, even TextEdit).
- All content (text, prices, hours link) is right in that one file — search for the words you want to change.
- Want to swap a photo? Just replace the file inside `/images/` with the same filename, or change the `src=""` reference in the HTML.

## Notes

- The Google Business link points to a Google Maps search for the laundromat. Once your business is verified on Google, the link will go directly to your listing where customers can see hours, reviews, and directions.
- Phone number used: (978) 979-7063 — update inside `index.html` (search for it) if you'd prefer a different number on the site.
