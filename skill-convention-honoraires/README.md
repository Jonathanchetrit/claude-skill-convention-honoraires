# 📄 Claude Skill — Convention d'honoraires

> Génère vos conventions d'honoraires en fichier Word (.docx) en quelques secondes.  
> 6 modèles adaptés à la pratique fiscaliste. Entièrement personnalisable.

---

## Le problème que ce skill résout

Rédiger une convention d'honoraires prend du temps, surtout pour les dossiers complexes (contrôle fiscal, modules d'expatriation, consultation multi-options). Et les oublis de clauses ou de formules ont des conséquences.

Ce skill donne à Claude la **logique de sélection** entre 6 types de conventions, les **formules de rédaction exactes** adaptées à la fiscalité, et génère le **fichier Word** avec les coordonnées de votre cabinet — prêt à envoyer.

---

## Les 6 types de conventions

| Type | Situation |
|---|---|
| **1** | Contrôle fiscal — vous entrez dès la proposition de rectification |
| **2** | Contrôle fiscal — vous reprenez un dossier déjà avancé |
| **3** | Contentieux fiscal — recours devant le Tribunal Administratif |
| **4** | Consultation ou opinion de droit |
| **5** | Consultation complexe avec plusieurs options (avec tableau de prestations) |
| **6** | Mission par modules — expatriation, restructuration, optimisation patrimoniale |

---

## Ce que ça donne concrètement

Vous tapez :
> *"Nouveau dossier : M. Dupont, contrôle IS reçu hier, rappel 80 000 €. Forfait 4 500 € HT."*

Claude identifie le Type 1, vous demande les informations manquantes si besoin, et génère le fichier Word avec votre en-tête, les bonnes formules et les clauses adaptées.

---

## Installation

### Prérequis

- Compte [Claude.ai](https://claude.ai) — abonnement **Pro ou Team** recommandé

### En 3 étapes

**1. Téléchargez** ce repo (bouton Code → Download ZIP)

**2. Remplissez** `CONFIG.md` avec les informations de votre cabinet :
   - Nom, adresse, email, SIREN, barreau
   - Vos taux horaires par type de dossier
   - Votre police de document et votre logo (si disponible)

**3. Créez un Projet dans Claude.ai**
   - Ouvrez Claude.ai → Projets → Nouveau projet → "Conventions d'honoraires"
   - Dans les instructions, collez dans l'ordre :
     - Le contenu de `SKILL.md`
     - Le contenu de votre `CONFIG.md` rempli
     - Le contenu de `references/types-detail.md`
     - Le contenu de `references/clauses-conditions.md`

> Le fichier `INSTALL.md` contient le guide complet avec des exemples de dossiers.

---

## Contenu du repo

```
skill-convention-honoraires/
├── README.md                         ← Vous êtes ici
├── SKILL.md                          ← Instructions pour Claude (4 étapes)
├── CONFIG.md                         ← À remplir : cabinet, taux, police, logo
├── INSTALL.md                        ← Guide d'installation détaillé
└── references/
    ├── types-detail.md               ← Structure exacte des 6 types
    └── clauses-conditions.md         ← Clauses paiement, débours, TVA, confidentialité
```

---

## Limites importantes

- Le skill génère le document — la **relecture reste indispensable** avant envoi
- Les taux horaires sont des valeurs par défaut configurables — vous gardez le contrôle
- **La relation client et la négociation des honoraires restent votre responsabilité**

---

## Licence

[MIT](./LICENSE) — Utilisation libre, y compris commerciale. Citez la source si vous partagez.
