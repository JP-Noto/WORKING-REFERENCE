# Filiation & sources · WORKING REFERENCE

**Version 0.1 · 2026-08-11 · statut : proposé.**

Cette doctrine n'invente pas ses primitives : elle **nomme une fonction** que quatre objets internes
dessinaient séparément, et que l'industrie pratique par morceaux sous d'autres noms. Ce fichier
rapporte chaque mécanisme à ses antériorités connues, internes et externes. **Antériorité n'est pas
influence** : la passe d'antériorité externe (gate #030, 2026-08-11) est postérieure à la formulation
des mécanismes ; les convergences sont rapportées parce que l'honnêteté l'exige. Le journal d'antériorité
adversarial est versé — [research/prior-art-2026-08-11.md](research/prior-art-2026-08-11.md) : pièces
décisives sur textes originaux, verdicts et limites déclarés. Assumer la filiation ne dilue
pas la contribution : la **réunion sous une seule fonction** et ses trois apports (WHITEPAPER § 8) sont
la contribution.

Convention par mécanisme : **primitive connue → source datée → recontextualisation → apport.**

## La lignée interne

```text
DOCTRINE DU TEMPLATE (pratique constatée 2025, formalisée le 2026-07-11)
  l'information légère, au bon moment, dans le bon contexte ;
  le contrat de chargement par section ; la fiche reliée à sa source
        │
[LIVING REFERENCE](https://github.com/JP-Noto/LIVING-REFERENCE) (2026, public depuis le 2026-08-06)
  la couche épistémique : le statut (proposition → validation → référence),
  fenêtre + invariants, la consignation qui fait preuve (S8),
  les tests de dérive ; cas fondateur : SLIDING CANON —
  référence maîtresse · fenêtre · déclencheur de révision
        │
THE LOOP 2.0 (juillet–août 2026) — le banc vivant
  les dés certifiés : CSPRNG + piste chaînée SHA-256 (2026-07-07) ;
  le kernel gelé + modules just-in-time (en jeu le 2026-08-07) ;
  le mode orchestré B-i : le need-to-know décidé par appel
  (8/8 conformes le 2026-08-10) ; LA RÉGIE v0.1, l'instanciateur
        │
DÉPÔT #032 (2026-08-11) — la convergence nommée
  la doctrine-fonction : constante + variables, décidée, servie, scellée ;
  verdict d'auteur le jour même, H(T) au registre (rév. 16),
  WORKING REFERENCE fondé
```

## Constante & variables ([SPEC règles C](SPEC.md#3-constante--règles-c))

**Interne.** La séparation référence/instance de LIVING REFERENCE : l'autorité d'un côté, la
restitution située de l'autre. « Le template est immuable, l'instance versionne » (doctrine du
template, règle 4, validée le 2026-07-11). Le kernel gelé de THE LOOP (en jeu le 2026-08-07) : la
constante gelée en partie, tout le reste en modules.

**Externe (passe #030).** Les **design tokens** : la constante en tokens, instanciée par plateforme ;
spécification du W3C Community Group (DTCG), première version stable octobre 2025 : vérifiée sur
l'annonce officielle ([journal](research/prior-art-2026-08-11.md)). Le principe *single source of
truth*. Rien de revendiqué.

**Apport.** Le test d'admission C4 (la survie au changement de génération de modèle comme critère)
et la gate comme seule porte d'entrée : l'épistémologie en amont de la structure (apport c).

## Instanciation ([SPEC règles I](SPEC.md#4-instanciation--règles-i))

**Interne.** SLIDING CANON : le déclencheur de révision : la décision d'output selon le travail en
cours, déjà dans le cas fondateur. Le mode orchestré B-i : la décision d'instanciation mécanisée,
8/8 appels conformes le 2026-08-10. LA RÉGIE v0.1 : la couche qui sert le canon à la table.

**Externe (passe #030).** Le **RAG** et la mémoire étagée : l'instanciation par récupération, critère :
la similarité. Le **headless CMS** : l'instanciation par canal. Rien de revendiqué.

**Apport.** La décision pilotée par l'**état du travail en cours** (ni similarité, ni canal) réglée
sans jugement d'auteur à l'appel (apport a).

## Service ([SPEC règles S](SPEC.md#5-service--règles-s))

**Interne.** La doctrine du template, source directe : chaque section porte son contrat de chargement —
« quand elle monte en RAM » : dans le TEMPLATE-CARTOUCHE de THE LOOP ; l'univers ne monte jamais en
bloc, les secrets vivent en need-to-know. H(Q) au registre (2026-08-10) : « le canon servi plutôt que
chargé », cas particulier déjà inscrit.

**Externe.** Le headless CMS (passe #030). Les acquis du plan de l'inférence (fenêtre glissante,
éléments épinglés, rappel explicite, coût borné) sont crédités au LINEAGE de LIVING REFERENCE
(StreamingLLM, MemGPT) : **acquis de famille, non re-revendiqués ici**.

**Apport.** Le couple S2 (« rien de plus, rien de moins ») + S4 (le contrat écrit dans la couche) comme
règles invocables, et la propriété I4 qui en découle, mesurable.

## Scellé ([SPEC règles Z](SPEC.md#6-scellé--règles-z))

**Interne.** Les dés certifiés de THE LOOP — CSPRNG local + piste chaînée SHA-256, en usage réel depuis
le 2026-07-07 : la primitive du scellé, réutilisée, jamais reconstruite : règle que le corpus
s'impose. S8 de LIVING REFERENCE : la consignation qui fait preuve — Z4 en est le miroir. Le principe
frère : l'autorité vérifiable se tient hors du modèle (note d'atelier du 2026-08-10, fiche au savoir du
conteneur). La garde « constate et alerte, n'autorise pas » : héritée de la famille (MYSTANCE, M2).

**Externe.** Le constat en creux de la passe #030 (« aucun voisin ne certifie pourquoi il a servi
quoi ») a été attaqué adversarialement le 2026-08-11 et **réfuté dans sa généralité** : les *decision
logs* d'Open Policy Agent certifient chaque décision (input, version de la politique, résultat,
identifiant), les *evaluation reasons* de LaunchDarkly motivent chaque variation servie,
l'observabilité LLM enregistre la provenance du contexte servi
([journal](research/prior-art-2026-08-11.md)). **L'apport (b) est requalifié en trois points** :
l'objet (le service d'une référence de production, pas d'une politique ni d'une configuration) · le
chaînage Z2 (non constaté chez les voisins consultés) · la constante gagnée par gates dans le scellé.

