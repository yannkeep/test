Maintenant je comprends tout. La structure du dataset est complètement différente de ce que j'avais prévu. Je réécris avec un import qui mappe EXACTEMENT cette structure.Je réalise qu'il y a probablement un problème avec la sauvegarde en IndexedDB. Laissez-moi renforcer le code et ajouter des safeguards.Version corrigée avec :

**Import amélioré :**
- Mapping COMPLET de tous les champs du dataset
- `arbre.causes[]` → string avec bullets
- `swot.strengths` → `swot.forces` 
- `pestel.politique` → `pestel.p`
- `pourquoi.why1` → `pourquoi.p1`
- `cibles.principale` → `cibles.principales`
- `smart.s/m/a/r/t` → `text/indicator/deadline`
- Logs de debug dans la console (F12)

**Calcul stats révisé :**
- VOIR: 10 champs → domino(3) + profil(4) + fleur(3)
- JUGER: 26 points → 22 champs + bonus acteurs (max 4)
- AGIR: 20 points → 15 champs + bonus smart/journal (max 5)

Avec le dataset complet, ça devrait donner **~95-100%** au lieu de 14%.

Ouvre la console (F12) après import pour voir les détails du mapping.
