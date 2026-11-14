# hetznerhof.de – statische Website (GitHub Pages)

## Veröffentlichen
1. Neues GitHub-Repo anlegen (z. B. `hetznerhof-website`, öffentlich) und den gesamten Inhalt dieses Ordners hochladen (inkl. `CNAME` und `.nojekyll`).
2. Repo → Settings → Pages → Source: „Deploy from a branch“, Branch `main`, Ordner `/ (root)`.
3. Custom domain: `hetznerhof.de` → speichern. Nach der DNS-Umstellung „Enforce HTTPS“ aktivieren.

## DNS bei WordPress.com (Domains → hetznerhof.de → DNS-Einträge)
- Löschen: A `@` → 23.227.38.65 und CNAME `www` → shops.myshopify.com (Shopify)
- Hinzufügen: vier A-Einträge für `@`:
  185.199.108.153 · 185.199.109.153 · 185.199.110.153 · 185.199.111.153
- Hinzufügen: CNAME `www` → `<dein-github-name>.github.io`
- NICHT anfassen: MX (smtp.google.com), TXT google-site-verification, TXT _domainconnect, NS

## Noch offen
- Impressum und Datenschutz sind Entwürfe – vor Livegang prüfen/vervollständigen.
- Headline-Schrift „Sailors“ ist eine Lizenzschrift: Datei als `assets/fonts/sailors-regular.woff2` ablegen, dann wird sie automatisch verwendet (bis dahin Poppins).
