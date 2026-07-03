# SLRcraft

[![DOI](https://zenodo.org/badge/DOI/10.5281zenodo.19852966.svg?v=1)](https://doi.org/10.5281/zenodo.19852966)

**Votre assistant pour les revues systématiques de la littérature**

> ⚠️ **Version alpha** — SLRcraft est en cours de test durant l'année académique 2026-2027. L'absence de bugs ne peut pas encore être garantie : l'utilisation se fait sous la responsabilité des utilisateur·trices. Pensez à exporter régulièrement votre projet en JSON.

SLRcraft est une application web mono-fichier, gratuite et entièrement offline, conçue pour accompagner toutes les étapes d'une revue systématique de la littérature (RSL). Aucune installation, aucun compte, aucun serveur : ouvrez le fichier HTML dans votre navigateur et commencez à travailler.

## Fonctionnalités

**Cadrage préalable**

- **Formulation préalable des objectifs** — Question préliminaire et dimensions personnalisables, susceptibles d'évoluer au fil de la revue

**Pipeline RSL en 7 étapes**

1. **Protocole** — Critères d'inclusion (screening 1 et 2), champs d'extraction configurables, verrouillage automatique une fois le screening commencé
2. **Recherche & Import** — Documentation des recherches par base de données (équation, date), import BibTeX / RIS / CSV lié à chaque recherche, dédoublonnage par DOI, titre exact et similarité floue (coefficient de Dice > 85 %) avec vérification manuelle côte à côte
3. **Screening titre/résumé** — Évaluation critère par critère (Oui / Non / ?), sauvegarde immédiate, raccourcis clavier, notifications d'inclusion/exclusion
4. **Screening texte intégral** — Même logique, critères indépendants
5. **Évaluation qualité** — Grilles prédéfinies (MMAT, CASP qualitatif, grille quantitative éducation) ou grille personnalisée, score sur 5 étoiles
6. **Extraction de données** — Champs configurables, métadonnées pré-remplies
7. **Synthèse & PRISMA** — Diagramme de flux PRISMA 2020 conforme au standard (Page et al., 2021), détail des raisons d'exclusion, synthèse narrative

**Travail collaboratif (hors ligne)**

- Équipe configurable (lead + co-évaluateur·trices), stratégie par étape : tout en double ou échantillon (% en double, reste réparti équitablement)
- Rounds d'évaluation par échange de fichiers JSON — aucun serveur, aucune connexion simultanée requise
- Double-aveugle : chaque évaluateur·trice travaille sans voir les décisions des autres
- Fusion automatique des retours, détection des désaccords et page de résolution pour le lead
- Cercles de progression par évaluateur·trice sur le tableau de bord

**Autres fonctionnalités**

- Mise à jour de recherche : pipeline parallèle pour les nouvelles vagues avec dédoublonnage croisé et colonne PRISMA dédiée
- Ajout de sources complémentaires (snowballing, littérature grise, recherche manuelle) comptées séparément dans le PRISMA
- Sauvegarde automatique configurable (10/15/30 min) vers un fichier local
- Mode sombre, interface responsive
- Export : RIS aux quatre stades du pipeline (bases fusionnées, après dédoublonnage, éligibles titre/résumé, conservés texte intégral), CSV complet, tableau d'extraction, BibTeX des inclus, rapport PRISMA imprimable (HTML, mise en forme APA 7), projet JSON
- Import/export de projet JSON pour sauvegarde et partage

## Utilisation

1. Téléchargez le fichier `SLRcraft.html`
2. Ouvrez-le dans un navigateur moderne (Chrome, Firefox, Edge, Safari — Chrome/Edge recommandés pour la sauvegarde automatique)
3. Commencez votre revue

Les données sont stockées localement dans le navigateur (IndexedDB). Pensez à exporter régulièrement votre projet en JSON.

## Prérequis

- Un navigateur web moderne
- Rien d'autre

## Licence

Ce projet est distribué sous licence [GPL v3](https://www.gnu.org/licenses/gpl-3.0.html). Vous pouvez librement utiliser, modifier et redistribuer ce logiciel, à condition que toute version dérivée reste sous la même licence et que le code source soit accessible. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## Citation

Si vous utilisez SLRcraft dans vos travaux, merci de le citer :

```
Coppe, T., & Delhaye, C. (2026). SLRcraft : un outil offline pour les revues systématiques de la littérature (Version 2.0.0) [Logiciel]. https://doi.org/10.5281/zenodo.19852967
```

Voir le fichier [CITATION.cff](CITATION.cff) pour le format de citation structuré.

## Équipe

**Thibault Coppe** — Université libre de Bruxelles (ULB) — CRSE — Shift Research Unit
**Coralie Delhaye** — Université libre de Bruxelles (ULB) — CRSE

## Contribuer

Les contributions sont les bienvenues. Vous pouvez :

- Signaler un bug ou proposer une amélioration via les [Issues](https://github.com/thibaultcoppe-ULB/SLRcraft/issues)
- Proposer des modifications via une Pull Request
- Forker le projet pour l'adapter à vos besoins
