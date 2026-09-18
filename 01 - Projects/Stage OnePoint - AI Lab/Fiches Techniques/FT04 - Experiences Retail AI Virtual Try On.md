---
type: fiche-technique
projet: Suite Retail AI & Virtual Try-On
categorie: Computer Vision & Generative Retail
entreprise: Onepoint (AI Lab)
date_debut: 2026-07-01
date_fin: 2026-09-17
statut: déployé en production
tags:
  - virtual-try-on
  - computer-vision
  - retail-ai
  - nextjs
  - diffusion-models
  - fashn-ai
---

# 🛍️ Fiche Technique 04 : Suite Retail AI & Virtual Try-On

> **Application en Production :** `https://experiences-retail-ai.vercel.app/demos/virtual-try-on`  
> **Rôle d'Émilie :** Développement frontend Next.js, intégration du pipeline de modèles de vision/diffusion et optimisation de l'expérience utilisateur sur borne tactile.

---

## 🎯 1. Objectif & Impact Métier
Offrir aux décideurs des secteurs Retail et Luxe une démonstration concrète de l'impact de l'IA générative sur le taux de conversion et l'engagement client. Le visiteur se prend en photo sur la borne et se voit immédiatement habillé avec les pièces de la collection, avec un rendu photoréaliste respectant sa morphologie réelle.

---

## 🛠️ 2. Ce que j'ai Conçu & Développé
- **Pipeline Génératif Multimodal :** Chaînage séquentiel haute performance : *Analyse de la morphologie et pose (Gemini Flash Lite) ➔ Génération d'environnement de style (FLUX Kontext) ➔ Transfert réaliste de vêtements sur corps humain (FASHN v1.6)*.
- **Système de Cadrage Visuel Assisté :** Conception d'un viseur graphique interactif en pied (repères visuels *"Tête ici"*, *"Pieds ici"*) avec décompte de pose étendu à 5 secondes pour maximiser la qualité du cliché source.
- **Composant de Masquage & Fusion Visuelle :** Développement d'un algorithme de fondu de contour dynamique pour fondre harmonieusement les textures textiles sur la silhouette sans effet de découpage artificiel.
- **Gestion de la Latence (Carrousels Actifs) :** Remplacement de l'écran d'attente passif par un carrousel interactif (avec boutons pause) affichant les fiches détaillées des articles (marque, prix, matières).
- **Panier Granulaire Interactif :** Implémentation d'une interface de sélection partielle des vêtements à l'écran résultat au lieu d'un ajout forcé de l'ensemble du look.

---

## 🏗️ 3. Architecture Technique

```mermaid
flowchart LR
    A["📸 Selfie Visiteur en Pied"] --> B["🧠 Analyse Morphologie (Gemini Flash Lite)"]
    B --> C["🎨 Génération Contexte (FLUX Kontext)"]
    C --> D["👗 Transfert Textile (FASHN v1.6)"]
    D --> E["✨ Masquage & Feathering Anti-Ghosting"]
    E --> F["🖥️ Borne Kiosque Next.js (Panier Sélectif)"]
```

---

## ⚡ 4. Défis Techniques Résolus (Preuves de Compétence)

| Défi Rencontré | Cause Racine Identifiée | Solution Technique Déployée |
|:---|:---|:---|
| **Artéfacts de dédoublement (ghosting)** | Mauvaise superposition des bordures entre le corps du mannequin et le vêtement généré. | **Élargissement du masque de fusion progressif (*feathering*)** et intégration d'un bouton de régénération granulaire en un clic. |
| **Mannequins non fidèles au visiteur** | La capture initiale se focalisait uniquement sur le visage, générant un corps standardisé. | Refonte du module caméra pour une **capture en pied complète** guidée par viseur géométrique respectant la silhouette réelle. |
| **Frustration liée au temps de génération** | Latence incompressible des modèles de diffusion lourds (10-15s). | Transformation du temps mort en expérience d'achat : navigation dans les détails produits et pause active sur le carrousel. |

---

## 📊 5. Métriques & Démonstrateur
- **Expérience Kiosque :** Application responsive plein écran déployée sur Vercel avec fluidité 60 fps sur bornes tactiles.
- **Fidélité textile :** Conservation rigoureuse des motifs, coutures et drapés des vêtements de marque.

---

## 🔗 Liens & Références
- [[01 - Projects/Stage OnePoint - AI Lab/Index du Stage|Index général du stage OnePoint]]
- [[02 - Areas/Compétences & R&D IA/IA Multimodale (Audio, Voix, Vidéo, Vision)|Compétence : IA Multimodale & Vision]]
- [[02 - Areas/Compétences & R&D IA/Product Building IA & Showroom Expérientiel|Compétence : Product Building & Kiosque]]
