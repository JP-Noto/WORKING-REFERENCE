# SPEC · WORKING REFERENCE

**Version 0.1 · 2026-08-11 · statut : proposé.**

Document normatif : les règles, sans leur justification. Le pourquoi de chaque règle est au
[whitepaper](WHITEPAPER.md). « DOIT » et « NE DOIT PAS » se lisent au sens de la RFC 2119. Le français
fait foi.

WORKING REFERENCE norme la **référence qui travaille** : comment un corpus de référence se structure
(une constante, des variables), s'instancie (une décision d'après le travail en cours), se sert (jamais
chargé en bloc) et se scelle (la décision traçable). Il ne norme ni le statut du savoir (rôle de
[LIVING REFERENCE](https://github.com/JP-Noto/LIVING-REFERENCE), qu'il généralise), ni la relation
humain–assistant (rôle de [MYSTANCE](https://github.com/JP-Noto/MYSTANCE)) : l'OS hôte, lui,
gouverne le système : quatre couches, quatre rôles, aucune redondance. La thèse en une phrase : un corpus n'est pas un document qu'on lit,
c'est une fonction qu'on appelle.

Les gates, bancs et rangs de ce document sont des **rôles**, jamais des institutions : l'appareil qui
les tient est hors du corpus, et tout déploiement conforme DOIT tenir ces rôles avec son propre
appareil et le nommer. Pour ONDE, ils sont tenus par [ACTA](https://github.com/JP-Noto/ONDE/blob/main/methode/ACTA.md),
l'appareil de méthode du laboratoire : qui
est en amont de la fonction (il fabrique et juge les constantes), jamais la fonction elle-même.

## 1. Termes

*Chaque terme a son ancre : les autres documents lient ici, domicile unique des définitions. Les termes
sont EN-canoniques, la glose française suit — régime de langue de la famille.*

### Constant
*(la constante)* L'invariant d'un corpus : canon, identité, règles : ce qui doit survivre à un
changement de génération de modèle sans révision. La constante se gagne par gates (règles C), jamais
par l'usage ; elle n'est réalisée dans aucun médium : texte, image et son n'en sont que des
instanciations.

### Variable
*(la variable)* Tout ce qui s'ajuste à l'appel : la part située de l'output. Le médium est une
variable. Une variable est faite pour changer ; sa révision n'est jamais un échec.

### Working state
*(l'état du travail en cours)* L'état déclaré du travail au moment de l'appel : la phase, l'unité en
cours, le besoin. C'est l'entrée de la décision d'instanciation : une donnée déclarée, pas un jugement
de pertinence laissé au contexte appelant.

### Call
*(l'appel)* L'acte par lequel un travail sollicite la référence. Un appel porte son working state ;
il reçoit une instanciation, jamais le corpus.

### Reference layer
*(la couche de référence)* L'autorité qui tient la constante et décide l'instanciation. Elle sert ;
elle ne se consulte pas en bloc. Note de famille : chez LIVING REFERENCE, une *référence* est un
élément validé : ici, « la référence » désigne la couche qui tient de tels éléments et les sert.
L'élément reste l'élément, la couche reste la couche.

### Instantiation
*(l'instanciation)* L'output d'un appel : la constante plus les variables résolues d'après le working
state. Située et jetable : elle guide le travail de son appel et ne modifie jamais la constante.

### Serving
*(le service)* La délivrance de l'instanciation au contexte appelant : exactement ce qui a été décidé,
rien d'autre. Le contraire du chargement en bloc.

### Seal
*(le scellé)* La trace certifiante d'une décision d'instanciation : quel appel, quel état de la
constante, ce qui a été servi, la règle qui l'a décidé. Le scellé rend la décision auditable ; il
n'autorise rien.

### Gate
*(la gate)* L'épreuve datée par laquelle un élément entre dans la constante ou en change. Le rang d'un
élément se gagne à la gate, jamais par récence, répétition ou usage. La gate est un rôle : l'appareil
qui la tient est déclaré par le déploiement et vit hors du corpus (intro) : lire « gate » ici, ce n'est
pas lire l'appareil de ONDE.

### Instance drift
*(la dérive d'instance)* La divergence entre une instanciation servie et la constante en vigueur. Sa
détectabilité est une exigence de construction (règles D) ; une divergence indétectable met le corpus
entier en défaut (§ 9, condition 1).

### Medium
*(le médium)* Le canal de réalisation d'une instanciation : texte, image, son, récit interactif. Une
variable parmi les autres : ajouter un médium ajoute un generator et un bench, jamais une seconde
couche de référence.

### Generator
*(le générateur)* Le composant qui réalise une instanciation dans un médium donné. Propre à chaque
médium ; sans autorité : il transcrit ce que la couche de référence a décidé.

### Bench
*(le banc)* Le dispositif qui éprouve, médium par médium, la conformité des instanciations à la
constante. C'est lui qui rend la dérive d'instance détectable ; il falsifie la mécanique, il ne valide
jamais la valeur.

## 2. Axiomes

- **A1. La référence est une fonction.** Un corpus conforme ne se lit pas, il s'appelle : son output
  est décidé, servi et scellé. Le document n'est qu'une réalisation possible de la fonction : commode
  pour l'humain, jamais l'objet lui-même.
- **A2. La constante n'est pas un média.** L'invariant est le canon, l'identité, les règles ; jamais le
  texte, l'image ou le son qui les réalisent. Corollaire : ce qui doit survivre au changement de
  génération est la constante ; les variables sont faites pour changer.
- **A3. L'autorité reste dans la couche.** Aucune instanciation ne fait autorité : l'autorité vit dans
  la constante, hors de l'instance servie. Principe hérité de LIVING REFERENCE — la référence vit dans
  la source, pas dans ses restitutions, et frère de la règle du sort : l'autorité vérifiable se tient
  hors du modèle.

## 3. Constante : règles C

- **C1.** Un corpus conforme déclare sa constante : un périmètre nommé, séparé des variables. Tout
  élément est **constante ou variable**, jamais les deux, jamais ni l'un ni l'autre ; un élément non
  déclaré est une variable.
- **C2.** Rien n'entre dans la constante que par une gate datée. L'usage, la récence, la répétition
  n'y font rien entrer.
- **C3.** La constante ne change que par révision datée, et toute révision énonce ce qu'elle remplace.
  Une constante qui bouge sans trace n'est pas une constante : c'est une variable qui se fait passer
  pour elle.
- **C4.** Test d'admission : un élément appartient à la constante si sa révision au changement de
  génération de modèle serait un échec du corpus. Tout élément qui peut varier selon le travail sans
  dommage est une variable : le doute se tranche variable.
- **C5.** La constante s'énonce indépendamment de tout médium (A2). Une « constante » qui ne s'énonce
  que dans un médium est une instanciation qui a pris la place de l'invariant.

## 4. Instanciation : règles I

- **I1.** Toute instanciation est décidée par la couche de référence d'après le working state de
  l'appel. Le contexte appelant déclare son état ; il ne choisit pas ce qui lui est servi.
- **I2.** La décision d'instanciation est réglée : elle s'exécute sans jugement d'auteur à l'appel.
  L'auteur PEUT régler les règles de décision ; il NE DOIT PAS être requis à chaque appel, sinon la
  fonction ne se code pas, on a renommé le travail (§ 9, condition 2).
- **I3.** Une instanciation est située et jetable : elle guide le travail de son appel, n'engage rien
  au-delà, et ne modifie jamais la constante. Une instanciation qui mérite de durer repasse par une
  gate (C2) ; il n'y a pas d'autre porte.
- **I4.** Le volume servi par appel est borné par le besoin de l'appel, jamais par la taille du
  corpus : à besoin constant, il ne croît pas quand le corpus croît. C'est la propriété mesurable
  centrale (§ 9, condition 3).

## 5. Service : règles S

- **S1.** La référence se sert, elle ne se charge pas : le corpus entier ne monte jamais au contexte
  d'un appel.
- **S2.** Ce qui est servi est exactement l'instanciation décidée : rien de plus (need-to-know), rien
  de moins (l'appel n'a pas à quémander ce que son working state appelle).
- **S3.** Tout élément servi reste relié à sa source dans la couche de référence. Une instanciation
  dont on ne peut plus remonter à la constante est une copie qui divergera, pas un service.
- **S4.** Le service déclare son moment : quel élément monte, à quel appel, sous quelle condition. Le
  contrat de chargement est écrit dans la couche, jamais improvisé à l'appel.

## 6. Scellé : règles Z

- **Z1.** Toute décision d'instanciation émet un scellé : l'appel et son working state, l'état
  (version) de la constante, ce qui a été servi, la règle qui l'a décidé.
- **Z2.** Les scellés se consignent dans l'instant du geste et se chaînent : une piste, pas des reçus
  épars. Un scellé écrit après coup n'est pas un scellé.
- **Z3.** Le scellé constate, il n'autorise pas : c'est une pièce d'audit, jamais un verrou sur le
  travail : garde héritée de la famille : un contrôle qui conditionne la progression a déplacé
  l'autorité.
- **Z4.** Un service sans scellé sert, mais ne fait pas preuve (miroir de la consignation de
  LIVING REFERENCE, règle S8).

## 7. Médium : règles M

- **M1.** Le médium d'une instanciation est une variable de l'appel ; la constante n'en porte aucun
  (C5).
- **M2.** Ajouter un médium ajoute un generator et un bench ; il n'ajoute jamais une couche de
  référence. Un médium qui exige sa propre constante réfute la portée média-agnostique (§ 9,
  condition 4).
- **M3.** Chaque médium sert avec son banc : la conformité d'une instanciation s'éprouve dans le médium
  où elle est servie, jamais par transposition depuis un autre.

## 8. Dérive d'instance : règles D

- **D1.** La dérive d'instance est détectable par construction : pour tout élément de la constante, il
  existe un test de banc qui constate qu'une instanciation le contredit. Un élément de la constante
  sans test n'est pas encore protégé, et le corpus le dit.
- **D2.** La détection constate et alerte ; la correction est une décision. Aucun banc ne corrige de
  lui-même ni ne bloque le travail (Z3).
- **D3.** Une instanciation en dérive ne rétro-agit jamais : la constante ne s'aligne pas sur ses
  instances. L'instance se corrige, ou la constante se révise par gate (C2, C3), jamais par
  contamination.

Ces règles s'appliquent au corpus WORKING REFERENCE lui-même : ce document est la constante déclarée
du corpus ; ses instanciations (résumés, extraits servis, adaptations) n'en font jamais autorité (A3).
En particulier, C2 s'applique à la SPEC : une règle n'y entre que par révision datée, et à une condition
d'admission : porter un banc vivant, ou la condition de falsification qui la tuerait. Le doute se
tranche « ça n'entre pas » (C4).

## 9. Falsification

La forme réfutable de la doctrine-fonction est domiciliée au registre des hypothèses d'ACTA — **H(T)**,
inscrite le 2026-08-11 (rév. 16, verdict d'auteur du dépôt #032). Cette section cite, elle ne redéfinit pas.
Règle de mesure héritée de la lignée interne : l'indicateur est arrêté avant la première mesure, jamais
après.

Le corpus est en défaut si :

1. **la machine à dérive parfaite** : une instanciation diverge de la constante sans qu'aucun banc ne
   le constate. C'est pire que le document statique, qui au moins ne prétend pas servir ; c'est la
   branche de mort à instrumenter en premier (réserve portée au verdict).
2. **la fonction ne se code pas** : la décision d'instanciation exige un jugement d'auteur à chaque
   appel. On n'a pas construit une fonction, on a renommé le travail.
3. **le volume croît** : à besoin constant, les tokens servis par appel croissent avec la taille du
   corpus. La propriété centrale (I4) tombe.
4. **une famille de systèmes, pas une fonction** : un médium ajouté exige sa propre couche de
   référence, ou son coût d'ajout dépasse un générateur plus un banc. H-média tombe : mesure : ce qui
   doit être réécrit au premier médium ajouté ; premier franchissement au banc : la transposition
   visuel → interactif, H(Q′).
5. **le partage ne découpe rien** : au changement de génération de modèle, la constante exige une
   révision comparable à celle des variables. La survie devait se mesurer sur la constante seule ; si
   elle ne s'y mesure pas, la distinction constante/variables n'était qu'un rangement.

Les conditions 1 et 2 sont armées dès les bancs vivants ; la 3 se mesure au premier terrain
instrumenté ; la 4 au premier médium ajouté ; la 5 au prochain changement de génération de modèle.
D'ici là, la réfutabilité est énoncée, pas toute instrumentée, et le corpus le dit plutôt que de
l'habiller.

## 10. Rangs de preuve

L'échelle est celle du pipeline du laboratoire : **réflexion → hypothèse → banc d'essai → terrain
chercheur → auditable → utilisateurs réels → répliqué → doctrine**. Aucun rang ne s'auto-décerne :
cette section cite ses verdicts, et le registre des hypothèses d'ACTA fait foi. Le statut documentaire
(`proposé / validé`) est une décision éditoriale de l'auteur : il atteste la cohérence arrêtée d'un
texte, jamais l'efficacité d'un mécanisme.

| Mécanisme | Rang | Pièce |
|---|---|---|
| La doctrine-fonction (le corpus entier) | **hypothèse** | verdict d'auteur du 2026-08-11, dépôt ACTA #032, inscrite H(T) au registre (rév. 16) |
| Le canon servi plutôt que chargé (règles S) | hypothèse, cas particulier | H(Q) au registre |
| La transposition hors médium (règles M) | hypothèse, cas particulier | H(Q′) au registre ; premier franchissement au banc (visuel → interactif) |
| La distillation qui monte (C2, la gate comme seule porte) | hypothèse, cas particulier | H(P′) au registre |
| Les invariants dans l'exécuteur | hypothèse, voisine | H(S) au registre (antériorité externe faite, apport rétréci à la certification de structure) |

**Bancs vivants, sans rang revendiqué** : le kernel gelé et les modules just-in-time de THE LOOP (en
jeu depuis le 2026-08-07) · le mode orchestré B-i, où l'orchestrateur décide le need-to-know de chaque
appel (8/8 appels conformes le 2026-08-10) · SLIDING CANON en usage réel · LA RÉGIE v0.1 comme
instanciateur · la doctrine du template, validée au conteneur (statut éditorial, pas un rang du
pipeline). THE LOOP est le banc vivant de la doctrine-fonction ; le plafond de H(P) est maintenu :
« démonstration » reste à prouver. Aucun mécanisme n'atteint le terrain chercheur : le corpus dit
« hypothèse » tant que le pipeline n'a pas tranché.

---

*JP Noto · WORKING REFERENCE · [CC BY-NC-SA 4.0](LICENSE.md). Domicile canonique : <https://github.com/JP-Noto/WORKING-REFERENCE>.*
