# Détail des 6 types de conventions d'honoraires

---

## TYPE 1 — Contrôle fiscal dès la proposition de rectification

**Déclencheur :** Le client vient de recevoir une proposition de rectification
(formulaires 3924-V-SD, 3929, 2120, etc.) et confie la défense du dossier depuis le début.

**Structure :**
1. En-tête + logo (ou NOM_CABINET si pas de logo)
2. Destinataire (nom, adresse)
3. Mention confidentialité + "Par email" (gras)
4. Ville + date
5. Objet : Convention d'honoraires (gras)
6. Formule d'appel
7. **Accroche** ("Dans le prolongement de nos échanges...")
8. **Description factuelle** :
   - Référence exacte de la proposition (ex : n°3924-V-SD du [date])
   - Nature des rectifications (TVA, IS, IR, etc.)
   - Montant total du rappel décomposé (droits + intérêts + majorations + amendes)
9. **Périmètre de la mission** :
   - "je me chargerai de vous assister dans le cadre de l'ensemble de ce contrôle
     et ce, jusqu'à la réception de votre avis de mise en recouvrement"
   - Mention obligatoire : "En cas de nécessité de poursuivre la procédure et de
     procéder à la rédaction d'une réclamation contentieuse avec demande de sursis
     de paiement, il conviendra de procéder à la mise en place d'une convention
     d'honoraires distincte."
10. Taux horaire (→ TAUX_CONTROLE dans CONFIG.md)
11. Forfait global : "je vous propose de convenir d'une convention d'honoraires
    forfaitaire s'élevant à [X] € HT pour l'ensemble de la procédure susmentionnée."
12. Phrase "bon pour accord"
13. "En vous remerciant par avance,"
14. Formule de politesse + NOM_AVOCAT + TITRE_AVOCAT

**Ne pas inclure :** tableau de prestations, section CONDITIONS formelle,
liste de documents, honoraire de résultat.

---

## TYPE 2 — Contrôle fiscal pris en cours de route

**Déclencheur :** L'avocat prend un dossier déjà avancé (plusieurs propositions envoyées,
réponse aux observations reçue, AMR imminent ou déjà reçu).

**Particularités :**
- Rappel **très détaillé** de l'historique procédural (dates, références, montants)
- **Analyse juridique préliminaire intégrée** : l'avocat pose les bases dès la convention
  (références CGI, LPF, jurisprudence) pour valoriser son expertise
- Formule d'appel adaptée si le client a un titre professionnel ("Cher Docteur,")
- **Pas de forfait global** → provision correspondant à un nombre d'heures précis
  (ex : "2 000 € HT = 5h × 400 €/h") + convention complémentaire ultérieure
- **Clause honoraire de résultat** :
  > "En cas de gain de cause et d'abandon total ou partiel par l'Administration
  > fiscale, je vous propose de convenir d'un honoraire de résultat de
  > [SUCCES_FEE_DEFAUT] % sur l'ensemble des sommes qui vous seront dégrevées."
- Mission préalable : obtenir l'intégralité du dossier avant de définir la stratégie
- Formule de politesse : "les meilleures" (relation de confiance implicite)

**Structure :**
1. En-tête + logo
2. Destinataire
3. Mention confidentialité + "Par email"
4. Ville + date
5. Objet
6. Formule d'appel (adaptée au titre du client)
7. Accroche
8. **Historique procédural détaillé** (dates + références + montants)
9. **Analyse préliminaire juridique** (articles CGI, LPF applicables, jurisprudence)
10. Stratégie envisagée + prochaine étape
11. Mention urgence si applicable (délais de recours)
12. Taux horaire (→ TAUX_CONTROLE ou TAUX_CONSEIL selon CONFIG.md)
13. **Provision** : "La provision sollicitée, d'un montant de [X] € HT, correspond
    ainsi à [Y] heures de travail d'ores et déjà destinées au traitement initial de
    votre dossier. Une fois les pièces intégralement obtenues, je vous adresserai
    une convention d'honoraires complémentaire."
14. **Honoraire de résultat** (SUCCES_FEE_DEFAUT %)
15. Phrase "bon pour accord"
16. Formule de politesse

---

## TYPE 3 — Contentieux fiscal — Recours Tribunal Administratif

**Déclencheur :** L'administration a définitivement rejeté la demande (refus de
remboursement de crédit TVA, maintien des rappels après AMR, rejet de réclamation
contentieuse) → saisir le Tribunal Administratif dans les délais.

**Particularités :**
- **Analyse procédurale dans la convention** : état de la procédure, vice de
  procédure éventuel, **délai de recours impératif** (2 mois à compter de la
  notification — préciser la date limite exacte)
- Retenir la date du courrier de l'administration (pas la date de réception)
  pour le calcul du délai
- Mention de la stratégie contentieuse envisagée
- Taux horaire (→ TAUX_CONTENTIEUX dans CONFIG.md)
- Forfait jusqu'en appel avec **convention distincte si appel** :
  > "Cela signifie que nous conviendrons d'une nouvelle convention d'honoraires
  > dans le cas où nous déciderions d'interjeter appel de la décision du
  > Tribunal Administratif."
- Formule de politesse : "les meilleures"

**Structure :**
1. En-tête + logo
2. Destinataire (nom société + interlocuteur si B2B)
3. Mention confidentialité + "Par email"
4. Ville + date
5. Objet
6. Formule d'appel
7. Accroche
8. **Rappel factuel** (nature du litige, décision contestée, montants)
9. **Analyse procédurale** + délais + stratégie
10. Mission : "je me chargerai de réaliser une requête devant le Tribunal
    Administratif compétent"
