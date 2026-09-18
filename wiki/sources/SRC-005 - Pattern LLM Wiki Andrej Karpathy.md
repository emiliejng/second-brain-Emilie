---
type: source
id: SRC-005
titre: LLM Wiki — A pattern for building personal knowledge bases using LLMs
auteur: Andrej Karpathy
date_publication: 2026-04-02
date_ingest: 2026-09-18
statut: traité & intégré
source_path: "raw/documents/LLM Wiki Idea File - Andrej Karpathy.md"
tags:
  - source
  - karpathy
  - llm-wiki
  - architecture
  - pkm
---

# 📑 SRC-005 : LLM Wiki — A pattern for building personal knowledge bases using LLMs

> **Auteur :** Andrej Karpathy  
> **Type de document :** Idea File / Architecture Specification  
> **Concept clé :** Remplacement du RAG ponctuel par un wiki persistant et cumulatif en 3 couches (`raw/`, `wiki/`, `CLAUDE.md`).

---

## 🎯 1. Synthèse de la Source

Andrej Karpathy formalise une rupture méthodologique dans la gestion des bases de connaissances personnelles avec les LLMs. Contrairement aux approches dominantes (RAG, NotebookLM, ChatGPT uploads) qui redécouvrent la connaissance *from scratch* à chaque requête sans mémoire cumulative, le **LLM Wiki Pattern** délègue entièrement la tenue d'un wiki Markdown à l'agent IA :
- L'humain sélectionne et dépose les sources brutes dans `raw/` (immuable).
- L'IA lit, extrait, met à jour les fiches d'entités et de concepts, résout les contradictions et maintient l'index.
- Les réponses aux questions complexes (`query`) sont réinjectées dans le wiki lorsqu'elles produisent une valeur durable.
- Des passes de vérification régulières (`lint`) garantissent la cohérence de la base.

---

## 🔑 2. Faits & Citations Clés

> *“Instead of just retrieving from raw documents at query time, the LLM incrementally builds and maintains a persistent wiki — a structured, interlinked collection of markdown files that sits between you and the raw sources.”*

> *“The wiki is a persistent, compounding artifact. The cross-references are already there. The contradictions have already been flagged. The synthesis already reflects everything you've read.”*

> *“Obsidian is the IDE; the LLM is the programmer; the wiki is the codebase.”*

> *“The human's job is to curate sources, direct the analysis, ask good questions, and think about what it all means. The LLM's job is everything else.”*

---

## 🔄 3. Impact & Pages Mises à Jour dans le Wiki

- **Schéma Créé :** [[CLAUDE.md|Constitution & Règles Opérationnelles (CLAUDE.md)]] & [[AGENTS.md]]
- **Concept Créé :** [[wiki/concepts/Pattern LLM Wiki (Andrej Karpathy)|Pattern LLM Wiki (Andrej Karpathy)]]
- **Index Central :** [[wiki/index|Index du Wiki]] (Section Sources & Concepts)
- **Registre Chronologique :** [[wiki/log|Operations Log (wiki/log.md)]]

---

## 🔗 Liens & Connexions Graphe
- [[CLAUDE.md|Schéma Directeur : CLAUDE.md]]
- [[wiki/index|📋 Index du Wiki]]
- [[wiki/log|📜 Operations Log]]
- [[wiki/concepts/Pattern LLM Wiki (Andrej Karpathy)|Concept : Pattern LLM Wiki]]
- [[Dashboard|🏠 Dashboard Principal]]
