# NutriPilot Coach V3 — iPhone / GitHub Pages

## Nouveautés V3
- Programme musculation sur cycle de **4 semaines** : semaine 1 volume, 2 variations, 3 intensité, 4 récupération active. Changement automatique chaque lundi, avec aperçu de la semaine suivante.
- **Illustrations SVG locales** par type de mouvement (schémas simplifiés, pas des démonstrations biomécaniques). Fonctionnent hors ligne.
- Historique de séances, charges et répétitions conservé. Les charges initiales sont des exemples et doivent être adaptées.
- Menus sur 7 jours et recettes, journal alimentaire, eau, poids, dashboard, sauvegarde JSON.
- L'algorithme nutritionnel varie selon la semaine lors de la **nouvelle génération** de menus. Les menus déjà enregistrés ne sont pas modifiés automatiquement.

## Installation depuis un iPhone
1. **Sauvegarde tes données** dans l'ancienne application : Réglages > Exporter mes données.
2. Décompresse le ZIP et transfère **tous les fichiers ET le dossier `illustrations/`** à la racine du dépôt GitHub existant. Remplace les anciens fichiers, sans supprimer `illustrations/`.
3. Vérifie GitHub Pages : Settings > Pages > Deploy from a branch > main > /(root).
4. Attends la publication, ouvre ton site dans Safari et actualise-le. Si l'ancienne version reste affichée, ferme puis rouvre la PWA après quelques minutes.
5. Les données sont stockées uniquement sur l'appareil dans `localStorage` (`nutripilot-v1`). Pas de compte ni synchronisation.

## Limites importantes
- Les images sont des **illustrations stylisées par catégorie**, pas des photos ni tutoriels techniques exercice par exercice.
- Les notifications ne fonctionnent que quand l'application est ouverte. Pas de push en arrière-plan sans infrastructure serveur.
- Pas d'IA conversationnelle : coach algorithmique avec programme périodisé.
- Les valeurs nutritionnelles et les prix sont approximatifs.
- En cas de douleur, fatigue inhabituelle ou reprise après maladie, réduire les charges et consulter un professionnel si nécessaire.

## Test local
`python -m http.server 8000` puis ouvrir `http://localhost:8000`.
