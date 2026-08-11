# INSTANCE DRIFT : la dérive d'instance · détectable par construction

Fiche opérationnelle. **Domicile normatif : [SPEC § 8, règles D1–D3](../SPEC.md#8-dérive-dinstance--règles-d)** ;
ce document explique, illustre et borne, il ne redéfinit pas.

## Le problème, en trois phrases

Une instanciation qui diverge de la constante sans que rien ne le constate est pire qu'un document
statique : le document ne prétend pas servir, la machine à dérive parfaite prétend, et elle industrialise
l'écart. C'est la branche de mort n° 1 du corpus, la réserve portée au verdict qui l'a admis. La parade
n'est pas la vigilance : c'est un test par élément, tenu par un banc.

## L'idée, en une image

Chaque élément de la constante porte son test, comme chaque dé certifié porte sa preuve : le banc
compare ce qui a été servi à l'invariant en vigueur, dans le médium servi. La détection et la
correction sont deux gestes : le banc constate et alerte ; corriger : l'instance, ou la constante par
gate : est une décision.

## Les questions que la pratique a posées, et les réponses

**« Qui corrige une dérive détectée ? »** Personne automatiquement (D2). Le banc alerte ; la décision
corrige. Un banc qui corrige seul est un auteur clandestin.

**« Et si l'instance est meilleure que la constante ? »** Ça arrive : alors la constante se révise par
gate (C2, C3), en connaissance de cause. Ce que D3 interdit, c'est l'alignement silencieux : la
constante qui suit ses instances n'est plus une référence, c'est une moyenne.

**« Un élément de la constante sans test, c'est grave ? »** C'est un élément non protégé, et le corpus
doit le dire (D1). L'inventaire des éléments sans test est la première chose qu'un banc honnête
publie.

## Les règles (SPEC § 8)

- **D1.** Détectable par construction : un test de banc par élément de la constante ; l'élément sans
  test est déclaré non protégé.
- **D2.** La détection constate et alerte ; la correction est une décision.
- **D3.** Jamais de rétro-action : l'instance se corrige, ou la constante se révise par gate : jamais
  par contamination.

## Les pièges

- **Le banc-correcteur** : un dispositif qui répare en silence cache la dérive au lieu de la montrer
  (D2) : la machine à dérive parfaite avec une couche de peinture.
- **La constante-moyenne** : « tout le monde fait comme ça maintenant » est une contamination, pas une
  révision (D3).
- **Le test-vague** : « relire de temps en temps » n'est pas un test ; D1 exige un test *par élément*,
  qui dit ce qu'une instance conforme n'a pas le droit de contredire.

## En pratique

C'est le banc prioritaire du corpus : le protocole de dérive d'instance sur THE LOOP, seuils fixés
avant mesure : prioritaire sur toute épaisseur de texte. Rien n'est instrumenté à ce jour, et le
corpus le dit.

**Ce que ça change** : une divergence a une date de détection et une pièce : la condition de
falsification n° 1 passe d'énoncée à armée.

---

*JP Noto · WORKING REFERENCE · [CC BY-NC-SA 4.0](../LICENSE.md). Domicile canonique : <https://github.com/JP-Noto/WORKING-REFERENCE>.*
