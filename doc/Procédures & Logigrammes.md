---
type: concept
subject: Procédures & Logigrammes
module: Module 7 — Documentation & Procédures
tags: [#procédure #logigramme #RAD #processus #documentation]
date: 2026-05-21
niveau: intermédiaire
statut: complet
analogie_domaine: Cuisine
---

# Procédures & Logigrammes

> **Analogie Cuisine :** Une recette, c'est une procédure. Elle dit exactement QUI fait QUOI, COMMENT, dans quel ORDRE. Sans recette, deux cuisiniers font le même plat différemment — avec des résultats imprévisibles. Le logigramme, c'est la version schématique : "Si la sauce est trop épaisse → ajouter du bouillon. Sinon → continuer."

---

## En une phrase simple
Une **procédure** est un mode d'emploi pas à pas pour accomplir une tâche. Un **logigramme** est sa version visuelle avec des décisions oui/non.

---

## Procédure vs Processus

| | Processus | Procédure |
|-|-----------|-----------|
| **Définition** | Ensemble d'activités qui transforment des entrées en sorties | La façon dont on met en place le processus |
| **Niveau** | Stratégique (QUOI) | Opérationnel (COMMENT) |

---

## Buts d'une procédure
- Limiter les erreurs
- Diminuer les tests de solutions à l'aveugle
- Permettre la transmission de connaissances
- Prévoir les risques
- Détailler pas à pas les tâches
- Solution stable aux situations récurrentes

## Qualités d'une bonne procédure
- **Utile** — répond à un besoin réel
- **Complète** — rien n'est oublié
- **Exacte** — techniquement correcte
- **Claire et accessible** — compréhensible par le public cible
- **Compatible** — cohérente avec les autres procédures
- **Accessible** — on peut la trouver et l'utiliser facilement

## Contenu obligatoire
**QUI** · **QUOI** · **COMMENT** · (éventuellement **QUAND**)

---

## Le logigramme

Représentation visuelle d'une procédure avec des symboles standardisés :

| Symbole | Forme | Signification |
|---------|-------|--------------|
| ⬭ | Rectangle arrondi | Début ou fin |
| ▭ | Rectangle | Action |
| ◇ | Losange | Question / Décision |

---

## Procédures utilisateurs — règles spécifiques

Quand la procédure est destinée à un utilisateur non-technicien :
- **1 action = 1 étape** (phrases courtes, verbes d'action)
- **Captures d'écran** indispensables (lisibles, annotées avec flèches)
- **Résultat attendu** : "À la fin, vous devez voir..."
- **Erreurs fréquentes** : "Si le bouton n'apparaît pas..."
- L'utilisateur doit pouvoir **réussir du premier coup sans aide**

---

## Modélisation RAD (Rôle-Activité-Diagramme)

Le RAD permet à chaque personne de ne voir que **sa colonne** (son rôle). Utile quand plusieurs personnes sont impliquées dans un processus.

---

## Connexions
- [[Rapport d'intervention]] — le rapport trace le passé, la procédure guide le futur
- [[Checklists]] — la checklist est la version condensée pour ne rien oublier
- [[ITIL — Incidents & Problèmes]] — ITIL exige des procédures reproductibles
- [[Technique de l'entonnoir]] — l'arbre de décision est un logigramme de diagnostic

---

## Questions de rappel actif

> **Q :** Quelle est la différence entre une procédure et un processus ?
> **R :** Un processus = ensemble d'activités qui transforment des entrées en sorties (le QUOI). Une procédure = la façon concrète dont on réalise ce processus (le COMMENT).

> **Q :** Cite les 3 symboles de base d'un logigramme et leur signification.
> **R :** Rectangle arrondi = début/fin · Rectangle = action · Losange = question/décision.

> **Q :** Une procédure pour un utilisateur non-technicien doit contenir quoi d'indispensable ?
> **R :** Étapes numérotées (1 action = 1 étape), captures d'écran annotées, résultat attendu ("vous devez voir..."), et les erreurs fréquentes.

---

## Pièges fréquents
- ⚠️ **Procédure trop technique pour le public** — adapter le vocabulaire au lecteur.
- ⚠️ **Pas de captures d'écran** — pour un utilisateur, c'est indispensable.
- ⚠️ **Confondre procédure et rapport** — la procédure dit COMMENT faire (futur), le rapport dit CE QUI A ÉTÉ FAIT (passé).

---

## À retenir absolument
- Procédure = mode d'emploi (COMMENT faire) · Rapport = trace (CE QUI A ÉTÉ FAIT)
- Logigramme = procédure visuelle avec décisions
- Symboles : rectangle arrondi (début/fin) · rectangle (action) · losange (décision)
- Pour les utilisateurs : 1 action = 1 étape + captures d'écran + résultat attendu
- QUI · QUOI · COMMENT · (QUAND)

## Explorer ensuite
- [[Checklists]] — la version "terrain" de la procédure
