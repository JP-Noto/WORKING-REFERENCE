# SEAL : le scellé · la décision de service prouvable

Fiche opérationnelle. **Domicile normatif : [SPEC § 6, règles Z1–Z4](../SPEC.md#6-scellé--règles-z)** ;
ce document explique, illustre et borne, il ne redéfinit pas.

## Le problème, en trois phrases

Un système qui décide et sert sans trace ne peut être ni audité ni réfuté : quand une dérive apparaît,
personne ne sait quand elle a commencé ni ce qui a été servi ce jour-là. Les voisins qui certifient
leurs décisions (logs de décision des moteurs de politique, raisons d'évaluation des feature flags)
certifient des politiques et de la configuration, sans piste chaînée ([journal
d'antériorité](../research/prior-art-2026-08-11.md)) ; le service d'une référence de production, lui,
reste sans preuve. Sans cette preuve, la falsification du corpus entier est désarmée.

## L'idée, en une image

Le même geste que les dés certifiés : chaque tirage chaîné à son prédécesseur, vérifiable après coup —
le sort prouvable. Le scellé applique ce geste à la décision de service : quel appel (et son working
state), quel état de la constante, ce qui a été servi, la règle qui l'a décidé. Une piste, pas des
reçus épars.

## Les questions que la pratique a posées, et les réponses

**« Le scellé va ralentir le travail ? »** Non par construction : il constate, il n'autorise pas (Z3).
Un scellé qui bloque une livraison n'est plus un scellé, c'est un verrou, et un contrôle qui
conditionne la progression a déplacé l'autorité.

**« On peut consigner en fin de séance ? »** Non (Z2). Un journal reconstruit après coup enregistre ce
qu'on croit avoir décidé ; le scellé enregistre ce qui a été décidé, dans l'instant du geste. C'est la
différence entre une preuve et un souvenir.

**« À quoi bon, si personne ne lit les scellés ? »** Ils ne se lisent pas, ils s'opposent : le jour où
une instance diverge, la piste dit quand, sur quel état, par quelle règle. Sans scellé, le service
fonctionne : il ne fait pas preuve (Z4).

## Les règles (SPEC § 6)

- **Z1.** Toute décision d'instanciation émet un scellé : appel, état de la constante, servi, règle.
- **Z2.** Consigné dans l'instant, chaîné au précédent.
- **Z3.** Le scellé constate, il n'autorise pas.
- **Z4.** Sans scellé, le service sert mais ne fait pas preuve.

## Les pièges

- **Le scellé-verrou** : transformer la pièce d'audit en gate de progression (Z3) : c'est la dérive que
  toute la famille interdit.
- **Le scellé-souvenir** : écrit le soir, il certifie la mémoire de l'auteur, pas la décision (Z2).
- **L'infrastructure** : si sceller exige de construire un système, la SPEC en demande trop : la
  primitive existe (la piste chaînée des dés), on la réutilise, on ne la réinvente pas — règle que le
  corpus s'impose.

## En pratique

La primitive tourne : la piste chaînée SHA-256 des dés certifiés de THE LOOP, en usage réel depuis le
2026-07-07. Le scellé d'instanciation est le même geste sur un autre objet : transposition non
implémentée à ce jour, et le corpus le dit.

**Ce que ça change** : « pourquoi ce service ? » a une réponse datée et chaînée, et la branche de mort
n° 1 (la dérive sans détection) devient instrumentable.

---

*JP Noto · WORKING REFERENCE · [CC BY-NC-SA 4.0](../LICENSE.md). Domicile canonique : <https://github.com/JP-Noto/WORKING-REFERENCE>.*
