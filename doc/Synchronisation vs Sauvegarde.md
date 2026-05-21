---
type: concept
subject: Synchronisation vs Sauvegarde
module: Module 5 — Sauvegardes & Restauration
tags: [#synchronisation #sauvegarde #OneDrive #cloud #piège]
date: 2026-05-21
niveau: intermédiaire
statut: complet
analogie_domaine: Restauration
---

# Synchronisation vs Sauvegarde

> **Analogie Restaurant :** Synchroniser, c'est avoir un miroir en face de toi — si tu casses le miroir original, le reflet disparaît aussi. Sauvegarder, c'est prendre une PHOTO du miroir : même si l'original casse, la photo reste intacte avec la version capturée.

---

## En une phrase simple
Synchroniser = **même fichier partout** (si tu supprimes ici, ça disparaît là-bas). Sauvegarder = **copie indépendante** avec historique (protège contre la suppression).

---

## Comparaison directe

| | Sauvegarde | Synchronisation |
|-|-----------|----------------|
| **Principe** | Copie historique | Copie miroir |
| **Suppression** | Protège contre | Propage l'erreur partout |
| **Historique** | Oui (versions) | Non (ou limité) |
| **Objectif** | Récupération | Accès multi-appareil |

---

## Le piège OneDrive

> **OneDrive = synchronisation, PAS sauvegarde !**

- Modification → synchronisée partout
- Suppression → supprimée partout
- Ransomware → chiffrement synchronisé partout

Microsoft le vend comme une "garantie de sécurité" mais c'est une copie miroir.

---

## Connexions
- [[Sauvegardes — Types & stratégies]] — la vraie sauvegarde avec historique
- [[Règle 3-2-1]] — OneDrive seul ne respecte pas la 3-2-1
- [[Cyber-résilience]] — la synchronisation seule = fausse sécurité

---

## Questions de rappel actif

> **Q :** Tu utilises OneDrive pour stocker tes fichiers. Un ransomware chiffre ton PC. Tes fichiers OneDrive sont-ils en sécurité ?
> **R :** Non. OneDrive synchronise, donc le chiffrement se propage au cloud. Les fichiers chiffrés remplacent les originaux dans OneDrive. Seul le versioning (si activé) pourrait aider, mais ce n'est pas garanti.

---

## À retenir absolument
- Synchroniser ≠ Sauvegarder
- Synchro = miroir (erreurs propagées) · Sauvegarde = historique (erreurs récupérables)
- OneDrive, Google Drive en mode synchro = PAS une sauvegarde
- Toujours combiner synchro cloud + sauvegarde indépendante (3-2-1)

## Explorer ensuite
- [[Restauration & Rollback]] — comment récupérer concrètement
