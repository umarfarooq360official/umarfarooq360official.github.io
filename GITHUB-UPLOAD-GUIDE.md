# AspireCompass: Simple Update Process

## 1. First-time setup

Open this project folder in VS Code, then run:

```powershell
npm install
```

## 2. Open the website locally

```powershell
npm run dev
```

Open the local address shown in the terminal, normally `http://localhost:5173`.

## 3. Edit the source

- Homepage: `app/page.tsx`
- Opportunities: `lib/opportunities.ts`
- Normal page content: `lib/pages.ts`
- Four expanded guides recovered from the live site: `lib/live-guide-overrides.ts`
- New long-form pages, FAQs and source panels: `lib/content-enhancements.ts`
- Site URL and genuine review date: `lib/site-config.ts`
- Global styling: `app/globals.css`
- Images and logo: `public/images` and `public/logo.svg`
- AdSense authorization: `public/ads.txt`

## 4. Build upload-ready files

Stop the development server with `Ctrl + C`, then run:

```powershell
npm run build
```

Wait until the terminal says:

```text
GitHub Pages package ready: github-pages (47 public pages)
```

## 5. Upload to GitHub

Open the generated `github-pages` folder. Upload **everything inside it** to the root of the current GitHub Pages repository.

Do not upload the `github-pages` folder as one nested folder. Its `index.html`, `ads.txt`, `CNAME`, `robots.txt`, `sitemap.xml`, page folders and asset folders must remain at the repository root.

Do not upload `node_modules` or the complete editable-source folder into the published-files repository.

## Important AdSense protection

Never remove or change this file unless Google gives a new publisher line:

```text
public/ads.txt
```

The build automatically includes it in `github-pages/ads.txt`.

The generated `github-pages` folder also contains the current sitemap, robots rules, consent-ready privacy disclosures and a proper 404 page. Upload the complete contents together so these files stay in sync.
