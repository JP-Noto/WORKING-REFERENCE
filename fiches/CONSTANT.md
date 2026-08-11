# CONSTANT : la constante · l'invariant gagné par gates

Fiche opérationnelle. **Domicile normatif : [SPEC § 3, règles C1–C5](../SPEC.md#3-constante--règles-c)** ;
ce document explique, illustre et borne, il ne redéfinit pas.

## Le problème, en trois phrases

Tout corpus de référence mélange ce qui ne doit pas bouger (le canon, l'identité, les règles) et ce
qui s'ajuste au travail du moment. Tant que tout est au même niveau, on recharge tout par peur, ou on
fige tout par prudence, et à la révision personne ne sait ce qu'on a le droit de toucher. Il faut un
partage structurel, avec un test d'admission, pas un tri d'intuition.

## L'idée, en une image

Pensez au kernel gelé d'un jeu : les règles ne bougent jamais en partie, l'habillage change à chaque
tour. La constante est ce kernel, et elle n'a pas de forme : elle s'énonce en canon, identité, règles,
jamais en texte, image ou son, qui n'en sont que des réalisations. Elle ne grossit pas par l'usage :
chaque entrée passe une **gate** datée, chaque révision dit ce qu'elle remplace.

## Les questions que la pratique a posées, et les réponses

**« Comment je sais si un élément est constante ou variable ? »** Un seul test (C4) : sa révision au
changement de génération de modèle serait-elle un échec du corpus ? Si non, c'est une variable. Le
doute se tranche variable.

**« Ma constante doit-elle être petite ? »** Elle est bornée par le test, pas par un nombre. Mais un
élément qui peut varier sans dommage n'y a pas sa place : la constante minimale est celle qui survit
au test, pas celle qui rassure.

**« Qui tient la gate ? »** L'appareil que votre déploiement déclare : la gate est un rôle, l'appareil
est hors du corpus (SPEC, intro). Pour ONDE, c'est [ACTA](https://github.com/JP-Noto/ONDE/blob/main/methode/ACTA.md).

## Les règles (SPEC § 3)

- **C1.** Constante déclarée, périmètre nommé ; tout élément est constante ou variable, un non-déclaré
  est une variable.
- **C2.** Rien n'entre que par gate datée, jamais par usage, récence ou répétition.
- **C3.** Révision datée seulement, qui énonce ce qu'elle remplace.
- **C4.** Test d'admission : la révision au changement de génération serait un échec ; le doute se
  tranche variable.
- **C5.** La constante s'énonce hors de tout médium.

## Les pièges

- **La constante-fourre-tout** : « important » n'est pas un critère ; un élément qui rate le test C4
  est du chargement en bloc en costume.
- **La constante-médium** : un texte sacré figé mot à mot est une instanciation qui a pris la place de
  l'invariant (C5) : c'est l'invariant qu'on protège, pas sa formulation.
- **L'entrée par habitude** : « on a toujours fait comme ça » n'est pas une gate (C2).
- **La constante qui bouge sans trace** : c'est une variable qui se fait passer pour elle (C3).

## En pratique

Le cas vivant est le kernel gelé de THE LOOP : les règles gelées en partie, tout le reste monté en
modules au besoin du tour : en jeu réel depuis le 2026-08-07, un praticien, non mesuré.

**Ce que ça change** : la survie au changement de génération de modèle se mesure sur un périmètre
nommé, pas sur le corpus entier, et l'échec y a une définition.

---

*JP Noto · WORKING REFERENCE · [CC BY-NC-SA 4.0](../LICENSE.md). Domicile canonique : <https://github.com/JP-Noto/WORKING-REFERENCE>.*
