# SERVING : le service · servi, jamais chargé

Fiche opérationnelle. **Domicile normatif : [SPEC § 5, règles S1–S4](../SPEC.md#5-service--règles-s)** ;
ce document explique, illustre et borne, il ne redéfinit pas.

## Le problème, en trois phrases

Charger le corpus en bloc coûte, dilue, et pondère mal ce qui compte ; demander à la main dépend de la
mémoire de l'opérateur. Les deux cassent en silence quand le corpus grossit : le premier par
saturation, le second par oubli. Il faut que la délivrance soit un contrat écrit, pas un réflexe.

## L'idée, en une image

La doctrine du template, devenue règle de service : l'information légère, au bon moment, dans le bon
contexte. Chaque élément de la couche porte son contrat de chargement — *quand il monte, à quel appel,
sous quelle condition*, comme une cartouche de jeu porte « quand elle monte en RAM ». Et chaque
élément servi garde son fil vers sa source : on peut toujours remonter certifier.

## Les questions que la pratique a posées, et les réponses

**« Rien de plus, rien de moins — comment on tient les deux ? »** Par le contrat (S4) : le « rien de
plus » interdit le chargement par peur, le « rien de moins » interdit à l'appel de quémander ce que son
working state appelle déjà. Si l'appel doit redemander, c'est le contrat qui est faux : corrigez le
contrat, pas l'appel.

**« Une synthèse servie, ça ne va pas diverger ? »** Si elle perd son lien vers la constante, si : une
copie sans source diverge toujours (S3). Le service sert des pointeurs habillés, jamais des orphelins.

**« Le service peut-il s'outiller d'une recherche ? »** Oui : l'outil peut chercher, mais la décision
de servir reste la règle (I1). La similarité peut proposer ; elle n'admet pas.

## Les règles (SPEC § 5)

- **S1.** La référence se sert ; le corpus entier ne monte jamais.
- **S2.** Exactement l'instanciation décidée : rien de plus, rien de moins.
- **S3.** Tout élément servi reste relié à sa source dans la couche.
- **S4.** Le contrat de chargement est écrit, jamais improvisé à l'appel.

## Les pièges

- **Le service par peur** : monter « au cas où », c'est reconstruire le chargement en bloc un élément à
  la fois (S1, S2).
- **La copie orpheline** : une synthèse sans lien source semble identique le jour du service ; elle
  ment trois semaines plus tard (S3).
- **Le contrat oral** : « d'habitude on monte ça » n'est pas un contrat ; ce qui n'est pas écrit se
  improvise, et ce qui s'improvise dérive (S4).

## En pratique

Le cas vivant est le contrat de chargement des cartouches de THE LOOP — chaque section porte son
« quand elle monte en RAM », l'univers ne monte jamais en bloc, les secrets vivent en need-to-know
(doctrine du template, validée au conteneur : statut éditorial, pas un rang du pipeline).

**Ce que ça change** : le coût d'un appel se prédit en lisant les contrats, pas en pesant le corpus,
c'est la propriété I4, et elle se mesure.

---

*JP Noto · WORKING REFERENCE · [CC BY-NC-SA 4.0](../LICENSE.md). Domicile canonique : <https://github.com/JP-Noto/WORKING-REFERENCE>.*
