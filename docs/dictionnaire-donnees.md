# Dictionnaire des données

> Un champ par ligne, d'après `SUJET.md` et le fichier de `donnees/`. La première ligne sert de modèle.

| Champ | Signification | Type | Règle de validation | Unité | Exemple |
| `id` | Identifiant unique | texte | non vide, absent des données | Texte(majuscule) | `O03` |
| `date` |Date de l'operation |texte |date reelle existante |AAAA-MM-JJ | `2026-11-04` |
| `parcelle` |surface delimité |obligatoire non vide | |texte |`p1` |
| `culture` |plante cultivee sur la parcelle |texte |obligatoire non vide |Texte(miniscule) | `tomate`|
| `oprration` | Intervention humaine | texte | Liste fermee uniquement | une des 5 valeurs | `arrosage` |
| `coutFCFA` |depense enregidtree | number| nombre>=0|francs cfa |`3000`|

**Listes de valeurs autorisées** : OPERATIONS['semis', 'arrosage' , 'desherbage' , 'repiquage', 'recolte']

**Sources** : SUJET.md et donnees/operations.json
