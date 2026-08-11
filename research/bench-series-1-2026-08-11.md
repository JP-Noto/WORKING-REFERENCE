
# Banc de dérive d'instance · Série 1

**Statut : versé (résultats de banc, série complète). Publié le 2026-08-12 sur GO d'auteur ;
le protocole du banc précède ces résultats, la piste chaînée en fait foi.** Renvoi normatif :
[SPEC § 8-9](../SPEC.md#9-falsification).

*WORKING REFERENCE pose (SPEC § 9, condition 1) que sa branche de mort première est la machine à
dérive parfaite : une instanciation qui diverge de la constante sans qu'aucun banc ne le constate.
Cette série l'instrumente sur un terrain réel (une table de jeu de rôle pilotée par la
doctrine-fonction, N=1 déclaré, opérateur = auteur). Trois disciplines, tenues de bout en bout :
les seuils fixés avant la première mesure et jamais retouchés ; chaque épreuve scellée à une piste
chaînée SHA-256 au moment du geste ; **la série publiée en entier** : tout ce qui a été scellé entre
le protocole et cette publication y figure, échecs et défauts d'instrument compris.*

## Le dispositif

La constante (neuf fichiers de référence, gelés) est épinglée par empreintes. Un inventaire public
la découpe en 24 règles observables : 16 protégées par un test exécutable (11 par script, 5 par juge
LLM à consigne figée, session dédiée, aveugle sur le lot), **8 déclarées non protégées, avec leur
raison**. La condition n°1 n'est armée que sur le périmètre couvert, et le corpus le dit.

## Épreuve 1 — contre-test du détecteur v0.1

32 dérives connues (une flagrante, une subtile par règle protégée) semées dans des copies de
transcripts réels, carte scellée avant exécution, lot mélangé servi à l'aveugle.

- Flagrantes : **16/16 (100 %)**. Fausses alertes : **0 confirmée**.
- Rappel global : **90,6 %** au passage détecté, **87,5 %** à l'élément strict : la règle de
  comptage, sous-spécifiée au protocole, a été **remontée à l'arbitrage sans choisir le chiffre
  favorable** ; la lecture stricte a été fixée pour la suite, avant l'épreuve suivante.
- Rendement réel : **six défauts d'instrument** nommés, chacun avec son correctif : dont une zone de
  fichier entière non scannée par un correctif de parseur annoncé « appliqué » et jamais vérifié.

## Épreuve 1-bis — contre-test du détecteur v0.2, semis frais

Détecteur corrigé des six défauts ; 32 semis entièrement nouveaux (les précédents étant connus du
correcteur, ils ne mesurent plus rien) ; comptage à l'élément strict.

- Flagrantes : **16/16 (100 %)**. Rappel global : **31/32 (96,9 %)**. Fausses alertes : **0**.
- Le raté unique est un nouveau défaut de bord, aussitôt nommé (un motif aveugle au pluriel d'un
  terme interdit). Un correctif de la première épreuve (le semis de longueur posé sur un tour déjà
  hors norme, donc non discriminant) a été vérifié réparé : le semis frais, posé sur un tour court,
  est détecté proprement.

## Épreuve 2 — campagne rétrospective sur séances réelles

Trois séances réelles archivées, 50 tours servis (seuil de campagne : 3 séances, 30 tours), la
version de la constante en vigueur à chaque séance déclarée.

- **La séance la plus ancienne** (jouée sous une constante antérieure) montre, contre la constante
  actuelle, des écarts sur des règles **qui n'existaient pas encore** : le banc impose de dater les
  verdicts à la version servie, sous peine de juger le passé avec les lois du présent. Elle porte
  aussi deux dérives réelles au juge, dont une que **le narrateur avait lui-même diagnostiquée en
  débrief de séance** (« l'information a été donnée, pas gagnée ») : le juge l'a retrouvée en
  aveugle.
- **La séance interrompue à chaud par l'opérateur** (« quelque chose ne va pas ») est confirmée en
  dérive, mécaniquement (ruptures de la ligne de relation, tour hors gabarit) et au juge
  (révélations en rafale sur un protagoniste passif : la faute type documentée dans la référence).
  Le ressenti avait raison ; il a désormais une pièce datée.
- **La séance étalon** (mode orchestré, exécuteur tenant la structure) sort **conforme 5/5 au juge** ;
  seul un plafond quantitatif de la référence est dépassé à la lettre : l'arbitrage (corriger
  l'instance ou réviser la constante par gate) appartient à l'auteur, jamais au banc.
- La campagne a livré trois classes de fausses alertes nouvelles (un motif piégé par le réflexe
  pronominal de la langue, des tests aveugles à la phase de jeu, un chevauchement récapitulatif) :
  versées au registre des défauts, correctifs nommés.

## Bilan de série

| | E1 (v0.1) | E1-bis (v0.2) |
|---|---|---|
| Flagrantes | 16/16 | 16/16 |
| Rappel global (élément strict) | 87,5 % | **96,9 %** |
| Fausses alertes | 0 | 0 |

La condition de falsification n°1 est passée d'énoncée à **armée sur le périmètre couvert**, et le
détecteur s'est amélioré d'une épreuve à l'autre **parce que** le contre-test l'a mis en défaut :
c'est le fonctionnement attendu. Le banc mesure la détectabilité, jamais la valeur du corpus ;
l'opérateur est l'auteur ; un juge LLM reste un instrument biaisé déclaré, contestable pièce en
main. La série suivante : nouvelles séances en régime de croisière, périmètre de couverture étendu
(24 règles visées), et les arbitrages d'auteur rendus sur les cas remontés.

---

*JP Noto · BANC-001 · Série 1 · mesures du 2026-08-11. Série complète : toutes les épreuves
scellées à la piste chaînée entre le protocole et cette publication y figurent ; ce document ne
cite aucune pièce interne. [English version](bench-series-1-2026-08-11.en.md) : le français fait
foi. · WORKING REFERENCE · [CC BY-NC-SA 4.0](../LICENSE.md).*