## Médium ([SPEC règles M](SPEC.md#7-médium--règles-m))

**Interne.** H(Q′) au registre (2026-08-10) : la transposition d'un canon de récit visuel vers le récit
interactif, banc d'essai en cours : l'unique pièce du volet. Dans la lignée : le template de prompt par
média de PRISM, agnostique au moteur (recensé à la doctrine du template).

**Externe (passe #030).** Le headless CMS revendique « du site web à l'agent IA » : la portée
média-agnostique est en production ailleurs depuis des années. Rien de revendiqué.

**Apport.** Le coût d'un médium compté en deux pièces nommées (générateur + banc) et posé comme
**mesure de falsification** (H-média), pas comme promesse d'architecture.

## Dérive d'instance ([SPEC règles D](SPEC.md#8-dérive-dinstance--règles-d))

**Interne.** Les tests de dérive de LIVING REFERENCE (ses règles D) : la grille transposée du
référentiel à l'instance servie. La discipline du contre-test tracé du laboratoire (adoptée le
2026-08-06) : la détection constate, la correction est une décision : maker et checker séparés.

**Externe.** Passe dédiée faite le 2026-08-11 ([journal](research/prior-art-2026-08-11.md)) : le
champ du monitoring de dérive est établi et outillé — Evidently, NannyML, Alibi Detect ; *data*,
*concept* et *prediction drift*. Objet distinct : la dérive statistique de distribution sur des flux,
là où D éprouve la conformité d'instances servies à une constante déclarée, par élément. Voisinage
nommé, position inchangée : aucune revendication de nouveauté sur ce mécanisme.

**Apport.** D1 — la détectabilité *par construction*, un test par élément de la constante, l'élément
sans test déclaré non protégé : au service de la branche de mort n° 1, à instrumenter en premier.

## L'assise empirique

Toutes les pièces internes sont l'œuvre d'un seul praticien opérant ses propres déploiements : un point
de donnée : l'auteur, déclaré comme tel. Les pièces datées : les dés certifiés (2026-07-07, usage réel
continu) · le kernel gelé + modules just-in-time (en jeu le 2026-08-07) · le mode orchestré B-i
(8/8 appels conformes, une séance, le 2026-08-10) · SLIDING CANON (usage réel, cas fondateur de
LIVING REFERENCE) · LA RÉGIE v0.1 (déployée, non mesurée). THE LOOP est le **banc vivant** de la
doctrine-fonction, pas sa démonstration : le plafond posé au registre est maintenu.

## Antériorité du corpus

**Le nom.** WORKING REFERENCE, acté par l'auteur le 2026-08-11 après passe d'antériorité favorable
(étude versée à l'appareil de méthode du laboratoire), complétée le jour même par la **passe
registres via TMview** — INPI (FR), EUIPO, OMPI, USPTO : **aucune collision exacte** ; environnement
« reference » banalisé en classes 9/16/41/42 (929 marques FR contenant le mot, aucune n'étant
« WORKING REFERENCE »). Filtrage documenté à l'étude, pas un avis de conseil en PI.

**Le concept.** Passe externe du 2026-08-11 (gate #030 de l'appareil) : le principe « une source
unique, des instanciations par contexte » est un standard industriel : l'apport revendicable est
rétréci aux trois points du WHITEPAPER § 8. La forme réfutable est domiciliée au registre des
hypothèses (H(T), rév. 16, verdict d'auteur du dépôt #032).

## Dettes purgées (2026-08-11)

Les deux dettes déclarées à la version initiale de ce fichier sont purgées, sur décision de l'auteur :

1. **Le journal d'antériorité adversarial est versé** —
   [research/prior-art-2026-08-11.md](research/prior-art-2026-08-11.md) : pièces décisives vérifiées,
   dont le constat en creux de l'apport (b), **réfuté dans sa généralité** et requalifié (§ Scellé
   ci-dessus). La passe a corrigé le corpus (WHITEPAPER § 8, fiche SEAL, ce fichier). Les formulations
   d'avant-passe subsistent dans les pièces datées du laboratoire (dépôt #032, entrée H(T) du
   registre) : leur révision est un geste de l'appareil de méthode, signalé, jamais fait d'ici.
2. **La passe « monitoring de dérive » est faite** : voisinage nommé (§ Dérive d'instance ci-dessus),
   position inchangée : aucune revendication de nouveauté sur D.

Une dette purgée n'est pas une question fermée : toute pièce nouvelle rouvre les verdicts.

---

*JP Noto · WORKING REFERENCE · version 0.1 du 2026-08-11. [CC BY-NC-SA 4.0](LICENSE.md). Domicile canonique : <https://github.com/JP-Noto/WORKING-REFERENCE>.*
