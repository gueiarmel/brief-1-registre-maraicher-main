# Registre des opérations maraîchères

> Projet individuel du SAS DFS, brief 1 (sujet : [SUJET.md](SUJET.md)). Remplacez chaque ✏️ par votre texte, puis supprimez cette ligne.

## Contexte

✏️ *En cinq à huit phrases : qui utilise l'outil (son métier, son geste professionnel), son besoin, ce qu'il saisit, ce que le programme lui affiche, ce que l'outil ne fait pas.*
ContexteLa personne qui utilise l'outil est la responsable d'une exploitation maraîchère pédagogique. Dans son travail quotidien, elle observe les parcelles, identifie les cultures et les interventions réalisées, puis note la date et les dépenses correspondantes. Le programme lui permet de saisir ces opérations dans un terminal à l'aide d'un identifiant, d'une date, d'une parcelle, d'une culture, d'un type d'opération et d'un coût en FCFA. Elle peut ensuite afficher le registre, rechercher une opération ou filtrer les interventions par parcelle et par culture. Elle peut aussi trier les opérations et obtenir le total des dépenses, leur répartition par parcelle ainsi que les coûts minimum et maximum. Les données sont conservées dans un fichier JSON afin de rester disponibles après la fermeture du programme. L'outil est un registre de suivi des interventions et des dépenses : il ne calcule ni les rendements, ni les revenus, ni la rentabilité de l'exploitation.

## Prérequis et lancement

- Node.js 20 ou plus récent, Git ; aucune bibliothèque à installer.

```bash
git clone https://github.com/gueiarmel/brief-1-registre-maraicher.git
cd brief-1-registre-maraicher
node app.js
npm test
```

Sous PowerShell, si `npm` est bloqué : `npm.cmd test`.

## Fonctionnalités

✏️ *Cochez seulement ce qui marche : `- [x]`.*

- [x] Données lues et enregistrées dans `donnees/operations.json`
- [x] Ajouter une opération, saisies invalides refusées sans arrêter le programme
- [x] Lister les opérations, message si le registre est vide
- [x] Rechercher par identifiant ou par parcelle ; filtrer par culture
- [x] Trier par coût ou par date
- [x] Synthèse : total, nombre et total par parcelle, coût minimum et maximum
- [x] Bonus : supprimer et modifier une opération (choix 6 et 7)
- [x] Bonus : tri par coût décroissant, parcelle la plus coûteuse

## Données

✏️ *Le fichier, le nombre d'opérations, les champs (voir [docs/dictionnaire-donnees.md](docs/dictionnaire-donnees.md)), les unités. Rappelez qu'elles sont fictives.*
Le fichier donnees/operations.json contient dix opérations fictives. Chaque objet comprend un identifiant unique (id), une date (date), une parcelle (parcelle), une culture (culture), une intervention (operation) et un coût (coutFCFA). Les coûts sont exprimés en francs CFA (FCFA) et les dates au format AAAA-MM-JJ.Avec les données de départ, le total des dépenses est de 40 000 FCFA : P1 totalise 15 500 FCFA, P2 9 500 FCFA et P3 15 000 FCFA. Le coût minimum est de 1 500 FCFA et le maximum de 8 000 FCFA

## Limites

✏️ *Au moins trois. Par exemple : le registre enregistre des dépenses, pas les revenus, il ne mesure donc pas la rentabilité.*
Le registre contient des dépenses, mais pas les revenus : il ne permet donc pas de calculer la rentabilité.- Il ne stocke pas les quantités récoltées, les surfaces cultivées ou les rendements.- Il ne vérifie pas la cohérence agronomique entre une parcelle et une culture ; par exemple, une culture peut être associée à une parcelle sans contrôle de référence.- Les données de départ sont fictives et ne décrivent pas une exploitation réelle.

## Documents

[Dictionnaire des données](docs/dictionnaire-donnees.md) · [Tâches](docs/taches.md) · [Relevé des tests](docs/releve-tests.md) · [Journal de recherche](docs/journal-recherche.md) · [Fiche agronomique](docs/fiche-agronomique.md) · [Fiche individuelle](docs/fiche-individuelle.md)

## Auteur

✏️ *Prénom NOM, compte GitHub. Entraide : avec qui, sur quoi.*
 Dinasson Deneclin Armel GUEI, https://github.com/gueiarmel Une assistance pédagogique par IA a été utilisée pour comprendre les consignes. YAO YAMOIN MARIE JEANNE, Daly Marie Manuella et Kamagaté junior dans la comprehension du sujet et la correction des erreurs sur certaines lignes de codes.