# Météo sur Kobo Nia (navigateur intégré)

La page `index.html` affiche la météo (données Open-Meteo, gratuites et sans clé) et se recharge toute seule toutes les heures.

## 1. Mettre la page en ligne

La Kobo doit pouvoir ouvrir la page par une adresse web. Le plus simple et gratuit : **GitHub Pages**.

1. Crée un compte sur https://github.com (si tu n'en as pas).
2. Clique sur **New repository**, nomme-le par exemple `meteo`, coche **Public**, puis **Create repository**.
3. Clique sur **uploading an existing file**, glisse `index.html`, puis **Commit changes**.
4. Va dans **Settings → Pages**. Sous *Branch*, choisis `main` et `/ (root)`, puis **Save**.
5. Après une à deux minutes, la page est disponible à :
   `https://TON-PSEUDO.github.io/meteo/`

## 2. Choisir sa ville

Ajoute la ville à la fin de l'adresse :

- `https://TON-PSEUDO.github.io/meteo/?ville=Lyon`
- ou, plus précis : `https://TON-PSEUDO.github.io/meteo/?lat=45.76&lon=4.84&nom=Lyon`

Sans paramètre, c'est Paris. Tu peux aussi changer la ville par défaut dans le bloc `REGLAGES` en haut du script.

## 3. Sur la Kobo

1. **Désactiver la mise en veille :** Paramètres → Économie d'énergie et confidentialité → *Mise en veille automatique* → **Jamais** (et *Extinction automatique* → **Jamais**).
2. **Ouvrir le navigateur :** Plus (☰) → Paramètres → **Fonctions bêta** → *Navigateur web* → Démarrer.
3. Tape l'adresse de ta page.
4. Ajoute-la en favori pour la retrouver facilement.

## Bon à savoir

- **Batterie :** l'écran e-ink ne consomme presque rien, c'est le Wi-Fi qui use la batterie. Pour un affichage permanent, laisse la liseuse branchée.
- **Wi-Fi coupé :** si la Kobo coupe le Wi-Fi, la page affiche « Météo indisponible » et réessaie toute seule toutes les 5 minutes.
- **Rafraîchissement :** il est réglé à 60 minutes (`rafraichissementMinutes` dans le script). La page se recharge aussi automatiquement une fois par heure, même si le script plante.
