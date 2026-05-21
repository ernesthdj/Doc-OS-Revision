---
type: concept
subject: Restauration & Rollback
module: Module 5 — Sauvegardes & Restauration
tags: [#restauration #rollback #image-système #snapshot #VM]
date: 2026-05-21
niveau: intermédiaire
statut: complet
analogie_domaine: Cuisine
---

# Restauration & Rollback

> **Analogie Cuisine :** Tu as trop salé le plat. Le rollback, c'est la touche "Ctrl+Z" de la cuisine : revenir à l'état d'avant l'erreur. Si tu avais mis de côté une portion non salée (sauvegarde), tu peux la resservir. Si tu n'avais rien gardé... c'est perdu.

---

## En une phrase simple
Restaurer = **récupérer** des données depuis une sauvegarde. Rollback = **revenir** à un état précédent du système après un problème.

---

## Restauration — Les 3 niveaux

| Niveau | Quoi | Impact | Usage |
|--------|------|--------|-------|
| **Fichier** | Un seul fichier | Faible | Quotidien (fichier supprimé par erreur) |
| **Dossier** | Un dossier entier | Moyen | Incident (dossier corrompu) |
| **Système** | Image complète | Fort | Catastrophe (virus, crash OS) |

> Question clé à toujours poser : **"À quelle date je veux revenir ?"**

---

## Rollback vs Restauration vs Correction

| Action | Objectif | Quand |
|--------|----------|-------|
| **Rollback** | Revenir en arrière rapidement | Mise à jour ratée, erreur récente |
| **Correction** | Réparer le problème spécifique | Cause identifiée |
| **Analyse** | Comprendre pourquoi | Après le rétablissement |

**Ordre logique :** 1. Rollback (service OK) → 2. Analyse → 3. Correction durable

---

## Types de rollback

| Type | Mécanisme | Exemple |
|------|-----------|---------|
| **Fichier** | Corbeille, historique des versions | Récupérer un fichier supprimé |
| **Système** | Point de restauration Windows | Annuler une mise à jour défaillante |
| **VM** | Snapshot (Hyper-V / VMware) | Revenir à l'état avant un test |
| **Cloud** | Versioning | Récupérer une version précédente d'un fichier |

---

## Rollback vs Sauvegarde

| | Sauvegarde | Rollback |
|-|-----------|---------|
| **Nature** | Copie des données | Retour à un état |
| **Approche** | Préventif (long terme) | Réactif (court terme) |
| **Horizon** | Jours / semaines / mois | Minutes / heures |

> Un rollback dépend souvent d'une sauvegarde (point de restauration, snapshot, image).

---

## Quand utiliser un rollback ?

**OUI :** Mise à jour foireuse · Logiciel instable · Mauvaise manipulation · Test raté

**NON :** Problème inconnu · Rollback risqué · Données non sécurisées avant le rollback

---

## Connexions
- [[Sauvegardes — Types & stratégies]] — la restauration est la raison d'être de la sauvegarde
- [[Règle 3-2-1]] — sans 3-2-1, la restauration peut être impossible
- [[Maintenance corrective]] — restauration et rollback = formes de corrective
- [[ITIL — Incidents & Problèmes]] — rollback = action immédiate sur un incident

---

## Questions de rappel actif

> **Q :** Quelle est la différence entre restauration et rollback ?
> **R :** Restauration = récupérer des données depuis une sauvegarde (ex: fichier supprimé). Rollback = revenir à un état précédent du système entier (ex: annuler une mise à jour). Le rollback est plus global et plus immédiat.

> **Q :** Après un rollback, que faut-il faire ensuite ?
> **R :** Analyser pourquoi le problème est survenu, puis appliquer une correction durable. Le rollback rétablit le service, il ne résout pas la cause.

---

## Pièges fréquents
- ⚠️ **Restaurer sans vérifier la date** — Restaurer une version trop ancienne peut faire perdre du travail récent.
- ⚠️ **Restaurer écrase ce qui existe** — Toujours restaurer dans un dossier SÉPARÉ, puis vérifier avant de remplacer.
- ⚠️ **Croire que le rollback suffit** — Sans analyse, le même problème reviendra.

---

## À retenir absolument
- Restauration = récupérer des données · Rollback = revenir à un état système
- 3 niveaux de restauration : fichier · dossier · système complet
- Ordre : rollback → analyse → correction durable
- Une sauvegarde jamais testée en restauration = inutile
- Toujours se demander : "à quelle date je veux revenir ?"

## Explorer ensuite
- [[Reformulation & Vulgarisation]] — comment communiquer le diagnostic à l'utilisateur
