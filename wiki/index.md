---
type: index
titre: Index du Wiki & Catalogue des Connaissances
statut: actif
last_updated: 2026-09-18
tags:
  - index
  - table-of-contents
  - catalog
  - llm-wiki
---

# 📋 Index du Wiki & Catalogue Général des Connaissances

> **Catalogue structuré du LLM Wiki (Architecture Andrej Karpathy).**  
> Ce catalogue recense l'intégralité des pages compilées du wiki avec leur lien direct, leur catégorie et leur résumé en une ligne.  
> *L'agent LLM consulte cet index en premier lieu avant toute opération de requête (`query`) ou d'ingestion (`ingest`).*

---

## 📑 1. Sources Brutes Ingestées (`wiki/sources/`)

| Identifiant | Document Source | Résumé en Une Ligne | Statut |
|:---|:---|:---|:---:|
| [[wiki/sources/SRC-001 - Notes de Stage M2 OnePoint\|SRC-001]] | `Contenu stage M2.docx` | Journal de bord technique et spécifications d'implémentation du stage Onepoint AI Lab (Ellis, Remotion, Rokid, Reachy). | ✅ Intégré |
| [[wiki/sources/SRC-002 - Deck Marketing Agentic Livepoint\|SRC-002]] | `Deck marketing livepoint V2.pptx` | Présentation stratégique de l'Agentic Livepoint, parcours client en 4 phases, 20 démonstrateurs et concept Frontier Firm. | ✅ Intégré |
| [[wiki/sources/SRC-003 - CV Emilie Jiang EN\|SRC-003]] | `EMILIE_JIANG_CV_EN_v2.docx` | Curriculum vitae certifié en anglais : diplômes ESILV/IFT/CUPGE, expériences professionnelles, publications et stack. | ✅ Intégré |
| [[wiki/sources/SRC-004 - Rapport et Soutenance Stage Recherche ZJU\|SRC-004]] | `rapport stage A4.pages` & `Défense 2025.pdf` | Rapport de recherche et soutenance sur le modèle hybride DimeNet++ Transformer, MAP et benchmark QM9 au LIULAB (ZJU). | ✅ Intégré |
| [[wiki/sources/SRC-005 - Pattern LLM Wiki Andrej Karpathy\|SRC-005]] | `LLM Wiki Idea File - Andrej Karpathy.md` | Spécification fondatrice d'Andrej Karpathy sur les bases de connaissances vivantes et cumulatives gérées par agents LLM. | ✅ Intégré |

---

## 💡 2. Concepts & Théories Fondamentales (`wiki/concepts/` & `02 - Areas/Compétences`)

