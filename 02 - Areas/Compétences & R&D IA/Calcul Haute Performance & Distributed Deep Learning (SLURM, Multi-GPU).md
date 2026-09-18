---
type: competence
domaine: Infrastructure de Calcul & Deep Learning Distribué
niveau: Avancé / Opérationnel
tags:
  - competences
  - hpc
  - slurm
  - distributed-computing
  - multi-gpu
  - cuda
  - r&d
---

# 💻 Compétence : Calcul Haute Performance & Distributed Deep Learning (SLURM)

## 🎯 Définition & Périmètre

Le passage à l'échelle (*scaling*) de modèles d'apprentissage profond volumineux sur des graphes ou des séquences complexes nécessite la maîtrise des architectures de calcul haute performance (**HPC**). Ce domaine englobe la gestion des environnements distribués, l'ordonnancement de charges multi-GPU via **SLURM**, l'optimisation drastique de la bande passante et de la mémoire vidéo (**VRAM**), ainsi que la garantie d'une reproductibilité scientifique stricte.

---

## 🛠️ Savoirs & Méthodologies Maîtrisés

1. **Ordonnancement & Soumission Batch SLURM :**
   - Écriture de scripts de soumission `#SBATCH` paramétrant précisément nœuds, GPUs dédiés, mémoire vive (`--mem`) et cœurs CPU par tâche (`--cpus-per-task`).
   - Gestion des files d'attente prioritaires, des partitions interactives et de calcul batch de nuit.
2. **Gestion Mémoire VRAM & Optimisation du Débit :**
   - Implémentation du **Gradient Checkpointing** sous PyTorch pour recalculer à la volée les activations intermédiaires du Transformer et libérer jusqu'à 60 % de mémoire GPU.
   - Entraînement en précision mixte automatique (**PyTorch AMP / FP16**) divisant par deux l'empreinte mémoire des tenseurs.
   - Conversion de batchs disjoints en tenseurs denses masqués (`to_dense_batch`) pour supprimer les allocations mémoire redondantes.
3. **Tolérance aux Pannes & Résilience :**
   - Enregistrement systématique de checkpoints complets (`torch.save(state_dict)`) à chaque epoch.
   - Scripts d'enveloppe (*wrapper bash*) avec reprise automatique (*auto-resume*) pour prévenir les interruptions dues aux limites de temps de calcul (*walltime*).
4. **Reproductibilité Scientifique & Déterminisme :**
   - Verrouillage strict des graines aléatoires (Python, NumPy, PyTorch, CUDA cuDNN) pour garantir l'identité exacte des résultats entre exécutions multi-seeds.

---

## 💼 Réalisations & Fiches Associées

- [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU03 - Orchestration HPC & Calcul Distribue Multi-GPU avec SLURM|FT-ZJU03 — Orchestration HPC & Multi-GPU sous SLURM]]
- [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU01 - Modele Hybride DimeNet++ Transformer & QM9|FT-ZJU01 — Modèle Hybride DimeNet++ + Transformer & Benchmark QM9]]
- [[01 - Projects/Stage Recherche - Zhejiang University/Index du Stage Recherche ZJU|Index du Stage Recherche ZJU (LIULAB)]]

---

## 🔗 Liens Transversaux
- [[02 - Areas/Compétences & R&D IA/Cloud Serverless & Sécurité des Systèmes IA (AWS, Vercel)|Compétence : Cloud Serverless & Sécurité (Contraste Cloud vs Cluster HPC)]]
- [[02 - Areas/Compétences & R&D IA/Graph Neural Networks & Chimie Computationnelle (DimeNet++, Transformer, QM9)|Compétence : GNNs & Chimie Computationnelle]]
- [[02 - Areas/Profil & Carrière/Cartographie des Compétences & Stack|⚡ Cartographie des Compétences & Stack]]
- [[03 - Resources/MOC - Carte des Connaissances & Graphe|🗺️ MOC — Carte des Connaissances & Graphe]]
