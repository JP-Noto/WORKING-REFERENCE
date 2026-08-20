# WORKING REFERENCE

**La référence qui travaille : le corpus comme fonction.**

WORKING REFERENCE est un corpus de règles écrites, pas un logiciel : rien à installer ; des règles
qu'un système peut appliquer, et que tout lecteur peut lire, opposer et vérifier.

[English version](README.md) · si les deux divergent, le corpus français fait foi.

`Statut : Public Draft` · `SPEC : 0.1` · `Rang : hypothèse` · `Licence : CC BY-NC-SA 4.0`

## Le constat

Un corpus de référence s'emploie de deux façons, et les deux échouent quand le travail dure.
**Chargé en bloc**, son coût croît avec sa taille et dilue ce qu'il protège. **Consulté à la
demande**, ce qui arrive au travail dépend de qui se souvient, ou de ce qui ressemble, et personne
ne constate la divergence entre le travail et la référence.

## Le principe : appeler, pas lire

Un corpus n'est pas un document qu'on lit, c'est une **fonction qu'on appelle** : une **constante**
(l'invariant gagné par gates — canon, identité, règles : ce qui doit survivre à un changement de
génération de modèle) plus des **variables** (résolues à chaque appel). Le travail déclare son état ;
la **couche de référence** décide ce qui est **servi** (jamais chargé en bloc) et chaque décision
est **scellée** : traçable, chaînée, opposable. Le média est une variable : un médium de plus coûte
un générateur et un banc, jamais une seconde couche de référence.

La propriété mesurable qui en découle : le volume servi par appel ne croît pas avec la taille du
corpus.

## Les documents

| Document | Voix | Ce qu'on y trouve |
|---|---|---|
| [SPEC](SPEC.md) | normative | termes, axiomes, règles C/I/S/Z/M/D, falsification, rangs — domicile unique des définitions |
| [WHITEPAPER](WHITEPAPER.md) | le papier | la thèse, l'architecture, les bancs vivants, ce qui réfuterait la méthode, les travaux voisins |
| [fiches/](fiches/index.md) | professeur | une fiche par mécanisme : le problème, l'image, les pièges, en pratique |
| [LINEAGE](LINEAGE.md) | filiation | chaque mécanisme relié à ses sources, internes et externes, et les dettes déclarées |
| [CHANGELOG](CHANGELOG.md) · [CITATION.cff](CITATION.cff) · [LICENSE](LICENSE.md) · [CONTRIBUTING](CONTRIBUTING.md) | | versions, citation, licence, état des contributions |

## La famille

Cinq couches, cinq rôles, aucune redondance — l'OS hôte gouverne le système, et quatre corpus se
partagent le reste : [**LIVING REFERENCE**](https://github.com/JP-Noto/LIVING-REFERENCE) norme le statut
du savoir, ce qui fait autorité ; [**MYSTANCE**](https://github.com/JP-Noto/MYSTANCE) norme la relation humain–assistant ; [**SOUNDNESS**](https://github.com/JP-Noto/SOUNDNESS) norme la
naissance du savoir extrait de documents, la fiche fondée sur la pièce ; **WORKING REFERENCE** norme
la référence qui travaille : comment l'autorité arrive
à l'appel. Les gates, bancs et rangs de ce corpus sont des **rôles** : l'appareil qui les tient est
celui du déployeur, jamais fourni par le corpus. La famille est opérée par le laboratoire
ONDE AI R&D — son portail : <https://github.com/JP-Noto/ONDE>.

## Le rang, dit honnêtement

L'ensemble est une **hypothèse** : verdict du 2026-08-11, forme réfutable domiciliée au registre de
l'appareil de méthode du laboratoire. Les mécanismes existent séparément en usage réel, chez un seul
praticien opérant ses propres déploiements : un point de donnée. Leur réunion sous une seule fonction
n'est pas éprouvée. Deux dettes d'antériorité sont déclarées au [LINEAGE](LINEAGE.md) et conditionnent
la publication. Le [WHITEPAPER § 7](WHITEPAPER.md) énonce ce qui réfuterait la méthode.

## Citer

Voir [CITATION.cff](CITATION.cff). Licence : [CC BY-NC-SA 4.0](LICENSE.md) : mettre en œuvre la
doctrine-fonction est expressément libre ; l'usage commercial des textes requiert un accord écrit.

---

*JP Noto · WORKING REFERENCE · [CC BY-NC-SA 4.0](LICENSE.md). Domicile canonique : <https://github.com/JP-Noto/WORKING-REFERENCE>.*
