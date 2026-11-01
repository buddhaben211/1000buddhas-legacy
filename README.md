# 1000buddhas.co — legacy static copy

A static snapshot of the WordPress version of 1000buddhas.co, taken Nov 1, 2026 so the site could leave the old 1000-Buddhas-2025 droplet. It holds the domain until the new agency site replaces it.

- Made with `wget --mirror --page-requisites --convert-links --adjust-extension` on the droplet, then cleaned up:
  - WordPress shortlinks (`/?p=1234`) now point to the matching page;
  - asset files that had `?ver=` in their names were renamed (`?` → `_`), with references updated;
  - absolute links to 1000buddhas.co were made site-relative.
- WordPress-only features don't work here: the contact form, search, comments, and anything else that needs PHP.
- Hosted on DigitalOcean App Platform as a static site. Pushing to `main` deploys.
- The original WordPress files and database are archived separately.
