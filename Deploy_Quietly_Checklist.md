
# Deploy Quietly — GitHub Pages or Netlify

## 🧭 Overview
This checklist guides your future site deployment once your QuietSite_Blueprint is complete.  
It keeps your **learning vault public-facing**, while protecting **personal reflections** and anything not meant for SEO.

---

## 🌐 GitHub Pages (Jekyll easiest)
1. Create a new GitHub repository named `jenn-quiet-notes`.
2. Copy your **jekyll/** folder contents from QuietSite_Blueprint to the repo root.
3. Add your study folders — e.g., `AI_Data_CySA_Track`, `HTB_JuniorAnalyst`, and `CIAT_Portfolio`.
4. Commit and push your changes.
5. In the repository:
   - Go to **Settings → Pages**
   - Under “Build and deployment,” select **Branch:** `main`, **Folder:** `/ (root)`
6. Wait 1–3 minutes for GitHub Pages to build your site.
7. Visit your published URL (it will look like `https://jennshagrin.github.io/jenn-quiet-notes`).
8. Verify `robots.txt` works correctly — open `https://.../robots.txt` and confirm `/Personal_Reflections` is disallowed.

---

## ☁️ Netlify (Hugo / Quartz / Jekyll compatible)
1. Log into [Netlify](https://www.netlify.com/).
2. Click **“Add new site → Import an existing project.”**
3. Connect your GitHub repository or drag-and-drop your project folder.
4. Choose your build command:
   - **Hugo:** `hugo`
   - **Jekyll:** `jekyll build`
   - **Quartz:** `npm install && npm run build`
5. Set your **publish directory:**
   - Hugo → `public`
   - Jekyll → `_site`
   - Quartz → `public`
6. Deploy your site. Netlify will generate a `.netlify.app` preview URL.
7. Confirm your robots.txt appears correctly and your reflections folder is blocked.

---

## 🔎 Lite SEO Tips
- Include the **meta_snippets.html** file in your site’s `<head>` section.
- Use **frontmatter tags** like `WomenInCyber`, `BlueTeam`, `CrumpledThoughts`, and `CIAT` for discoverability.
- Add an **About** page that explicitly references:
  - *Women in Cybersecurity*
  - *AI & Data Literacy*
  - *Nonprofit Tech Education (Crumpled Thoughts)*  
  This helps search engines understand your intent.
- Keep tone educational, reflective, and professional.

---

## 🧱 Maintenance & Privacy
- Run `jekyll serve` or `hugo server` locally to preview updates.
- Update robots.txt if you add new private folders.
- Consider publishing under a **custom domain** later (optional).
- Review your SEO footprint every 3–6 months to confirm indexing is still limited to approved folders.

---

### ✅ Final Check Before Publishing
- [ ] Public folders only (`AI_Data_CySA_Track`, `HTB_JuniorAnalyst`, `CIAT_Portfolio`)
- [ ] `/Personal_Reflections` fully excluded
- [ ] Meta tags added to all public pages
- [ ] About page finalized
- [ ] Verified via online robots.txt validator

---

**Quiet means intentional.**  
You’re not hiding — you’re curating visibility with purpose.
