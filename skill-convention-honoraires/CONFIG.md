# CONFIG.md — Configuration cabinet
# Remplir une seule fois. Lu automatiquement à chaque génération de convention.
# Remplacez chaque valeur entre [ ] par vos informations.

---

## Identité du cabinet

```
NOM_CABINET     : [Ex. : MARTIN SOPHIE AVOCATE / CABINET DUPONT & ASSOCIÉS]
NOM_AVOCAT      : [Ex. : Sophie MARTIN / Jean-Pierre DUPONT]
TITRE_AVOCAT    : [Ex. : Avocat à la Cour / Avocat associé / Of Counsel]
BARREAU         : [Ex. : Barreau de Paris / Barreau de Lyon]
ADRESSE         : [Ex. : 12 avenue de la République — 75011 PARIS]
TEL             : [Ex. : 01 XX XX XX XX]
EMAIL           : [Ex. : contact@cabinet-martin.fr]
VILLE           : [Ex. : Paris]
SIREN           : [Ex. : 123 456 789]
```

---

## Taux horaires du cabinet

```
TAUX_CONTROLE   : [Ex. : 450]   € HT  ← Contrôle fiscal, consultation complexe
TAUX_CONSEIL    : [Ex. : 400]   € HT  ← Consultation, opinion de droit
TAUX_CONTENTIEUX: [Ex. : 350]   € HT  ← Contentieux TA, recours
```

> Ces taux sont des valeurs par défaut. L'avocat peut toujours préciser
> un taux différent au moment de la génération.

---

## Style du document

```
POLICE          : [Ex. : Garamond / Times New Roman / Calibri]
TAILLE_CORPS    : [Ex. : 11]    pt
TAILLE_PIED     : [Ex. : 10]    pt
```

---

## Logo

```
LOGO_DISPONIBLE : [oui / non]
LOGO_CHEMIN     : [Ex. : /mnt/user-data/uploads/logo_cabinet.png]
                  ← Si "non" : le nom du cabinet sera affiché en texte centré gras
```

---

## Paramètres de génération

```
SUCCES_FEE_DEFAUT : [5]   %  ← Taux honoraire de résultat (Type 2)
ACOMPTE_TYPE5     : [50]  %  ← Acompte à la signature (Type 5)
SOLDE_TYPE5       : [50]  %  ← Solde à la remise de la consultation (Type 5)
```

---

## Mention de confidentialité (personnalisable)

```
MENTION_CONFIDENTIEL : [Personnel et Confidentiel / Confidentiel / Personnel]
```

---

## Instructions spéciales

```
INSTRUCTIONS    : [Ex. : "Toujours ajouter une référence dossier AA.MM.N."
                          "Utiliser 'les meilleures' pour tous les clients."
                          "Inclure systématiquement la clause de médiation."
                          Laisser vide si aucune instruction particulière.]
```

---

*Ce fichier CONFIG.md est lu au démarrage de chaque génération de convention.
Modifiez-le à tout moment pour adapter les paramètres du skill à votre cabinet.*
