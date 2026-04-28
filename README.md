# SLRcraft

**Votre assistant pour les revues systématiques de la littérature**

SLRcraft est une application web mono-fichier, gratuite et entièrement offline, conçue pour accompagner toutes les étapes d'une revue systématique de la littérature (RSL). Aucune installation, aucun compte, aucun serveur : ouvrez le fichier HTML dans votre navigateur et commencez à travailler.

## Fonctionnalités

**Pipeline complet en 9 étapes**

1. **Question de recherche** — Structuration libre par dimensions personnalisables
2. **Protocole** — Critères d'inclusion (screening 1 et 2), champs d'extraction configurables, stratégie de recherche
3. **Recherche documentaire** — Documentation des recherches par base de données (équation, date, nombre de résultats)
4. **Import et dédoublonnage** — Import BibTeX, RIS, CSV. Détection des doublons par DOI, titre exact et similarité fuzzy (coefficient de Dice > 85 %) avec vérification manuelle côte à côte
5. **Screening titre/abstract** — Évaluation critère par critère (Oui / Non / ?), sauvegarde immédiate, notifications d'inclusion/exclusion
6. **Screening texte intégral** — Même logique, critères indépendants
7. **Évaluation qualité** — Grilles prédéfinies (MMAT, CASP qualitatif, grille quantitative éducation) ou grille personnalisée, score sur 5 étoiles
8. **Extraction de données** — Champs configurables, métadonnées pré-remplies
9. **Synthèse et PRISMA** — Diagramme de flux PRISMA 2020 multi-colonnes, détail des raisons d'exclusion, synthèse narrative

**Autres fonctionnalités**

- Mise à jour de recherche : pipeline parallèle pour les nouvelles recherches avec dédoublonnage croisé et colonne PRISMA dédiée
- Ajout de sources complémentaires (snowballing, littérature grise, recherche manuelle)
- Verrouillage automatique des critères une fois le screening commencé
- Export : CSV complet, tableau d'extraction, BibTeX des inclus, rapport PRISMA, projet JSON
- Import/export de projet JSON pour sauvegarde et partage

## Utilisation

1. Téléchargez le fichier `SLRcraft.html`
2. Ouvrez-le dans un navigateur moderne (Chrome, Firefox, Edge, Safari)
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
Coppe, T. (2026). SLRcraft: An offline tool for systematic literature reviews (Version 1.0.0) [Software]. https://github.com/thibaultcoppe/SLRcraft
```

Voir le fichier [CITATION.cff](CITATION.cff) pour le format de citation structuré.

## Auteur

**Thibault Coppe**
Université libre de Bruxelles (ULB) — CRSE — Shift Research Unit

## Contribuer

Les contributions sont les bienvenues. Vous pouvez :

- Signaler un bug ou proposer une amélioration via les [Issues](https://github.com/thibaultcoppe/SLRcraft/issues)
- Proposer des modifications via une Pull Request
- Forker le projet pour l'adapter à vos besoins