| Note Conceptuelle | Résumé Fondamental en Une Ligne |
|:---|:---|
| [[wiki/concepts/Pattern LLM Wiki (Andrej Karpathy)\|Pattern LLM Wiki (Andrej Karpathy)]] | Architecture en 3 couches (`raw/`, `wiki/`, `CLAUDE.md`) remplaçant le RAG par une base de code de connaissances cumulative. |
| [[02 - Areas/Compétences & R&D IA/Architecture Agentique & Meta-Prompting\|Architecture Agentique & Meta-Prompting]] | Conception de systèmes multi-agents autonomes, décomposition de tâches, prompts maîtres et garde-fous stricts. |
| [[02 - Areas/Compétences & R&D IA/Graph Neural Networks & Chimie Computationnelle (DimeNet++, Transformer, QM9)\|Graph Neural Networks & Chimie Computationnelle]] | Deep Learning géométrique 3D, bases radiales de Bessel, harmoniques sphériques et auto-attention globale sur molécules. |
| [[02 - Areas/Compétences & R&D IA/Calcul Haute Performance & Distributed Deep Learning (SLURM, Multi-GPU)\|Calcul Haute Performance & Deep Learning (SLURM)]] | Scaling multi-GPU sous Linux HPC, ordonnancement SLURM, gradient checkpointing et gestion de VRAM. |
| [[02 - Areas/Compétences & R&D IA/IA Multimodale (Audio, Voix, Vidéo, Vision)\|IA Multimodale (Audio, Voix, Vidéo, Vision)]] | Orchestration de flux croisés vision par ordinateur, modèles de diffusion, synthèse vocale et interfaces immersives. |
| [[02 - Areas/Compétences & R&D IA/Video-as-Code & Motion Design (Remotion & Lambda)\|Video-as-Code & Motion Design (Remotion & Lambda)]] | Moteur de rendu programmatique de vidéos en React/TypeScript distribué sur fonctions AWS Lambda sans serveur. |
| [[02 - Areas/Compétences & R&D IA/Robotique Incarnée & Informatique Ambiante (Reachy, Rokid, MuJoCo)\|Robotique Incarnée & Informatique Ambiante]] | Embodied AI : simulation physique sous MuJoCo, robotique Reachy Mini et affichage tête haute AR sur lunettes Rokid. |
| [[02 - Areas/Compétences & R&D IA/Product Building IA & Showroom Expérientiel\|Product Building IA & Showroom Expérientiel]] | Design et déploiement de démonstrateurs interactifs d'accueil sur kiosques Samsung Flip (55-85") pour comités exécutifs. |
| [[02 - Areas/Compétences & R&D IA/Cloud Serverless & Sécurité des Systèmes IA (AWS, Vercel)\|Cloud Serverless & Sécurité des Systèmes IA]] | Architecture cloud serverless (AWS Lambda, S3, IAM, Vercel) et sécurisation intégrale des clés d'API sans fuite frontend. |
| [[03 - Resources/Vision Frontier Firm & Organisation Agentique\|Vision : La « Frontier Firm » & l'Économie Agentique]] | Modèle de transition organisationnelle des entreprises vers des réseaux de valeur agentiques à productivité démultipliée. |

---

## 🏢 3. Entités Clés & Systèmes (`wiki/entities/`)

| Entité / Système | Rôle & Nature |
|:---|:---|
| [[wiki/entities/Zhejiang University (LIULAB)\|Zhejiang University (LIULAB)]] | Laboratoire mondial d'IA & Chimie computationnelle (séparation d'isotopes pour ITER, cages poreuses). |
| [[wiki/entities/OnePoint (AI Lab)\|Onepoint (AI Lab)]] | Cellule d'innovation IA, conception de la plateforme Ellis et animation de l'Agentic Livepoint. |
| [[wiki/entities/Ellis (Plateforme Agentique)\|Ellis (Plateforme Agentique)]] | Suite logicielle de vente agentique en production (`ellis-tau.vercel.app`) : ScriptWriter vidéo et PPTX builder. |
| [[wiki/entities/Reachy Mini (Pollen Robotics)\|Reachy Mini (Pollen Robotics)]] | Robot expressif incarné simulé sous MuJoCo et déployé comme agent modérateur de réunions. |
| [[wiki/entities/Rokid Glasses (AR Wearable)\|Lunettes AR Rokid Glasses]] | Wearable tête haute Micro-OLED programmé sous Android pour afficher en temps réel (<80ms) le flux de pensée de l'IA. |

---

## 🚀 4. Projets & Fiches Techniques (`01 - Projects/`)

### 🏢 Stage OnePoint AI Lab (M2) — Suite Ellis & Agentic Livepoint
- [[01 - Projects/Stage OnePoint - AI Lab/Index du Stage|Index Général du Stage OnePoint]] — Vue d'ensemble des 10 fiches techniques, des agents de vente et de l'Agentic Livepoint.
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT01 - Agent Video Propale Remotion Lambda|FT01 — Agent Vidéo Propale (ScriptWriter)]] — Montage automatisé Video-as-Code (Remotion, Kling 1.6, AWS Lambda).
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT02 - Agent Proposition Commerciale PPTX|FT02 — Agent Proposition Commerciale PPTX]] — Génération de decks PowerPoint via Claude 3.5 Sonnet et skills graphiques.
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT03 - Agent Veille Tech Obsidian|FT03 — Agent Veille Tech Obsidian]] — Workflow autonome GitHub Actions + Gemini 2.5 Flash alimentant le coffre.
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT04 - Experiences Retail AI Virtual Try On|FT04 — Suite Retail AI & Virtual Try-On]] — Cabine d'essayage virtuelle (Computer Vision, FLUX Kontext, FASHN v1.6).
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT05 - Vocal Playground et Comite Simule|FT05 — Vocal Playground & Comité Simulé]] — Débat contradictoire multi-experts et clonage de voix ElevenLabs (11 langues).
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT06 - Reachy Mini Robotique et MuJoCo|FT06 — Reachy Mini Robotique & MuJoCo]] — Modélisation cinématique et simulation 3D physique d'agent modérateur incarné.
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT07 - Lunettes IA Rokid Glasses et Wearables|FT07 — Lunettes AR Rokid Glasses & Wearables]] — Interface HUD Micro-OLED Android contrôlée par branche tactile.
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT08 - Multimodal Rokid x Reachy|FT08 — Projet Multimodal : Rokid x Reachy]] — Streaming WebSocket local (<80ms) synchronisant gestes du robot et HUD visuel.
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT09 - Generic Showroom Experience Livepoint|FT09 — Generic Showroom Experience]] — Application d'accueil tactile grand format sur Samsung Flip (55-85").
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT10 - Prospection Salons et Curation Tech|FT10 — Prospection Salons & Curation Tech]] — Synthèse et benchmark de salons mondiaux (VivaTech, WAIC Shanghai, Google Cloud Summit).
- [[01 - Projects/Stage OnePoint - AI Lab/Catalogue des 20 Expériences de l'Agentic Livepoint|Catalogue des 20 Expériences du Livepoint]] — Répertoire exhaustif des démonstrateurs client classés par maturité.
- [[01 - Projects/Stage OnePoint - AI Lab/Offre & Parcours Client — Agentic Livepoint|Offre & Parcours Client — Agentic Livepoint]] — Offre commerciale, tarification et parcours décisionnaire en 4 phases.

### 🧪 Stage Recherche Zhejiang University (A4) — LIULAB ZJU
- [[01 - Projects/Stage Recherche - Zhejiang University/Index du Stage Recherche ZJU|Index du Stage Recherche ZJU]] — Projet de recherche en fusion nucléaire (ITER), séparation isotopique et chimie quantique.
- [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU01 - Modele Hybride DimeNet++ Transformer & QM9|FT-ZJU01 — Architecture Hybride DimeNet++ + Transformer]] — Modélisation 3D géométrique locale et attention globale sur benchmark QM9.
- [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU02 - Pre-entrainement Auto-Supervise Masked Atom Prediction (MAP)|FT-ZJU02 — Pré-entraînement Auto-Supervisé (MAP) & t-SNE]] — Protocole de masquage probabiliste (15%) inspiré de MCRT et analyse latente 2D.
- [[01 - Projects/Stage Recherche - Zhejiang University/Fiches Techniques/FT-ZJU03 - Orchestration HPC & Calcul Distribue Multi-GPU avec SLURM|FT-ZJU03 — Orchestration HPC & Calcul Multi-GPU sous SLURM]] — Gestion de 10 pipelines parallèles sous SLURM, optimisation mémoire VRAM et checkpointing.

