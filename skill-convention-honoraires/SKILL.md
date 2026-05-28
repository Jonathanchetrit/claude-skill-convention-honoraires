---
name: convention-honoraires
description: >
  Rédiger les conventions d'honoraires pour avocats fiscalistes.
  Déclencher ce skill dès que l'utilisateur mentionne "convention d'honoraires",
  "lettre de mission", "honoraires", "nouveau dossier", "proposition d'honoraires",
  ou décrit une situation client nécessitant une convention (contrôle fiscal,
  contentieux, consultation, restructuration, expatriation, optimisation patrimoniale).
  Le skill produit un fichier Word (.docx) professionnel, en sélectionnant
  automatiquement le bon type de convention parmi les 6 modèles disponibles,
  et en utilisant les informations du cabinet définies dans CONFIG.md.
---

# Convention d'honoraires — Avocat fiscaliste

## Étape 0 — Prérequis obligatoires

1. Lire `/mnt/skills/public/docx/SKILL.md` avant d'écrire la moindre ligne de code
2. Lire `CONFIG.md` pour récupérer les informations du cabinet

---

## Étape 1 — Collecter les informations du dossier

Poser les questions suivantes si les informations ne sont pas déjà fournies :

| Information | Pourquoi |
|---|---|
| Nom complet du client (ou société + interlocuteur) | Destinataire |
| Adresse complète du client | En-tête |
| Civilité (M. / Mme / Dr / Me / autre) | Formule d'appel et politesse |
| Date de la convention | Datation |
| Origine du contact (entretien du X / appel du X / échanges) | Phrase d'accroche |
| Nature de la mission | Choix du type (→ Étape 2) |
| Contexte factuel complet | Corps de la convention |
| Montants en jeu (si contrôle ou contentieux) | Corps + argumentation |
| Honoraires retenus (taux horaire et/ou forfait) | Si non fournis : utiliser CONFIG.md |
| Modules ou options ? | Types 5 ou 6 uniquement |
| Niveau de proximité avec le client | Formule de politesse |

---

## Étape 2 — Choisir parmi les 6 types

| Type | Situation | Honoraires | Structure |
|---|---|---|---|
| **1** | Contrôle fiscal — dès la proposition de rectification | Taux horaire + forfait global | Simple, sans tableau ni CONDITIONS |
| **2** | Contrôle fiscal — prise en cours de route | Provision + convention complémentaire + success fee | Historique procédural + analyse juridique préliminaire |
| **3** | Contentieux fiscal — recours Tribunal Administratif | Taux horaire + forfait jusqu'en appel | Analyse procédurale + délais impératifs |
| **4** | Consultation / opinion de droit | Taux horaire + forfait(s) par mission | Analyse juridique préliminaire intégrée |
| **5** | Consultation complexe multi-options | Taux horaire + tableau DÉTAIL DES PRESTATIONS | CONTEXTE + TABLEAU + DOCUMENTS + CONDITIONS |
| **6** | Mission par modules (expatriation, restructuration, optimisation) | Taux horaire + forfaits par module + total global | Modules numérotés avec sous-points |

Consulter `references/types-detail.md` pour la structure exacte de chaque type.

---

## Étape 3 — Éléments stylistiques invariants

### Phrases-clés à respecter mot pour mot

**Accroche :**
> « Dans le prolongement de [notre entretien / notre conversation téléphonique /
> notre rendez-vous / nos échanges] en date du [date], je vous confirme être
> [à votre disposition pour vous assister / en mesure de vous assister dans le
> cadre de...] »

**Rappel des faits :**
> « Ainsi que vous l'avez exposé, [...] »

**Pivot vers la mission :**
> « Dans ce contexte, si les termes de cette proposition d'honoraires vous
> conviennent, je me chargerai de [...] »

**Taux horaire (toujours mentionné, même si forfait ensuite) :**
> « Conformément aux usages de ma pratique, mes honoraires sont calculés sur la
> base du temps consacré à votre dossier, au taux horaire de [TAUX_CONFIG] € HT
> (auquel s'ajoute la TVA au taux de 20 %). »

**Passage au forfait :**
> « Toutefois, compte tenu de la difficulté d'anticiper précisément le temps
> nécessaire à l'accomplissement de mes travaux, je vous propose de convenir
> d'une convention d'honoraires forfaitaire s'élevant à [X] € HT [...] »

**Confirmation d'accord :**
> « Je vous serai reconnaissant de [bien vouloir] me confirmer votre accord
> [quant à mes conditions financières d'intervention] en me renvoyant la copie
> de cette lettre annotée de la mention *« bon pour accord »*. »

**Avant la formule de politesse :**
> « En vous remerciant par avance, »

### Formules de politesse

| Contexte | Formule |
|---|---|
| Client standard / professionnel | « Je vous prie de croire, Cher Monsieur / Chère Madame, en l'expression de mes salutations **distinguées**. » |
| Client proche / relation de confiance | « Je vous prie de croire, Cher Monsieur / Chère Madame, en l'expression de mes salutations **les meilleures**. » |
| Médecin | « Cher Docteur, » → formule adaptée |
| Couple | S'adresser au principal interlocuteur |

### Taux horaires — valeurs par défaut

Utiliser les taux définis dans `CONFIG.md`.
Si non renseignés, appliquer ces valeurs par défaut courantes en fiscalité :

| Type de dossier | Taux par défaut |
|---|---|
| Contrôle fiscal, consultation complexe | 400 € HT |
| Consultation / opinion de droit | 350 € HT |
| Contentieux TA | 300 € HT |

> ⚠️ Si l'avocat précise les honoraires → les respecter exactement.
> Les taux CONFIG.md et ceux précisés par l'avocat ont toujours la priorité.

---

## Étape 4 — Générer le fichier Word (.docx)

### Mise en page

- **Format** : A4
- **Marges** : 2,5 cm (haut / bas / gauche / droite)
- **Police** : [POLICE_CONFIG] (défaut : Garamond 11pt corps, 10pt pied de page)
- **Interligne** : 1,15
- **Alignement** : justifié

### Structure de la page

```
[En-tête : logo si disponible, sinon NOM_CABINET en gras centré]

                                    [NOM CLIENT en gras, aligné droite]
                                    [Adresse ligne 1]
                                    [Adresse ligne 2]
                                    A l'attention de [M./Mme NOM]  ← si société

Personnel et Confidentiel  (gras)
Par email  (gras)

                                    [VILLE_CONFIG], le [date]

Objet : Convention d'honoraires  (gras)

[Cher Monsieur / Chère Madame,]

[Corps de la convention — voir types-detail.md]

[NOM_AVOCAT]
[TITRE_AVOCAT]
```

### Pied de page (sur chaque page)
```
[NOM_CABINET] — [ADRESSE_CONFIG] — [TEL_CONFIG] — [EMAIL_CONFIG]
```

### Nommage du fichier
```
Convention_honoraires_[NOM_CLIENT]_[YYYYMMDD].docx
```

---

## Références complémentaires

- `references/types-detail.md` — Structure et formules pour chacun des 6 types
- `references/clauses-conditions.md` — Clauses CONDITIONS, paiement, débours, TVA
- `CONFIG.md` — Informations du cabinet (à lire en Étape 0)
