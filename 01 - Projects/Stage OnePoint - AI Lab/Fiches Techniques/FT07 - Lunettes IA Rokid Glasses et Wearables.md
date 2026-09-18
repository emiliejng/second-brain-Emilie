---
type: fiche-technique
projet: Lunettes IA Rokid Glasses & Informatique Ambiante
categorie: Ambient Computing & Smart Glasses
entreprise: Onepoint (AI Lab)
date_debut: 2026-08-01
date_fin: 2026-09-17
statut: opérationnel
tags:
  - rokid-glasses
  - android
  - kotlin
  - java
  - wearables
  - ambient-computing
---

# 👓 Fiche Technique 07 : Lunettes IA Rokid Glasses & Informatique Ambiante

> **Hardwares :** Lunettes AR Rokid Glasses with Display (micro-OLED) + Montre connectée Huawei.  
> **Rôle d'Émilie :** Développement Android natif, intégration du SDK Rokid et conception de l'expérience d'affichage tête haute (*HUD*).

---

## 🎯 1. Objectif & Impact Métier
Démontrer la valeur de l'**informatique ambiante sans écran tenu en main** pour les professionnels de terrain ou les visiteurs du Lab. En captant le contexte visuel et spatial en direct, les lunettes projettent des informations augmentées (*Méta-Information*) dans le champ de vision sans rompre l'attention ni mobiliser les mains.

---

## 🛠️ 2. Ce que j'ai Conçu & Développé
- **Développement Android Natif (Java / Kotlin) :** Conception de l'application compagnon pilotant l'affichage micro-OLED transparent et les flux de capteurs.
- **Interactions Gestuelles via Branche Tactile :** Implémentation du composant `AiEventListener` sur la branche droite des lunettes (défilement vertical par swipe, sélection par tap, rejet par long-press).
- **Visite Assistée du Lab par Vision Contextuelle :** Détection automatique d'objets et de QR codes géoréférencés pour déclencher l'affichage instantané de fiches techniques tête haute et la diffusion audio spatiale.
- **Interface Slicer Verticale :** Conception d'un menu déroulant adapté à la vision périphérique, synchronisé en direct avec un curseur interactif (*SeekBar*) sur smartphone.

---

## 🏗️ 3. Architecture Technique

```mermaid
flowchart LR
    A["👓 Capteurs & Caméra Lunettes"] --> B["👆 Branche Tactile (AiEventListener)"]
    B --> C["📱 Application Android (Kotlin / Java)"]
    C --> D["🧠 Modèle Vision & Méta-Information"]
    D --> E["👁️ Affichage Tête Haute HUD Micro-OLED"]
```

---

## ⚡ 4. Défis Techniques Résolus (Preuves de Compétence)

| Défi Rencontré | Cause Racine Identifiée | Solution Technique Déployée |
|:---|:---|:---|
| **Fatigue visuelle en réalité augmentée** | Des textes trop denses ou colorés occultaient la vue du monde réel. | Design d'un **HUD monochrome épuré à fort contraste**, positionné en coin supérieur pour préserver la vision binoculaire. |
| **Contrôle sans périphérique externe** | Obligation initiale d'utiliser l'écran tactile du smartphone, cassant l'immersion. | Programmation directe des gestes de la **branche tactile des lunettes (`AiEventListener`)** pour un contrôle 100 % autonome. |

---

## 🔗 Liens & Références
- [[01 - Projects/Stage OnePoint - AI Lab/Index du Stage|Index général du stage OnePoint]]
- [[02 - Areas/Compétences & R&D IA/Robotique Incarnée & Informatique Ambiante (Reachy, Rokid, MuJoCo)|Compétence : Wearables & Smart Glasses]]
- [[01 - Projects/Stage OnePoint - AI Lab/Fiches Techniques/FT08 - Multimodal Rokid x Reachy|FT08 — Projet Multimodal : Rokid x Reachy]]
