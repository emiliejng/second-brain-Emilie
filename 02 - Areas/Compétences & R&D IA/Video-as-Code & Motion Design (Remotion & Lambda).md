---
type: competence
domaine: Frontend, Motion Design & Cloud Rendering
niveau: Expert / Spécialiste
tags:
  - competences
  - remotion
  - video-as-code
  - react
  - typescript
  - aws-lambda
  - motion-design
---

# 🎬 Compétence : Video-as-Code & Motion Design (Remotion & Lambda)

## 🎯 Définition & Périmètre

Le paradigme de **Video-as-Code** consiste à concevoir et générer des contenus vidéo au pixel et à la frame près en utilisant des technologies web modernes (**React, TypeScript, CSS, Canvas**), en lieu et place des logiciels de montage classiques (Premiere, After Effects). Cette approche permet d'automatiser entièrement la production vidéo à l'échelle via des pipelines programmatiques.

---

## 🛠️ Savoirs & Outils Maîtrisés

1. **Architecture & Composition Remotion (React/TypeScript) :**
   - Structuration de compositions vidéo modulaires (`<Composition>`, `<Sequence>`, `<Series>`).
   - Synchronisation absolue au millième de seconde entre les flux vidéo externes, les sous-titres typographiques et les pistes audio.
   - Utilisation rigoureuse des composants natifs (`<Img>`, `<Audio>`, `<Video>`) garantissant le préchargement des médias avant le rendu.
2. **Bibliothèque de Motion Design Onepoint :**
   - Développement en code de transitions animées vectorielles personnalisées (`o-wipe`, `arc-sweep`, `dot-punch`, `donut-iris`, `only-the-o`).
   - Application programmatique de l'effet **Ken Burns** (pan & zoom sur images fixes avec 6 mouvements calculés dynamiquement).
   - Animation de KPI et graphiques façon *AnimStats* (count-up dramatique, ressorts physiques, révélation mot par mot).
3. **Rendu Distribué dans le Cloud (Remotion Lambda) :**
   - Déploiement et orchestration d'une infrastructure de rendu serverless sur **AWS Lambda** avec stockage temporaire sur **AWS S3**.
   - Parallélisation massive : chaque morceau de la vidéo est calculé par une instance Lambda distincte puis réassemblé dans un fichier MP4 final.
   - Optimisation des coûts : exploitation du *Free Tier* AWS (1M d'invocations gratuites/mois), générant un coût de calcul négligeable (0.04 $ sur toute la durée du stage).
4. **Player Réactif Côté Navigateur :**
   - Intégration du composant `<Player>` Remotion permettant une prévisualisation instantanée et interactive dans l'application web sans dépendance serveur.

---

## 💼 Projets OnePoint Associés
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT01 - Agent Video Propale Remotion Lambda|FT01 — Agent Vidéo Propale (ScriptWriter / Ellis)]]
