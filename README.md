# Marco Tayar portfolio

Static portfolio for https://marcotayar.com. No build dependencies.

## Local preview

Run `python3 -m http.server 4173` from this directory and open http://localhost:4173.

## Content

Edit `index.html` for project descriptions, publications, awards, and profile links; edit `style.css` for presentation. Replace `assets/marco-tayar-cv.pdf` when updating the public CV. The supplied CV includes personal contact information and named industrial partners. Review it before each publication.

RAPTOR is a pretrained policy: Marco's contribution here is integration and deployment, not RAPTOR training. LARS 2025 documents separate PPO/SAC research. YouTube links are intentionally omitted until provided.

The design follows the academic profile/sidebar pattern used by AcademicPages and Arthur Bucker's site: compact masthead, circular portrait and profile links, white background, system sans-serif typography, blue links, and text-led sections. This is a custom static implementation, not a Jekyll/AcademicPages installation. No external fonts or client-side scripts are needed.

Keep the voice personal and factual. Main content order: About me and research interests, Publications, Selected projects, Research & engineering experience, Education, Awards & service, Technical skills & languages, Contact.

The current content and downloadable CV use the user-supplied `assets/marco-tayar-cv1.pdf`. Keep that source file intact. Corrected details include 3D Gaussian-splatting relocalization, warehouse coverage planning and earlier offboard box identification, onboard/simulation VLA baselines, ArduPilot EKF-source switching demonstrated in flight, and leadership of a 40-person SEMEAR team.

## GitHub Pages and Cloudflare

Publish the repository root from the `main` branch. `CNAME` sets `marcotayar.com` as the custom domain.

In Cloudflare, create DNS-only A records for `@` pointing to 185.199.108.153, 185.199.109.153, 185.199.110.153, and 185.199.111.153. Create a DNS-only CNAME for `www` pointing to `marcotayar.github.io`. Preserve email records. Replace conflicting website records only.

Verify the domain in GitHub account Settings > Pages using GitHub's supplied TXT record. After DNS validation and certificate issuance, enable Enforce HTTPS in repository Settings > Pages. Check both apex and www URLs.

## Search and AI discovery

The HTML contains Person, ProfilePage, and ScholarlyArticle JSON-LD. Keep identity links and publication metadata consistent with visible content. `sitemap.xml` lists the canonical home page; section fragments are not separate pages. `robots.txt` permits all crawlers, including search and model-training crawlers. This is public access permission, not a promise of indexing or inclusion in model training.

`llms.txt` is an experimental machine-readable guide; it is not an established Google ranking factor or a guaranteed LLM ingestion mechanism. Update it when changing the portfolio's factual content.

Verify the domain in Google Search Console with its TXT record, submit `https://marcotayar.com/sitemap.xml`, and request indexing of the home page. Import the verified property into Bing Webmaster Tools and submit the sitemap there. Add the canonical site URL to Scholar, ORCID, GitHub, and LinkedIn profiles. Account verification and profile edits require the owner's access.
