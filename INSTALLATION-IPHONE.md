# SamaBudget PWA v2 — installation iPhone

## Nouveautés
Chaque transaction comporte désormais **Modifier** et **Supprimer**. La suppression demande une confirmation. Les totaux sont recalculés automatiquement.

## Mise en ligne depuis Safari
1. Dans Fichiers sur iPhone, décompresse `SamaBudget-PWA-v2.zip`.
2. Ouvre github.com dans Safari, puis ton dépôt `samabudget-pwa`.
3. Remplace `index.html`, `manifest.webmanifest` et `service-worker.js` à la racine et ajoute les deux images dans `icons/`. Attention à conserver exactement les chemins.
4. Active GitHub Pages dans Settings > Pages > Deploy from a branch > main > /(root), si ce n'est pas déjà fait.
5. Ouvre l'adresse HTTPS de ton site dans Safari, attends la mise à jour et recharge si nécessaire.
6. Dans Safari, touche Partager > Sur l'écran d'accueil > Ajouter. Si déjà installée, ferme puis rouvre l'application après le déploiement.

## Données
Les transactions sont enregistrées localement dans le navigateur sur l'appareil. La version 2 conserve la clé de stockage `samabudget-v1` pour permettre la migration des anciennes transactions **sur la même origine et dans le même contexte de stockage**. Ne supprime pas les données du site et conserve une sauvegarde avant toute réinstallation. Les données ne se synchronisent pas entre appareils ou contextes de stockage.
