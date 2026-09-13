# AspireCompass

**Your Global Opportunity Compass** — an editable, production-ready website for international scholarships, internships, fellowships, exchange programmes, graduate programmes and early-career opportunities.

## Current package

- Exactly 47 public pages, including the homepage
- 23 official-source opportunity records with current status and checked dates
- 15 detailed application and programme guides plus 7 destination guides
- Dedicated Privacy Policy, Terms, Disclaimer and Editorial Policy pages
- Pakistan-focused 2027 scholarship guide and five programme guides
- Search and filter matcher, deadline calendar and category directories
- Responsive desktop, tablet and mobile design
- Original SVG logo and six optimised editorial images
- Per-page titles, descriptions, canonical URLs and keyword targets
- Organization, WebSite, Article, FAQ, Breadcrumb and ItemList structured data
- Dynamic XML sitemap, robots rules and web app manifest
- Contextual internal links, breadcrumbs, related-page modules and primary-source panels
- Custom 404 page and automated build validation

## Run and edit in VS Code

1. Extract the ZIP and open the folder containing `package.json` in VS Code.
2. Open the integrated terminal.
3. Install packages the first time:

   ```bash
   npm install
   ```

4. Start the local development server:

   ```bash
   npm run dev
   ```

5. Open the local URL shown in the terminal (normally `http://localhost:5173`).

The commands are compatible with Windows PowerShell, Command Prompt, macOS and Linux. If `npm install` has already completed, you do not need to run it again after replacing the project with an updated ZIP.

## Create files for GitHub Pages

Run:

```bash
npm run build
```

The build creates a folder named `github-pages`. Upload the **contents inside that folder** to the root of the GitHub Pages repository. It contains all page HTML, browser assets, `CNAME`, `ads.txt`, `robots.txt` and `sitemap.xml`.

Do not upload `node_modules`, `app`, `components`, `lib`, `dist` or the complete source ZIP into the existing published-files repository.

## Where to edit

| Task | File |
| --- | --- |
| Add or update opportunities | `lib/opportunities.ts` |
| Edit original inner pages | `lib/pages.ts` |
| Edit added content, policy and programme guides | `lib/content-enhancements.ts` |
| Change review dates or site URL | `lib/site-config.ts` |
| Edit homepage sections | `app/page.tsx` |
| Edit generated inner-page layouts | `app/[...slug]/page.tsx` |
| Change global design and responsive styles | `app/globals.css` |
| Change header or footer | `components/site-header.tsx`, `components/site-footer.tsx` |
| Replace logo and editorial images | `public/logo.svg`, `public/images/` |
| Review the 47-page SEO plan | `PAGE-MAP.md` |

## Before publishing

- Canonical URLs, schema, sitemap and robots use `https://aspirecompass.org`.
- Keep `public/ads.txt` in place while the AdSense review is active.
- Recheck every listing against its official source; dates, eligibility and funding can change.
- Replace the displayed review date whenever records and guides are genuinely updated.
- The contact address currently remains `hello@aspirecompass.com`, matching the published site. Change it only after an `.org` mailbox or forwarding address is ready.

## Editorial policy

AspireCompass is a discovery and comparison website. It does not award scholarships, accept applications or guarantee selection. Every opportunity should link to a programme-owner source, display a checked date and direct the visitor to verify the current call before applying.
