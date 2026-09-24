# pse-cadre-public

Révision des règlements européens (CRA, NIS 2, RGPD...), des référentiels nationaux (RGAA, RGS, RGI...) et des publications de la DINUM.

14 modules, consultables depuis l'application de révision
https://guiraudjb.github.io/PSE25-27/ (ce dépôt en fournit les données via GitHub Pages).

## Séries

- **01** : Règlements européens
- **02** : Référentiels nationaux
- **04** : Numérique de l'État : IA, Suite Numérique, gouvernance

## Organisation : un seul dossier pour le jeu et la page web

Tout est dans `batocera/pse-cadre-public/`, le dossier du jeu Batocera, copié tel quel
sur la console. La page web lit les **mêmes** fichiers (via GitHub Pages).

- `batocera/pse-cadre-public/data/` : `modules.json` (liste des modules) et, pour chaque
  module `<nom>` : `fiche/<nom>.txt`, `quizz/<nom>.csv`, `flashcard/<nom>.csv`,
  éventuellement `tp/<nom>.csv`, `icone/<nom>.png`, et les médias
  `podcast/<nom>.mp3`, `infographie/<nom>.png`, `chanson/<nom>.mp3` (+ paroles
  `.txt`), `fiche_audio/<nom>.mp3` (narration de la fiche).
- `batocera/pse-cadre-public/tts_assets/cache/<module>/` : audio des QCM (`quiz_N_ask`,
  `quiz_N_feedback_correct|incorrect`) et des flashcards (`flash_N_recto|verso`),
  joué par le jeu ET par la page web.
- `batocera/pse-cadre-public/*.py`, `pse-cadre-public.pygame`, `jeu.json`, `assets/` : le jeu.

## Outils (`batocera/`)

- `deploy.py` : copie le dossier du jeu sur la Batocera (SMB).
- `generate_tts_voicestudio.py` / `generate_fiche_audio_voicestudio.py` :
  génèrent l'audio (VoiceStudio local) directement dans le dossier du jeu.

Le moteur du jeu est commun à tous les dépôts : il se modifie dans le modèle
de l'espace de travail puis se synchronise, jamais ici.
