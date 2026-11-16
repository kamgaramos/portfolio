# Portfolio – Kamga Christian Ludovic

Site statique (HTML/CSS), sans installation ni dépendance.

Fichiers : index.html (accueil), projets.html, parcours.html, contact.html, portrait.jpg.

## Mettre en ligne

**Netlify (le plus simple)** : va sur https://app.netlify.com/drop et glisse-dépose ce dossier.
**Vercel** : installe Vercel CLI, puis `vercel` dans ce dossier.
**GitHub Pages** : crée un dépôt, envoie ces fichiers à la racine, puis Settings > Pages > Deploy from a branch (main, /root).

Pour tester en local : ouvre index.html dans ton navigateur.

## Sécurité

- Site 100 % statique : aucun script, aucun formulaire, aucune base de données.
- `vercel.json` (Vercel) et `_headers` (Netlify) ajoutent les en-têtes de sécurité : CSP stricte, anti-clickjacking (X-Frame-Options), nosniff, Referrer-Policy, Permissions-Policy, HSTS, COOP/CORP.
- Les pages contiennent aussi une balise CSP (utile sur GitHub Pages, qui ne permet pas d'en-têtes personnalisés).
- Active l'authentification à deux facteurs sur GitHub et Vercel.