### 🔬 Projets Personnels & R&D
- [[02 - Areas/Profil & Carrière/Projets Phares & Recherche|Projets Phares & Recherche]] — Robot Sealy (vision somnolence, posture), Deep Learning MNIST from scratch TinyGrad WebGPU, ESP32 WebSocket, Kickstarter.

---

## 👤 5. Profil & Trajectoire Ingénieure (`02 - Areas/Profil & Carrière/`)

| Note de Profil | Contenu Clé |
|:---|:---|
| [[02 - Areas/Profil & Carrière/Profil & Parcours — Émilie Jiang\|Profil & Parcours — Émilie Jiang]] | Fiche biographique, positionnement AI Product Builder, portfolio et vision d'ingénierie. |
| [[02 - Areas/Profil & Carrière/Formation & Diplômes\|Formation & Diplômes]] | Diplôme d'Ingénieur ESILV (Creative Technology), MSc IFT, CUPGE Math-Physique Paris Cité. |
| [[02 - Areas/Profil & Carrière/Expériences Professionnelles\|Expériences Professionnelles]] | Parcours complet : OnePoint AI Lab, LIULAB Zhejiang University, Caribe Wave, Pitié-Salpêtrière. |
| [[02 - Areas/Profil & Carrière/Cartographie des Compétences & Stack\|Cartographie Complète des Compétences & Stack]] | Matrice détaillée par pôle : LLMs/Agents, Deep Learning, Video-as-Code, HPC, Web, CAO 3D. |
| [[02 - Areas/Développement Personnel & Compétences\|Hub des Domaines de Responsabilité]] | Pôle de gouvernance et standards d'excellence pour la méthode P.A.R.A. |

---

## 🧭 6. Méta-Navigation & Infrastructure du Coffre

- [[CLAUDE.md|⚙️ CLAUDE.md — Master Schema & Règles de l'Agent Wiki]]
- [[AGENTS.md|🤖 AGENTS.md — Configuration Miroir Multi-Agents]]
- [[wiki/log|📜 wiki/log.md — Registre Chronologique des Opérations]]
- [[Dashboard|🏠 Dashboard Principal]]
- [[03 - Resources/MOC - Carte des Connaissances & Graphe|🗺️ MOC — Atlas du Graphe & Carte des Connaissances]]
- [[03 - Resources/Méthode PARA|📚 Méthode P.A.R.A. (Tiago Forte)]]
- [[README|📖 README du Coffre GitHub]]
