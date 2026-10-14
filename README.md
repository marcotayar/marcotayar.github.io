# Marco Tayar portfolio

Static portfolio for https://marcotayar.com. No build dependencies.

## Local preview

Run `python3 -m http.server 4173` from this directory and open http://localhost:4173.

## Content

Edit `index.html` for project descriptions, publications, awards, and profile links; edit `style.css` for presentation. Replace `assets/marco-tayar-cv.pdf` when updating the public CV. The supplied CV includes personal contact information and named industrial partners. Review it before each publication.

RAPTOR is a pretrained policy: Marco's contribution here is integration and deployment, not RAPTOR training. LARS 2025 documents separate PPO/SAC research. YouTube links are intentionally omitted until provided.

## GitHub Pages and Cloudflare

Publish the repository root from the `main` branch. `CNAME` sets `marcotayar.com` as the custom domain.

In Cloudflare, create DNS-only A records for `@` pointing to 185.199.108.153, 185.199.109.153, 185.199.110.153, and 185.199.111.153. Create a DNS-only CNAME for `www` pointing to `marcotayar.github.io`. Preserve email records. Replace conflicting website records only.

Verify the domain in GitHub account Settings > Pages using GitHub's supplied TXT record. After DNS validation and certificate issuance, enable Enforce HTTPS in repository Settings > Pages. Check both apex and www URLs.
