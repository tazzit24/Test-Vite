# Guappo Test (Vite -> GH Pages)

But: repo de test minimal pour vérifier le build Vite + déploiement sur gh-pages.

## Commandes locales
- `npm ci`
- `npm run dev`
- `npm run build`
- `npm run preview`

## Étapes recommandées
1. Crée un nouveau repo de test ou utilise ce dossier local.
2. `npm ci`
3. `npm run dev` puis ouvre `http://localhost:5173`.
4. `npm run build`
5. `npm run preview` pour vérifier le build.
6. Optionnel: modifie `vite.config.js` et règle `base` sur `'/TON_REPO/'` pour GitHub Pages.
7. Commit & push sur GitHub (`main`). L’action GitHub va builder et publier `./dist` sur `gh-pages`.
8. Vérifie ensuite `https://<user>.github.io/<repo>/`.

## Notes
- Pour un test local rapide, laisse `base = '/'`.
- Pour déployer sur GitHub Pages, ajuste `base` vers `'/TON_REPO/'`.
- Si tu veux éviter `gh-pages`, tu peux aussi utiliser un dossier `docs/` sur `main`, mais cela modifie la branche principale.
