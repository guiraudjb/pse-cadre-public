# pse-cadre-public

Révision des règlements européens (CRA, NIS 2, RGPD...), des référentiels nationaux (RGAA, RGS, RGI...) et des publications de la DINUM.

14 modules, consultables depuis l'application de révision
https://guiraudjb.github.io/PSE25-27/ (ce dépôt en fournit les données via GitHub Pages).

## Séries

- **01** : Règlements européens
- **02** : Référentiels nationaux
- **04** : Numérique de l'État : IA, Suite Numérique, gouvernance

## Contenu par module

Chaque module `<nom>` dispose de : `fiche/<nom>.txt`, `quizz/<nom>.csv`,
`flashcard/<nom>.csv`, éventuellement `tp/<nom>.csv`, et des médias
`podcast/<nom>.m4a`, `infographie/<nom>.png`, `chanson/<nom>.mp3` (+ paroles
`.txt`) et `fiche_audio/<nom>.mp3` (narration de la fiche). La liste des
modules est dans `modules.json`.

## Jeu Batocera

`batocera/pse-cadre-public/` contient le jeu pygame jouable à la manette, déployé par
`batocera/deploy.py`. Le moteur est commun à tous les dépôts : il se modifie
dans le modèle de l'espace de travail puis se synchronise, jamais ici.
