---
type: competence
domaine: Intelligence Artificielle & Chimie Computationnelle
niveau: Avancé / Recherche
tags:
  - competences
  - graph-neural-networks
  - dimenet-plus-plus
  - transformer
  - computational-chemistry
  - r&d
  - qm9
---

# ⚛️ Compétence : Graph Neural Networks & Chimie Computationnelle

## 🎯 Définition & Périmètre

La modélisation de systèmes moléculaires et de matériaux cristallins par l'Intelligence Artificielle requiert des architectures de réseaux de neurones capables de respecter les symétries physiques fondamentales de l'espace tridimensionnel : invariance ou équivariance aux translations et rotations euclidiennes $\text{SE}(3)$. 

Ce pôle de compétence couvre la conception d'architectures de **Deep Learning géométrique (GNNs)**, l'intégration de mécanismes d'**auto-attention globale (Transformers)** et l'apprentissage auto-supervisé pour la prédiction de propriétés quantiques et le criblage virtuel de cages moléculaires.

---

## 🛠️ Savoirs & Méthodologies Maîtrisés

1. **Réseaux de Neurones sur Graphes Géométriques 3D :**
   - **Directional Message Passing (DimeNet++) :** Projection des distances interatomiques sur une base de fonctions de Bessel radiales sphériques (RBF) et des angles de triplets de liaisons sur des harmoniques sphériques (SBF).
   - **Atomistic Line Graph Neural Networks (ALIGNN) :** Représentation double en graphe de liaisons (nœuds = atomes) et graphe de lignes (nœuds = liaisons, arêtes = angles).
2. **Couplage Hybride GNN + Transformer :**
   - Dépassement du rayon de coupure local ($r_c \approx 5.0\,\text{Å}$) par injection d'un encodeur Transformer à attention globale tous-vers-tous ($O(N^2)$).
   - Intégration d'encodages positionnels préservant la topologie moléculaire.
3. **Pré-entraînement Auto-Supervisé (Self-Supervised Learning) :**
   - Mise en œuvre du protocole **Masked Atom Prediction (MAP)** inspiré de **MCRT** (*Chemical Science* 2025) : 15 % de masquage (80 % `[MASK]`, 10 % random, 10 % identique) avec Cross-Entropy pondérée pour contrer le déséquilibre de classe de l'hydrogène.
4. **Analyse Dimensionnelle & Espaces Latents :**
   - Extraction des vecteurs de représentations moléculaires $\mathbf{z}_{\text{mol}}$ et projection non-linéaire **t-SNE** pour auditer la structuration spatiale des groupements chimiques.
5. **Benchmarks de Référence :**
   - Entraînement et validation sur **QM9** (133 886 molécules organiques stables, H, C, N, O, F) avec suivi rigoureux des métriques **MAE** et **RMSE**.

---

## 💼 Réalisations & Fiches Associées

- [[01 - Projects/Stage Recherche - Zhejiang University/Index du Stage Recherche ZJU|Index du Stage Recherche ZJU (LIULAB)]]
- [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU01 - Modele Hybride DimeNet++ Transformer & QM9|FT-ZJU01 — Modèle Hybride DimeNet++ + Transformer & Benchmark QM9]]
- [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU02 - Pre-entrainement Auto-Supervise Masked Atom Prediction (MAP)|FT-ZJU02 — Pré-entraînement Auto-Supervisé (MAP) & Analyse t-SNE]]
- [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU03 - Orchestration HPC & Calcul Distribue Multi-GPU avec SLURM|FT-ZJU03 — Orchestration HPC & Multi-GPU sous SLURM]]

---

## 🔗 Liens Transversaux
- [[02 - Areas/Profil & Carrière/Cartographie des Compétences & Stack|⚡ Cartographie des Compétences & Stack]]
- [[02 - Areas/Profil & Carrière/Projets Phares & Recherche|🚀 Projets Phares & Travaux de Recherche]]
- [[02 - Areas/Compétences & R&D IA/Calcul Haute Performance & Distributed Deep Learning (SLURM, Multi-GPU)|Compétence : Calcul Haute Performance & SLURM]]
- [[03 - Resources/MOC - Carte des Connaissances & Graphe|🗺️ MOC — Carte des Connaissances & Graphe]]
