# Marco Tayar portfolio

Static portfolio for https://marcotayar.com. No build dependencies.

## Local preview

Run `python3 -m http.server 4173` from this directory and open http://localhost:4173.

## Content

Edit `index.html` for project descriptions, publications, awards, and profile links; edit `style.css` for presentation. Replace `assets/marco-tayar-cv.pdf` when updating the public CV. The supplied CV includes personal contact information and named industrial partners. Review it before each publication.

RAPTOR is a pretrained policy: Marco's contribution here is integration and deployment, not RAPTOR training. LARS 2025 documents separate PPO/SAC research. YouTube links are intentionally omitted until provided.

Keep the voice personal and factual: the opening uses Marco's name and field description, and section headings use direct labels rather than promotional taglines.

Page order: name and field description, a two-paragraph About introduction, Projects, Publications, Research interests, Awards & service, Experience & education, Contact. Keep the experience timeline separate from the short introduction.

## GitHub Pages and Cloudflare

Publish the repository root from the `main` branch. `CNAME` sets `marcotayar.com` as the custom domain.

In Cloudflare, create DNS-only A records for `@` pointing to 185.199.108.153, 185.199.109.153, 185.199.110.153, and 185.199.111.153. Create a DNS-only CNAME for `www` pointing to `marcotayar.github.io`. Preserve email records. Replace conflicting website records only.

Verify the domain in GitHub account Settings > Pages using GitHub's supplied TXT record. After DNS validation and certificate issuance, enable Enforce HTTPS in repository Settings > Pages. Check both apex and www URLs.

## Search and AI discovery

The HTML contains Person, ProfilePage, and ScholarlyArticle JSON-LD. Keep identity links and publication metadata consistent with visible content. `sitemap.xml` lists the canonical home page; section fragments are not separate pages. `robots.txt` permits all crawlers, including search and model-training crawlers. This is public access permission, not a promise of indexing or inclusion in model training.

`llms.txt` is an experimental machine-readable guide; it is not an established Google ranking factor or a guaranteed LLM ingestion mechanism. Update it when changing the portfolio's factual content.

Verify the domain in Google Search Console with its TXT record, submit `https://marcotayar.com/sitemap.xml`, and request indexing of the home page. Import the verified property into Bing Webmaster Tools and submit the sitemap there. Add the canonical site URL to Scholar, ORCID, GitHub, and LinkedIn profiles. Account verification and profile edits require the owner's access.
