# NutriPilot Mobile (PWA)

Application statique pour iPhone/Android, sans serveur ni compte. Les données sont enregistrées localement dans le navigateur (localStorage). **Ne pas ouvrir `index.html` directement depuis l’app Fichiers** : les navigateurs bloquent généralement le chargement des recettes en mode `file://`.

## Mise en ligne gratuite avec GitHub Pages (sans ordinateur)
1. Sur Safari, crée un compte sur https://github.com (si nécessaire).
2. Crée un dépôt **public** nommé `nutripilot-mobile`.
3. Dans le dépôt, utilise **Add file > Upload files** et envoie **tous les fichiers contenus dans le dossier `nutripilot-mobile`**, pas le ZIP. Sur iPhone, si l’upload multiple est difficile, tu peux utiliser l’éditeur web GitHub et créer les fichiers un par un, ou un ordinateur une seule fois.
4. Va dans **Settings > Pages > Build and deployment**, sélectionne **Deploy from a branch**, puis **main / (root)** et sauvegarde.
5. Attends la publication ; l’adresse sera `https://TON_PSEUDO.github.io/nutripilot-mobile/`.
6. Ouvre cette adresse dans Safari sur iPhone, puis **Partager > Sur l’écran d’accueil > Ajouter**.

GitHub Pages est un hébergement statique gratuit selon les conditions de GitHub. Le dépôt public rend le **code** public, mais pas les données enregistrées sur ton iPhone. N’ajoute aucune donnée personnelle au dépôt.

## Tester localement (facultatif)
`python -m http.server 8000` puis ouvrir `http://localhost:8000`.

## Limites de cette version
- 18 recettes avec estimations nutritionnelles et prix indicatifs, pas de prix de supermarché en direct.
- Le générateur ajuste approximativement les portions aux calories, mais **ne garantit pas** l’objectif protéines ni le budget. Les données ne remplacent pas les conseils d’un professionnel.
- La catégorie « sans porc ni alcool » ne certifie pas les ingrédients ou viandes halal.
- Aucune synchronisation : effacer les données Safari ou changer d’appareil peut supprimer les données. Exporter régulièrement une sauvegarde JSON dans Profil.
- L’installation et le mode hors ligne nécessitent d’ouvrir d’abord l’application sur son adresse HTTPS.
