---
type: competence
domaine: Cloud Computing, DevOps & Sécurité
niveau: Avancé
tags:
  - competences
  - aws
  - vercel
  - serverless
  - securite
  - api-keys
---

# ☁️ Compétence : Cloud Serverless & Sécurité des Systèmes IA (AWS, Vercel)

## 🎯 Définition & Périmètre

Le déploiement en production d'applications d'IA générative et agentique requiert une architecture cloud élastique, capable d'absorber des calculs sporadiques et asynchrones lourds tout en garantissant une **sécurisation absolue des secrets (clés d'API, endpoints) et une gestion stricte des coûts d'inférence**.

---

## 🛠️ Savoirs & Outils Maîtrisés

1. **Infrastructure Serverless AWS (Lambda & S3) :**
   - Configuration de fonctions Lambda à forte allocation mémoire et processeur optimisé pour le rendu vidéo.
   - Gestion fine des rôles et politiques de sécurité **AWS IAM** pour isoler les accès aux buckets S3 et aux logs CloudWatch.
2. **Déploiement & Edge Computing sur Vercel :**
   - Déploiement d'applications Next.js complexes combinant rendu hybride (SSR, CSR) et API routes serverless.
   - Résolution de contraintes d'infrastructure : contournement de la limite de 12 fonctions serverless simultanées par fusion logique des endpoints d'orchestration.
3. **Sécurisation des Secrets & Proxification des APIs :**
   - **Règle d'or de sécurité :** Zéro clé API sensible exposée dans le bundle frontend client (Gemini, ElevenLabs, fal.ai, Anthropic, AWS).
   - Développement de **proxies d'API serveurs** pour relayer les requêtes de manière anonyme et chiffrée.
   - Détection et contournement des blocages liés aux certificats SSL d'entreprise en environnement corporate de développement local.
4. **Monitoring & Plafonds Budgétaires :**
   - Suivi fin de la consommation des tokens et des temps d'inférence GPU pour éviter les surprises de facturation lors des démonstrations client.

---

## 💼 Projets OnePoint Associés
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT01 - Agent Video Propale Remotion Lambda|FT01 — Agent Vidéo (AWS Lambda & S3)]]
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT02 - Agent Proposition Commerciale PPTX|FT02 — Agent Propale (Vercel Serverless)]]
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT09 - Generic Showroom Experience Livepoint|FT09 — Generic Showroom (Proxy Gemini sécurisé)]]

---

## 🔗 Liens Transversaux
- [[02 - Areas/Profil & Carrière/Cartographie des Compétences & Stack|⚡ Cartographie des Compétences & Stack]]
- [[02 - Areas/Compétences & R&D IA/Calcul Haute Performance & Distributed Deep Learning (SLURM, Multi-GPU)|Compétence : Calcul HPC & SLURM (Contraste Cloud vs Cluster)]]
- [[02 - Areas/Compétences & R&D IA/Video-as-Code & Motion Design (Remotion & Lambda)|Compétence : Video-as-Code & Rendu Lambda]]
- [[03 - Resources/MOC - Carte des Connaissances & Graphe|🗺️ MOC — Carte des Connaissances & Graphe]]