11. Taux horaire
12. Forfait + mention "jusqu'en appel" + nouvelle convention si appel
13. Phrase "bon pour accord"
14. Formule de politesse

---

## TYPE 4 — Consultation / Opinion de droit

**Déclencheur :** Question de droit fiscal ciblée (résidence fiscale, exit tax,
donation internationale, structuration, etc.) sans caractère contentieux.

**Particularités :**
- **Analyse juridique préliminaire intégrée** : poser les bases légales dans la
  convention (références aux textes, conventions bilatérales, qualification des
  situations) pour valoriser l'expertise dès la lettre de mission
- Honoraires : **deux forfaits distincts** si deux missions différentes
  (ex : 2 500 € HT pour la consultation + 3 000 € HT pour la note exit tax)
- Pas de tableau de prestations
- Pas de section CONDITIONS formelle
- Formule de politesse : "distinguées"

**Structure :**
1. En-tête + logo
2. Destinataire
3. Mention confidentialité + "Par email"
4. Ville + date
5. Objet
6. Formule d'appel
7. Accroche
8. **Contexte factuel** (situation du client)
9. Mission : "je me chargerai de rédiger une opinion de droit sur [...]"
10. **Analyse juridique préliminaire** (textes applicables, qualification, enjeux)
11. Taux horaire (→ TAUX_CONSEIL dans CONFIG.md)
12. Forfait(s) par mission
13. Phrase "bon pour accord"
14. Formule de politesse

---

## TYPE 5 — Consultation complexe multi-options (avec tableau)

**Déclencheur :** Mission complexe avec plusieurs prestations principales +
options facultatives (ex : consultation fiscale + rédaction contrat de prêt en
option + création SCI en option + régularisation déclarative en option).

**Particularités :**
- Section **CONTEXTE DE LA MISSION** (titre en gras majuscules) avec situation
  factuelle détaillée
- Description de la mission : liste numérotée en italique *(1)*, *(2)*, *(3)*...
- **Tableau DÉTAIL DES PRESTATIONS** : 4 colonnes
  (N° | Prestation | Statut [Inclus / Option] | Honoraires HT)
- Total forfaitaire HT et TTC
- **LISTE DES DOCUMENTS ET RENSEIGNEMENTS À FOURNIR** (titre gras majuscules)
  avec liste à puces
- **CONDITIONS** (titre gras majuscules) → voir `clauses-conditions.md`
- Séparateur `* * *` avant la phrase finale
- Taux horaire (→ TAUX_CONTROLE dans CONFIG.md)
- Formule de politesse : "distinguées"

**Structure :**
1. En-tête + logo
2. Destinataire
3. Mention confidentialité + "Par email"
4. Ville + date
5. Objet
6. Formule d'appel
7. Accroche
8. **CONTEXTE DE LA MISSION** (gras majuscules + paragraphe)
9. Mission numérotée en italique
10. **DÉTAIL DES PRESTATIONS** (tableau 4 colonnes)
11. Total HT + Total TTC
12. **LISTE DES DOCUMENTS ET RENSEIGNEMENTS À FOURNIR**
13. **CONDITIONS** (modalités de paiement, débours, TVA, périmètre, confidentialité)
14. Séparateur `* * *`
15. Phrase "bon pour accord"
16. Formule de politesse

---

## TYPE 6 — Consultation par modules

**Déclencheur :** Mission très complexe avec plusieurs axes thématiques :
résidence fiscale, structuration société, exit tax, gestion patrimoniale —
typiquement les projets d'installation à l'étranger, d'Aliyah, ou de
restructuration patrimoniale d'envergure.

**Particularités :**
- Phrase de transition obligatoire :
  > "Cette mission s'articulera autour des modules suivants :"
- **Modules numérotés** : Module 1 —, Module 2 —, etc. (titres en gras)
- Chaque module contient :
  - Titre descriptif
  - Paragraphe d'explication
  - Sous-points avec tiret (—)
- Remise d'une note finale structurée + rétroplanning opérationnel
- **Honoraires par module** avec montant ou XXXX si non encore fixés + total global
- Les frais tiers (expert-comptable, valorisation de titres) exclus du forfait
  et refacturés sur justificatifs — le mentionner explicitement
- Pas de tableau formel
- Formule de politesse : "distinguées"

**Formule de transition vers les honoraires :**
> "Conformément aux usages de ma pratique, mes honoraires seront calculés sur la
> base du temps consacré à votre dossier, au taux horaire de [TAUX_CONFIG] € HT
> (auquel s'ajoute la TVA au taux de 20 %).
> Toutefois, compte tenu de la difficulté d'anticiper précisément le temps
> nécessaire à la réalisation de cette consultation, à l'analyse des différents
> schémas envisagés et aux formalités [...], je vous propose une facturation
> forfaitaire, modulable selon les modules retenus, selon le détail suivant :"

**Structure :**
1. En-tête + logo
2. Destinataire
3. Mention confidentialité + "Par email"
4. Ville + date
5. Objet
6. Formule d'appel
7. Accroche + contexte
8. **Modules numérotés** (titres gras + tirets)
9. Note finale + rétroplanning mentionnés
10. Formule de transition honoraires
11. Honoraires par module + total global
12. Mention frais tiers exclus
13. Phrase "bon pour accord"
14. Formule de politesse

---

## Cas particulier — Référence dossier

Si le cabinet utilise un système de référence dossier, ajouter sous la date :
```
Nos Réf. : [REFERENCE] / [M./Mme NOM_CLIENT]
```
À inclure si mentionné dans CONFIG.md > INSTRUCTIONS ou si demandé par l'avocat.
