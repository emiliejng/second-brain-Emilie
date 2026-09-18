---
type: source
id: SRC-004
titre: Rapport de Stage A4 & Soutenance Recherche — LIULAB Zhejiang University
auteur: Émilie Jiang
date_source: 2025-09-05
date_ingest: 2026-09-18
statut: traité & intégré
source_path: "raw/documents/rapport de stage A4.pages & raw/documents/Défense 2025.pdf"
tags:
  - source
  - zhejiang-university
  - liulab
  - research
  - gnn
  - computational-chemistry
---

# 📑 SRC-004 : Rapport de Stage A4 & Soutenance Recherche (LIULAB ZJU)

> **Fichiers sources :** `raw/documents/rapport de stage A4.pages` et `raw/documents/Défense 2025.pdf`  
> **Auteur :** Émilie Jiang  
> **Superviseurs :** Prof. Ming Liu, Xiao Xiao, Siyuan Yang (ZJU-HIC, Hangzhou, Chine).

---

## 🎯 1. Synthèse de la Source
Rapport académique complet et deck de soutenance de 14 slides documentant les 4 mois de recherche au sein du LIULAB :
- **Application :** Fusion nucléaire propre (ITER), manipulation et séparation des isotopes d'hydrogène ($^1\text{H}, ^2\text{H}, ^3\text{H}$) par cages organiques poreuses (*Science* 2019).
- **Modélisation :** Conception d'un réseau hybride associant le passage de messages directionnel 3D de DimeNet++ et l'auto-attention globale d'un Transformer à encodages positionnels.
- **Auto-supervision :** Protocole *Masked Atom Prediction* (MAP - 15 % masquage 80/10/10) inspiré de MCRT (*Chemical Science* 2025).
- **HPC :** Orchestration de 10 pipelines parallèles sous SLURM, optimisation VRAM par gradient checkpointing, analyse d'espaces latents par t-SNE.

---

## 🏗️ 2. Pages Dérivées & Mises à Jour dans le Wiki

- **Projets / Fiches Techniques :**
  - [[01 - Projects/Stage Recherche - Zhejiang University/Index du Stage Recherche ZJU|Index du Stage Recherche ZJU]]
  - [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU01 - Modele Hybride DimeNet++ Transformer & QM9|FT-ZJU01 — DimeNet++ + Transformer & Benchmark QM9]]
  - [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU02 - Pre-entrainement Auto-Supervise Masked Atom Prediction (MAP)|FT-ZJU02 — Pré-entraînement MAP & Analyse t-SNE]]
  - [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU03 - Orchestration HPC & Calcul Distribue Multi-GPU avec SLURM|FT-ZJU03 — Orchestration Multi-GPU sous SLURM]]
- **Concepts :**
  - [[02 - Areas/Compétences & R&D IA/Graph Neural Networks & Chimie Computationnelle (DimeNet++, Transformer, QM9)|GNNs & Chimie Computationnelle]]
  - [[02 - Areas/Compétences & R&D IA/Calcul Haute Performance & Distributed Deep Learning (SLURM, Multi-GPU)|Calcul Haute Performance & SLURM]]

---

## 🔗 Liens & Connexions
- [[wiki/index|📋 Index du Wiki]]
- [[wiki/log|📜 Operations Log]]
- [[01 - Projects/Stage Recherche - Zhejiang University/Index du Stage Recherche ZJU|Index Recherche ZJU]]
