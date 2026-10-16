# Ascolta

La musique qu'on se recommande.

Tu partages un morceau (artiste, titre, un petit mot, et le lien de ta plateforme si tu en as un). Ascolta fabrique un lien qui contient toute la reco. La personne qui l'ouvre voit un bouton vers **sa** plateforme : le lien direct si c'est la même que la tienne, sinon la recherche « artiste + titre ».

- Aucun serveur, aucun compte, aucun service tiers au moment du partage.
- La reco voyage dans le fragment de l'adresse (`#r=…`, JSON compressé en deflate-raw) : il n'est jamais envoyé à GitHub.
- Les recos reçues et envoyées restent sur l'appareil (`localStorage`, clés `ascolta.*`).
- Volontairement sans manifest ni service worker : l'icône de l'écran d'accueil s'ouvre dans Safari et partage les mêmes données que les liens reçus.
- Interface en français et en anglais.

## Calendrier de l'Avent

Menu ⋯ → « Créer mon calendrier de l'Avent ». On remplit 24 cases (même formulaire qu'une reco), un mot d'accueil, son prénom, puis « Partager le calendrier » : un seul lien (`#c=…`) contient les 24 morceaux.

- La personne qui l'ouvre garde le calendrier sur son appareil (`ascolta.cals`) et ouvre une case par jour, du 1er au 24 décembre (date locale de l'appareil).
- Une case ouverte se lit comme une reco : bouton vers sa plateforme, « Ajouter à ma liste ».
- Autant de calendriers qu'on veut : « Pour qui ? » (visible seulement par l'autrice, jamais dans le lien) et « Dupliquer » pour repartir d'un calendrier rempli. Chaque calendrier a son propre lien.
- Morceaux ou albums : le champ « Titre ou album » accepte les deux, on peut mélanger.
- Corriger un calendrier déjà envoyé : renvoyer le nouveau lien ; les cases déjà ouvertes restent ouvertes.
- « Aperçu » montre le calendrier comme les proches le verront. Pour tester un autre jour : `index.html?date=2026-12-05`.
- Le verrouillage est une politesse, pas un coffre : les 24 morceaux sont dans le lien, quelqu'un de très curieux peut les décoder.

Fichiers : `index.html`, `icon.png` (180×180).
