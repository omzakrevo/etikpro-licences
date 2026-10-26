# Licences ETIKPRO

Fichier lu par l'application ETIKPRO pour vérifier les licences :
`https://raw.githubusercontent.com/omzakrevo/etikpro-licences/main/licences.json`

- Ce dépôt doit rester **public** (l'application le lit sans identifiant).
- Il ne contient que l'**empreinte SHA-256** des clés : aucune clé n'est lisible ici.

## Ajouter / modifier une licence

1. Ouvrez la page d'administration (`admin.html`, ou https://omzakrevo.github.io/etikpro-licences/ si GitHub Pages est activé).
2. « Nouvelle licence » → la page donne la **clé** (à remettre au client) et un bloc JSON.
3. Ici sur GitHub : `licences.json` → ✏️ → collez le bloc dans la liste `"licences"` (virgule entre deux blocs) → **Commit changes**.

Pour **prolonger** : modifiez `"expire"`. Pour **suspendre** : `"actif": false`.
Pour **limiter à certains appareils** : ajoutez leurs identifiants dans `"appareils"` (affichés dans l'app, écran licence ou Réglages).

Les applications appliquent le changement à leur prochaine ouverture (quelques minutes de cache GitHub possibles).
