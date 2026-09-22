# Ascolta

La musique qu'on se recommande.

Tu partages un morceau (artiste, titre, un petit mot, et le lien de ta plateforme si tu en as un). Ascolta fabrique un lien qui contient toute la reco. La personne qui l'ouvre voit un bouton vers **sa** plateforme : le lien direct si c'est la même que la tienne, sinon la recherche « artiste + titre ».

- Aucun serveur, aucun compte, aucun service tiers au moment du partage.
- La reco voyage dans le fragment de l'adresse (`#r=…`, JSON compressé en deflate-raw) : il n'est jamais envoyé à GitHub.
- Les recos reçues et envoyées restent sur l'appareil (`localStorage`, clés `ascolta.*`).
- Volontairement sans manifest ni service worker : l'icône de l'écran d'accueil s'ouvre dans Safari et partage les mêmes données que les liens reçus.
- Interface en français et en anglais.

Fichiers : `index.html`, `icon.png` (180×180).
