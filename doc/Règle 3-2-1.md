---
type: concept
subject: Règle 3-2-1
module: Module 5 — Sauvegardes & Restauration
tags: [#sauvegarde #3-2-1 #stratégie #hors-site]
date: 2026-05-21
niveau: intermédiaire
statut: complet
analogie_domaine: Restauration
---

# Règle 3-2-1

> **Analogie Restaurant :** Tes recettes secrètes existent en **3 exemplaires** : le classeur dans la cuisine, une copie dans le bureau, une chez ton comptable. Sur **2 supports** : papier + clé USB. Et **1 copie hors du restaurant** : chez le comptable. Si le restaurant brûle, tes recettes survivent. C'est la règle 3-2-1.

---

## En une phrase simple
**3** copies des données · **2** supports différents · **1** copie hors site ou déconnectée. C'est une règle de **bon sens**, pas de technique.

---

## Décomposition

| Chiffre | Règle | Protection contre | Exemple |
|---------|-------|------------------|---------|
| **3** | 3 copies des données (1 originale + 2 sauvegardes) | Suppression accidentelle, corruption, mauvaise manipulation | PC + disque externe + cloud |
| **2** | 2 supports différents | Panne matérielle, défaut de fabrication, bug logiciel | NAS + disque USB |
| **1** | 1 copie hors site / déconnectée | Incendie, vol, ransomware, catastrophe locale | Cloud versionné / disque chez un proche |

---

## Connexions
- [[Sauvegardes — Types & stratégies]] — la 3-2-1 combine les types de sauvegarde
- [[Synchronisation vs Sauvegarde]] — OneDrive n'est PAS la copie 3-2-1 si c'est juste de la synchronisation
- [[Restauration & Rollback]] — la 3-2-1 n'a de sens que si la restauration est testée

---

## Questions de rappel actif

> **Q :** Explique la règle 3-2-1 avec un exemple concret pour un étudiant.
> **R :** 3 copies : fichiers sur le PC + disque externe + Google Drive. 2 supports : disque dur interne + disque externe USB. 1 hors site : Google Drive est dans le cloud, hors de l'appartement. Si le PC meurt et l'appartement brûle, les données sont sur Google Drive.

---

## Pièges fréquents
- ⚠️ **OneDrive seul = pas 3-2-1** — OneDrive synchronise. Si tu supprimes un fichier, il disparaît partout. Ce n'est pas une copie indépendante.
- ⚠️ **Disque externe branché en permanence** — Un ransomware chiffre aussi les disques connectés. La copie déconnectée est cruciale.

---

## À retenir absolument
- 3-2-1 = règle de bon sens, pas de technique
- 3 copies · 2 supports · 1 hors site/déconnectée
- Protège contre : erreur humaine + panne matérielle + catastrophe locale

## Explorer ensuite
- [[Synchronisation vs Sauvegarde]] — pourquoi OneDrive n'est PAS une sauvegarde
