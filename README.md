# Diceplacement Adventures Dungeon — version 3D (web)

Jouable dans le navigateur avec GitHub Pages : https://padsauce.github.io/Diceplacements-dungeon/

Les règles du livret Paper App DUNGEON (impair en diagonale, pair en ligne droite, six étages jusqu'à la Salle du Trésor), dans un donjon en 3D vu de dessus, légèrement en plongée. Le rendu est gravé à la plume en noir et blanc et éclairé par la torche du héros.

Trois modes de jeu :

- **Partie rapide** : 5 étages tirés au hasard. Plus de PV, partie terminée. Score = PV + pièces + objets non utilisés.
- **Normal** : 50 étages, toujours les mêmes, jusqu'à la Salle du Trésor. Une mort ajoute une tombe et on continue. Score = pièces + PV + objets − 10 par tombe.
- **Sans fin** : des étages au hasard, de plus en plus durs, jusqu'à la mort. Score = 10 par étage terminé + pièces + objets.

Chaque mode a son classement local et une sauvegarde à part. Des trophées se débloquent en jouant.

## Installer sur un téléphone

Le jeu s'installe comme une appli depuis le lien ci-dessus, sans store. Il marche ensuite hors connexion.

- **Android** (Chrome, Edge, Samsung Internet) : bouton « Installer sur mon téléphone » dans le menu du jeu, ou menu ⋮ puis « Installer l'application ».
- **iPhone / iPad** : bouton Partager, puis « Sur l'écran d'accueil », puis « Ajouter ». Le jeu installé a sa propre mémoire : les profils de Safari n'y sont pas repris.

## Technique

- Tout le jeu est dans `index.html` (HTML, CSS et JavaScript). `manifest.webmanifest`, `sw.js` (cache hors connexion) et `icons/` en font une web app installable. Les polices viennent de Google Fonts et le moteur 3D de Three.js 0.160.0 (jsDelivr).
- Profils, sauvegarde et classement restent dans le navigateur du joueur. Aucune base de données.
- Le jeu Unity est développé dans un autre dépôt, privé.
