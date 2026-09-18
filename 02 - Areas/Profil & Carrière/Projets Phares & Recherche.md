---
type: projets-recherche
tags:
  - projets
  - sealy
  - tinygrad
  - webgpu
  - esp32
  - kickstarter
---

# 🚀 Projets Phares & Travaux de Recherche — Émilie Jiang

## 🧪 1. IA Moléculaire & GNNs — LIULAB Zhejiang University (2025)
> **Mots-clés :** *Graph Neural Networks (GNNs), DimeNet++, Transformers, Auto-Attention Globale, Masked Atom Prediction (MAP), Benchmark QM9, HPC SLURM, Fusion Nucléaire.*

- **Vision :** Accélérer la découverte de matériaux et cages poreuses pour la séparation des isotopes d'hydrogène (H, D, T) au service de l'énergie de fusion nucléaire propre (ITER), inspiré des travaux de Liu et al. (*Science* 2019).
- **Architecture Hybride Développée :**
  - Fusion d'un encodeur spatial 3D **DimeNet++** (passage de messages directionnel basé sur bases de Bessel et harmoniques sphériques) et d'un encodeur **Transformer** avec encodages positionnels pour capturer simultanément la géométrie locale 3D et les interactions stériques/électroniques à longue portée ($O(N^2)$).
  - Validation sur le benchmark de référence **QM9** (133 886 molécules organiques).
- **Pré-entraînement Auto-Supervisé (MAP) :**
  - Protocole de masquage probabiliste (15 % masquage : 80/10/10) inspiré de MCRT (*Chemical Science* 2025) pour apprendre des représentations latentes transférables sans dépendance aux calculs DFT coûteux.
  - Projection et analyse de l'espace latent par réduction dimensionnelle **t-SNE**.
- **Calcul Distribué Haute Performance :**
  - Déploiement de 10 pipelines expérimentaux sous ordonnanceur **SLURM** sur supercalculateur GPU, gestion d'erreurs OOM via gradient checkpointing et apprentissage déterministe multi-seeds.
- **Documentation complète :** [[01 - Projects/Stage Recherche - Zhejiang University/Index du Stage Recherche ZJU|Consulter le hub de recherche ZJU]]  
  - [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU01 - Modele Hybride DimeNet++ Transformer & QM9|FT-ZJU01 — Architecture Hybride DimeNet++ + Transformer & Benchmark QM9]]  
  - [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU02 - Pre-entrainement Auto-Supervise Masked Atom Prediction (MAP)|FT-ZJU02 — Pré-entraînement Auto-Supervisé (MAP) & Analyse t-SNE]]  
  - [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU03 - Orchestration HPC & Calcul Distribue Multi-GPU avec SLURM|FT-ZJU03 — Orchestration HPC & Multi-GPU sous SLURM]]

---

## 🤖 2. Sealy — Robot Compagnon IA pour la Productivité (2025 – 2026)
> **Mots-clés :** *Fatigue detection, Vigilance, Facteurs humains, Charge cognitive, Vision par ordinateur, Prototypage physique.*

- **Vision :** Conception d'un robot de bureau compagnon autonome dédié au bien-être et à la concentration au travail.
- **Intelligence & Vision (PyTorch) :** Développement de 3 algorithmes distincts de vision par ordinateur fonctionnant en temps réel :
  1. *Détection de la fatigue et de la somnolence :* Analyse des micro-mouvements oculaires, fréquence de clignement et bâillements.
  2. *Estimation de la posture corporelle :* Détection des affaissements dorsaux et de l'alignement cervical.
  3. *Détection des distractions :* Reconnaissance visuelle de l'utilisation du smartphone en phase de travail profond.
- **Ingénierie Matérielle & Form Factor :**
  - Modélisation 3D complète sous **Autodesk Fusion 360** et **Blender** pour itérer sur la morphologie et l'intégration des capteurs.
  - Prototypage rapide par impression 3D et assemblage mécatronique.
- **Étude Utilisateur & IHM :**
  - Conduite d'une étude d'ergonomie complète en conditions réelles : recueil des retours qualitatifs/quantitatifs, tests d'utilisabilité et raffinement de la boucle de rétroaction non-intrusive (signaux discrets vs alertes sonores).

---

## ⚡ 3. Deep Learning — MNIST from Scratch : TinyGrad ➔ WebGPU (2025)
> **Mots-clés :** *Deep learning from scratch, TinyGrad, WebGPU, Inférence edge dans le navigateur, Visualisation temps réel.*

- **Objectif :** Maîtriser les fondations algorithmiques du Deep Learning sans dépendre des couches d'abstraction lourdes (framework minimaliste **TinyGrad** développé par George Hotz).
- **Entraînement :**
  - Implémentation et entraînement de modèles de réseaux de neurones (MLP et CNN) *from scratch* sur le benchmark MNIST (70 000 images de chiffres manuscrits).
  - Gestion manuelle des tenseurs, rétropropagation du gradient et optimisation des hyperparamètres.
- **Inférence Client via WebGPU :**
  - Compilation et export des poids de modèle entraînés vers l'API moderne **WebGPU**.
  - Développement d'une application web interactive où l'utilisateur dessine un chiffre sur un canvas et observe en temps réel (latence < 5 ms) la mise à jour des probabilités de classe et des cartes d'activation du réseau.

---

## 📦 4. Quickstarter — Campagne & Produit Kickstarter (2024 – 2025)
> **Mots-clés :** *Product management, Design direction, Recherche utilisateur, Financement participatif.*

- Lancement et gestion d'une campagne de financement participatif sur la plateforme **Kickstarter**.
- Définition complète de la direction artistique, de la charte graphique et de l'identité de marque.
- Réalisation d'entretiens qualitatifs utilisateurs, synthèse des attentes et itérations sur les spécifications du produit final.

---

## 📡 5. Arduino / ESP32 + Dashboard WebSocket Temps Réel (2024)
> **Mots-clés :** *IoT, Systèmes embarqués, WebSockets, Télémesure temps réel.*

- Architecture d'un banc de mesure IoT reliant un microcontrôleur **ESP32 / Arduino** à un dashboard web moderne (HTML5 / CSS3 / JavaScript).
- Communication bidirectionnelle à très faible latence via protocole **WebSocket**.
- Télémétrie de capteurs en temps réel avec graphiques dynamiques et commandes de relais matériels à distance.

---

## 🔗 Liens
- [[02 - Areas/Profil & Carrière/Profil & Parcours — Émilie Jiang|Retour au profil]]
- [[02 - Areas/Profil & Carrière/Cartographie des Compétences & Stack|Cartographie des compétences]]
