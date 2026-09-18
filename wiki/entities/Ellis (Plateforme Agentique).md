---
type: entity
categorie: plateforme-logicielle
produit: Ellis
createur: Onepoint AI Lab (Émilie Jiang)
url_production: "https://ellis-tau.vercel.app"
technologies:
  - nextjs
  - vercel
  - anthropic-claude
  - gemini
  - remotion
  - aws-lambda
  - fal-ai
  - elevenlabs
tags:
  - entity
  - ellis
  - agentique
  - platform
  - production
---

# 🤖 Entité : Ellis (Plateforme Agentique de Vente)

> **Application déployée en production :** `https://ellis-tau.vercel.app`  
> Plateforme unifiée de vente agentique conçue par Émilie Jiang au sein de Onepoint AI Lab.

---

## 🎯 1. Fonctionnalités & Modules
1. **ScriptWriter (Agent Vidéo de la Propale) :**
   - Ingestion de brief client (PDF/texte) via Gemini.
   - Génération de vidéos commerciales haute définition (30s - 2min) par composition programmatique React (**Remotion**) et rendu distribué sans serveur (**AWS Lambda**).
2. **Pitch Builder (Agent Proposition Commerciale) :**
   - Génération de présentations PowerPoint professionnelles (`.pptx`) alignées sur la charte Onepoint et celle du prospect via **Anthropic Claude 3.5 Sonnet**.
3. **Sécurisation Cloud Serverless :**
   - 100 % des appels API tiers (fal.ai, ElevenLabs, Gemini, Anthropic, AWS) encapsulés derrière des proxies d'API serverless sur Vercel sans aucune exposition de secret côté client.

---

## 🔗 Liens & Connexions dans le Wiki
- **Fiches Techniques Associées :**
  - [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT01 - Agent Video Propale Remotion Lambda|FT01 — Agent Vidéo Propale (Remotion & Lambda)]]
  - [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT02 - Agent Proposition Commerciale PPTX|FT02 — Agent Proposition Commerciale PPTX]]
- **Entité Parente :** [[wiki/entities/OnePoint (AI Lab)|Onepoint AI Lab]]
- **Concepts Liés :**
  - [[02 - Areas/Compétences & R&D IA/Architecture Agentique & Meta-Prompting|Architecture Agentique & Meta-Prompting]]
  - [[02 - Areas/Compétences & R&D IA/Video-as-Code & Motion Design (Remotion & Lambda)|Video-as-Code & Motion Design]]
  - [[02 - Areas/Compétences & R&D IA/Cloud Serverless & Sécurité des Systèmes IA (AWS, Vercel)|Cloud Serverless & Sécurité]]
- **Catalogue :** [[wiki/index|Index du Wiki]]
