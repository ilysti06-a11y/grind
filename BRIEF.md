# Brief : faire une appli perso « comme Grind »

Copie ce texte dans une nouvelle conversation Claude Code, puis remplace la partie « Ce que je veux cette fois » par ta nouvelle idée.

---

## Le principe

Je veux une petite appli perso pour mon iPhone, du même genre que **Grind** (https://ilysti06-a11y.github.io/grind/, code dans le dépôt GitHub `ilysti06-a11y/grind`). Inspire-toi de ce dépôt pour le style et la technique.

**Grind, c'est :**
- Une web app installable sur l'écran d'accueil (PWA) : Safari, puis Partager, puis « Sur l'écran d'accueil ». Elle s'ouvre en plein écran comme une vraie appli.
- **Onglet Discipline** : un calendrier du mois avec des points lumineux de couleur. Chaque jour, je coche « Oui / Non » pour muscu, cardio et révisions (satisfait ou pas). Il y a la série de jours d'affilée et les totaux du mois. On peut toucher un jour passé pour le corriger.
- **Onglet S2 Biopass** : une liste de chapitres (Biophysique et Biostatistiques) avec une case « Fiche » et une case « ACC » par chapitre, ou par partie de chapitre. En haut, une bulle par tâche (bleue pour les fiches, dorée pour les ACC) qui s'allume quand c'est fait, plus un % global.
- Quand je valide quelque chose, des **petites bulles de couleur éclatent** autour du bouton.

## Technique (à garder)

- **Un seul fichier `index.html`** (HTML + CSS + JS, sans framework), plus `manifest.json`, `sw.js` (service worker pour marcher hors ligne) et des icônes PNG (180, 192 et 512 px).
- **Données sur le téléphone** (`localStorage`). Pas de serveur, pas de compte.
- **Hébergement gratuit avec GitHub Pages** : un dépôt public, branche `main`, dossier racine.
- À chaque mise à jour, **change le numéro de version du cache** dans `sw.js` pour que l'appli se mette à jour quand je la rouvre.
- Pense aux zones sûres de l'iPhone (encoche, barre du bas) : `viewport-fit=cover` et `env(safe-area-inset-*)`.

## Style (à garder)

- **Fond noir bleuté** `#03050a` avec un léger halo bleu nuit en haut. Cases `#0b1122`, bordures `#1b2742`.
- Texte `#e8eefc`, texte secondaire `#7f8db0`.
- **Couleurs d'accent** (palette « Saphir & grenat ») : bleu saphir `#2f5ed8`, bordeaux grenat `#a3274a`, blanc nacré `#e6e8ee`, et l'or `#d4a63c` pour une 2e catégorie.
- Polices : **Sora** pour les titres et **Inter** pour le texte (Google Fonts).
- Coins arrondis, éléments allumés avec un halo (`box-shadow`) de leur couleur, animations rebondissantes.
- Tout en français, sobre, sans emoji dans l'interface.

## Ma façon de travailler

- Avant de coder, montre-moi **plusieurs maquettes visuelles cliquables** pour que je choisisse.
- Pour les couleurs, propose plusieurs palettes, puis des variantes de celle qui me plaît.
- Après chaque changement, mets en ligne et dis-moi simplement de fermer et rouvrir l'appli.
- Explique-moi les étapes GitHub simplement : je suis souvent sur iPhone.

## Ce que je veux cette fois

> (Décris ici ta nouvelle appli : à quoi elle sert, ce que tu veux suivre ou cocher, les onglets, et si tu veux une nouvelle palette ou garder celle-ci.)
