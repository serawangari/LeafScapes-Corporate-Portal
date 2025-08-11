# Vercel Wrapper for ArcGIS Experience Builder (v2)

This static site shows your ArcGIS Experience under **your** domain using a full-screen iframe.

## Quick start
1) Open `config.js` and set:
   ```js
   window.EXPERIENCE_URL = "https://experience.arcgis.com/experience/YOUR_APP_ID/";
   window.PAGE_TITLE = "Corporate Signup"; // optional
   ```
2) Deploy to Vercel
   - **GitHub:** push these files to a repo → Vercel → New Project → Deploy
   - **CLI:** `npm i -g vercel` → `vercel` → `vercel --prod`
3) Add a custom domain in **Vercel → Project → Settings → Domains**, then create the DNS CNAME to `cname.vercel-dns.com`.
4) Visit `https://apps.yourdomain.com/corporate-signup/`

## Notes
- The Experience must be shared appropriately and embeddable.
- Sign-in flows work inside the iframe.
- If your Experience loads custom services from your domain and you see CORS issues, add your domain as an allowed origin in ArcGIS Online Org Settings.
