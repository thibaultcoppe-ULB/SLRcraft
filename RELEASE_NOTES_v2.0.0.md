## SLRcraft v2.0.0 — Travail collaboratif (alpha)

> ⚠️ **Version alpha** — en cours de test durant l'année académique 2026-2027. L'absence de bugs ne peut pas encore être garantie : l'utilisation se fait sous la responsabilité des utilisateur·trices. Exportez régulièrement votre projet en JSON.

### 🤝 Nouveau : travail collaboratif hors ligne

- Équipe configurable (lead + co-évaluateur·trices), stratégie par étape : tout en double ou échantillon (% en double, reste réparti équitablement)
- Rounds d'évaluation par simple échange de fichiers JSON — aucun serveur, aucune connexion simultanée requise
- Double-aveugle : chaque évaluateur·trice travaille sans voir les décisions des autres
- Le lead évalue sa part directement dans son interface (aucun fichier à gérer pour lui)
- Fusion automatique des retours, consensus par article, page « Désaccords » pour l'arbitrage du lead
- Cercles de progression par évaluateur·trice sur le tableau de bord

### 🔄 Pipeline restructuré

- « Recherche documentaire » et « Import & Dédoublonnage » fusionnés en une seule étape **Recherche & Import** : chaque recherche documentée est directement liée à l'import de son fichier de résultats
- « Formulation préalable des objectifs » distinguée comme étape de cadrage, hors pipeline numéroté (7 étapes)
- Base de données en saisie libre avec suggestions (Scopus, PsycINFO, ERIC, WoS…) ; sources complémentaires (snowballing, littérature grise…) comptées séparément dans le PRISMA
- Ajout manuel intelligent : les références ajoutées en cours de screening rejoignent automatiquement la bonne file

### 📊 PRISMA 2020

- Diagramme refondu selon le standard PRISMA 2020 (Page et al., 2021) : phases Identification / Sélection / Inclusion, colonnes par voie d'identification, raisons d'exclusion dans les nœuds
- Colonnes vides masquées automatiquement (mises à jour, autres méthodes)
- Export HTML imprimable, mise en forme adaptée aux normes APA 7 (A4, noir et blanc, Times New Roman)

### 📤 Exports enrichis

- **RIS aux quatre stades du pipeline** : bases fusionnées, après dédoublonnage, éligibles titre/résumé, conservés texte intégral
- Format auteurs fiabilisé (« Nom, Prénom » multi-auteurs préservé en RIS et BibTeX)
- CSV compatible avec les évaluations collaboratives

### ✨ Interface

- Mode sombre (préférence mémorisée), interface responsive (mobile/tablette)
- Raccourcis clavier pour le screening (1/2/3, Entrée, ↑↓)
- Sauvegarde automatique configurable (10/15/30 min) vers un fichier local réécrit silencieusement (Chrome/Edge)
- Recherche et pagination dans les listes de références, glisser-déposer pour les imports
- Choix du mode de travail (seul·e / à plusieurs) dès la page d'accueil ; aide contextuelle (opérateurs booléens, fonctionnement du collaboratif) ; bouton de citation

### 🐛 Corrections

Audit complet et test de bout en bout (import → dédoublonnage → double screening → qualité → extraction → PRISMA → exports, y compris le cycle collaboratif avec conflit et arbitrage). Parmi les corrections notables :

- Dédoublonnage non destructif (les articles déjà screenés ne sont plus requalifiés) et vérification manuelle des correspondances floues, y compris pour les vagues de mise à jour
- Raisons d'exclusion correctement reportées dans le PRISMA et le CSV en mode collaboratif
- Échappement des guillemets dans les critères, équations et noms de dimensions
- Parseur CSV compatible point-virgule (exports Excel francophones) ; parseur BibTeX plus robuste (accolades imbriquées, champs ambigus)
- Sauvegarde automatique fiabilisée (l'ancienne approche par téléchargement était bloquée par les navigateurs)
- Verrous d'écriture contre les pertes de données lors de saisies rapides

### 📖 Citation

```
Coppe, T., & Delhaye, C. (2026). SLRcraft : un outil offline pour les revues systématiques de la littérature (Version 2.0.0) [Logiciel]. https://doi.org/10.5281/zenodo.19852967
```
