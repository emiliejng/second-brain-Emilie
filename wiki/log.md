# 📜 Operations Log (`wiki/log.md`)

> Chronological, append-only ledger of all knowledge base operations (Ingest, Query, Lint, Refactor).  
> Parseable format: `## [YYYY-MM-DD] <operation> | <Title>`

---

## [2026-09-15] init | Architecture & Second Brain Initialization
- **Action :** Initial setup of Obsidian Vault repository and GitHub sync.
- **Repository :** `https://github.com/emiliejng/second-brain-Emilie.git`
- **Output :** Vault layout initialized, Git workflow configured, and core templates created.

---

## [2026-09-17] ingest | Stage M2 OnePoint AI Lab
- **Source :** `raw/documents/Contenu stage M2.docx`
- **Summary Page :** [[wiki/sources/SRC-001 - Notes de Stage M2 OnePoint]]
- **Compiled Projects :** [[wiki/projects/stage-onepoint/Index du Stage|Index du Stage OnePoint]], [[wiki/projects/stage-onepoint/FT01 - Agent Video Propale Remotion Lambda|FT01]] to [[wiki/projects/stage-onepoint/FT10 - Prospection Salons et Curation Tech|FT10]]
- **Compiled Concepts :** [[wiki/concepts/Architecture Agentique & Meta-Prompting|Architecture Agentique]], [[wiki/concepts/Video-as-Code & Motion Design (Remotion & Lambda)|Video-as-Code]], [[wiki/concepts/IA Multimodale (Audio, Voix, Vidéo, Vision)|IA Multimodale]], [[wiki/concepts/Robotique Incarnée & Informatique Ambiante (Reachy, Rokid, MuJoCo)|Robotique Incarnée]]
- **Key Contribution :** Extraction of the 10 engineering technical sheets demonstrating AI agent orchestration, Remotion serverless video rendering, Reachy Mini physics simulation, and Rokid AR glasses integration.

---

## [2026-09-17] ingest | Deck Marketing de l'Agentique Livepoint V2
- **Source :** `raw/documents/[AI LAB] Deck marketing de l'agentique livepoint V2.source.md`
- **Summary Page :** [[wiki/sources/SRC-002 - Deck Marketing Agentic Livepoint]]
- **Compiled Pages :** [[wiki/projects/stage-onepoint/Catalogue des 20 Expériences de l'Agentic Livepoint|Catalogue des 20 Expériences]], [[wiki/projects/stage-onepoint/Offre & Parcours Client — Agentic Livepoint|Offre & Parcours Client]], [[wiki/concepts/Vision Frontier Firm & Organisation Agentique|Concept Frontier Firm]]
- **Key Contribution :** Strategic business models, client journey in 4 phases (C-Level, COMEX, DSI, Métiers) and the 20 interactive demonstrators of the Agentic Livepoint.

---

## [2026-09-18] ingest | Curriculum Vitae Émilie Jiang (EN v2)
- **Source :** `raw/documents/EMILIE_JIANG_CV_EN_v2.docx`
- **Summary Page :** [[wiki/sources/SRC-003 - CV Emilie Jiang EN]]
- **Compiled Pages :** [[wiki/profile/Profil & Parcours — Émilie Jiang|Profil]], [[wiki/profile/Expériences Professionnelles|Expériences]], [[wiki/profile/Formation & Diplômes|Formation]], [[wiki/profile/Projets Phares & Recherche|Projets Phares]], [[wiki/profile/Cartographie des Compétences & Stack|Cartographie des Compétences]]
- **Key Contribution :** Full trajectory documentation: ESILV / IFT Creative Technology, CUPGE Paris Cité, Pitié-Salpêtrière clinical data, Sealy companion robot, TinyGrad to WebGPU from scratch.

---

## [2026-09-18] ingest | Stage Recherche Zhejiang University (LIULAB)
- **Source :** `raw/documents/rapport de stage A4.pages` & `raw/documents/Défense 2025.pdf`
- **Summary Page :** [[wiki/sources/SRC-004 - Rapport et Soutenance Stage Recherche ZJU]]
- **Compiled Projects :** [[wiki/projects/stage-zju/Index du Stage Recherche ZJU|Index Recherche ZJU]], [[wiki/projects/stage-zju/FT-ZJU01 - Modele Hybride DimeNet++ Transformer & QM9|FT-ZJU01]], [[wiki/projects/stage-zju/FT-ZJU02 - Pre-entrainement Auto-Supervise Masked Atom Prediction (MAP)|FT-ZJU02]], [[wiki/projects/stage-zju/FT-ZJU03 - Orchestration HPC & Calcul Distribue Multi-GPU avec SLURM|FT-ZJU03]]
- **Compiled Concepts :** [[wiki/concepts/Graph Neural Networks & Chimie Computationnelle (DimeNet++, Transformer, QM9)|GNNs & Chimie Computationnelle]], [[wiki/concepts/Calcul Haute Performance & Distributed Deep Learning (SLURM, Multi-GPU)|HPC & SLURM]]
- **Key Contribution :** Nuclear fusion application (ITER, isotope separation), DimeNet++ directional message passing coupled with Transformer attention on QM9, Masked Atom Prediction (MAP) self-supervision, and multi-GPU SLURM cluster management.

---

## [2026-09-18] refactor | Graph Restructuration & Zero-Orphan Topology
- **Action :** Elimination of all orphan nodes, cross-linking of lateral companion sheets, establishment of 8 colored graph view groups in `.obsidian/graph.json`.
- **Metrics :** Density increased from ~98 to 326 links (7.76 links/node). Total orphans reduced to 0.

---

## [2026-09-18] infra | LLM Wiki Architecture Implementation (Andrej Karpathy Pattern)
- **Action :** Implementation of the 3-Layer Karpathy Architecture (`raw/`, `wiki/`, `CLAUDE.md`, `AGENTS.md`).
- **Files Created :** `CLAUDE.md`, `AGENTS.md`, `wiki/index.md`, `wiki/log.md`, `wiki/concepts/Pattern LLM Wiki (Andrej Karpathy).md`.
- **Organization :** Setup of `raw/documents/`, `raw/assets/`, `wiki/sources/`, `wiki/entities/`, `wiki/concepts/`, `wiki/projects/`, and `wiki/profile/`.
