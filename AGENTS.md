# APKP website maintenance

Production: https://apkp.pl/ on LH.pl; upload only public/ through the existing GitHub Actions workflow.
Preserve original logos and the approved red-white design.
Whenever inline scripts in public/index.html change, recompute their SHA-256 CSP hashes in public/.htaccess (including JSON-LD). Keep script/style/image policy compatible with the page. Do not disable CSP as a shortcut.
Keep sitemap.xml limited to actual canonical pages. Update organization structured data only with verified facts. Search Console verification requires the user's real verification token; never invent one.
After security changes verify live HTTP status, redirects, security headers, assets, robots.txt, sitemap.xml and a missing URL. Do not block legitimate search-engine crawlers.
