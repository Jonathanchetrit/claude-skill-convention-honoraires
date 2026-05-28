# INSTALL.md — Guide d'installation en 5 minutes
# Skill : Convention d'honoraires — Avocat fiscaliste
# Aucune compétence technique requise.

---

## Ce que fait ce skill

Ce skill génère automatiquement vos conventions d'honoraires en fichier Word (.docx),
prêtes à envoyer. Il choisit le bon modèle parmi 6 types selon la nature du dossier,
applique votre style de rédaction et utilise les informations de votre cabinet.

---

## Étape 1 — Prérequis

- Un compte **Claude.ai** (Pro ou Team recommandé)
- Le connecteur **Google Drive** activé (optionnel, pour sauvegarder directement)
  → Paramètres → Outils → Google Drive → Activer

---

## Étape 2 — Configurer votre cabinet

**C'est l'étape la plus importante.** Ouvrez le fichier `CONFIG.md` et remplissez :

- [ ] Nom de votre cabinet
- [ ] Votre nom et titre (Avocat à la Cour, etc.)
- [ ] Votre barreau
- [ ] Adresse, téléphone, email, ville
- [ ] Vos taux horaires par type de dossier
- [ ] Votre police de document (Garamond recommandé)
- [ ] Disponibilité d'un logo (et son chemin si oui)
- [ ] Paramètres de facturation (acompte Type 5, success fee Type 2)

---

## Étape 3 — Installer le skill

### Option A — Via un Projet Claude (recommandé)

1. Ouvrez **Claude.ai** → **Projets** → **Nouveau projet**
2. Nommez-le "Conventions d'honoraires"
3. Dans les **instructions du projet**, copiez-collez dans l'ordre :
   - Le contenu de `SKILL.md`
   - Le contenu de votre `CONFIG.md` **rempli**
4. Toujours dans les instructions, ajoutez les contenus de :
   - `references/types-detail.md`
   - `references/clauses-conditions.md`

### Option B — À la demande (sans projet)

Dans une conversation Claude, commencez par :
> "Voici mes instructions pour générer une convention d'honoraires : [coller SKILL.md + CONFIG.md]"

---

## Étape 4 — Générer votre première convention

Dans votre Projet, tapez par exemple :

> *"Nouveau dossier : M. Durand, contrôle fiscal IS reçu hier, rappel de 45 000 €.
> Réunion ce matin. Convention Type 1, honoraires 3 500 € HT."*

Claude va :
1. Identifier le Type 1 (contrôle fiscal dès la proposition)
2. Vous demander les informations manquantes si nécessaire
3. Générer le fichier Word avec votre en-tête, vos coordonnées, les bonnes formules
4. Nommer le fichier `Convention_honoraires_DURAND_[date].docx`

---

## Étape 5 — Personnaliser davantage

Vous pouvez adapter le comportement en modifiant `CONFIG.md` :

| Paramètre | Exemple |
|---|---|
| Ajouter une référence dossier automatique | INSTRUCTIONS : "Toujours inclure une référence Nos Réf. : AA.MM.N" |
| Changer la formule de politesse par défaut | INSTRUCTIONS : "Utiliser 'les meilleures' pour tous les clients" |
| Ajouter la clause de médiation | INSTRUCTIONS : "Inclure systématiquement la clause de médiation" |
| Facturation différente | Modifier ACOMPTE_TYPE5 et SOLDE_TYPE5 |

---

## Les 6 types en un coup d'œil

| Type | Quand l'utiliser |
|---|---|
| **1** | Contrôle fiscal — vous entrez dès la proposition de rectification |
| **2** | Contrôle fiscal — vous prenez le dossier en cours de route |
| **3** | Contentieux — recours devant le Tribunal Administratif |
| **4** | Consultation ou opinion de droit (question ciblée) |
| **5** | Consultation complexe avec plusieurs options (avec tableau) |
| **6** | Mission multi-modules (expatriation, restructuration, optimisation) |

---

## En cas de problème

| Problème | Solution |
|---|---|
| Le fichier Word ne se télécharge pas | Vérifiez votre abonnement Claude (Pro requis pour les fichiers) |
| Les informations du cabinet sont fausses | Vérifiez votre CONFIG.md — chaque valeur entre [ ] doit être remplacée |
| Claude choisit le mauvais type | Précisez "Type X" dans votre demande |
| La mise en page est incorrecte | Précisez votre police dans CONFIG.md > POLICE |

---

*Skill créé pour les avocats fiscalistes.*
*Version 1.0*
