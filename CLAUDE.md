# 🧠 LLM Wiki Schema & Operating Rules (`CLAUDE.md`)

> **System Constitution for the LLM Wiki Agent**  
> Based on the **LLM Wiki Pattern** conceived by **Andrej Karpathy** (2026).  
> *“Obsidian is the IDE; the LLM is the programmer; the wiki is the codebase.”*

---

## 🏛️ 1. Core Philosophy & The 3-Layer Architecture

The LLM Wiki replaces traditional query-time RAG (where knowledge is re-discovered from scratch on every question) with a **persistent, compounding knowledge base**. The LLM reads sources once, extracts structural facts, resolves contradictions, maintains cross-references, and synthesizes evolving knowledge into an interlinked network of markdown pages.

```
my-wiki/
├── raw/            --> Immutable source of truth (User curates, LLM reads only)
├── wiki/           --> Persistent compiling layer (LLM owns & maintains 100%)
│   ├── index.md    --> Content catalog & table of contents
│   ├── log.md      --> Chronological append-only operations history
│   └── ...         --> Structured wiki pages (sources, entities, concepts, projects)
├── CLAUDE.md       --> System schema & operating conventions (this file)
└── AGENTS.md       --> Agent mirror for multi-agent compatibility (Antigravity, Codex)
```

### The Three Layers:
1. **`raw/` (Raw Sources) — Immutable Ground Truth :**
   - Contains raw, unmodified source files: articles, PDFs, presentations, papers, audio/video transcripts, datasets, and local assets.
   - **Strict Rule :** The LLM **NEVER** modifies or deletes files in `raw/`. It only reads them.
2. **`wiki/` (The Compiled Wiki) — LLM-Maintained Knowledge Base :**
   - The LLM **owns this layer entirely**. It creates pages, revises them when new sources arrive, maintains cross-references, flags contradictions, and prunes stale data.
   - The user reads and explores; the LLM does the heavy lifting of bookkeeping, synthesis, and maintenance.
3. **`CLAUDE.md` / `AGENTS.md` (The Schema) — Rules of Engagement :**
   - The configuration file and operating protocol that transforms the LLM into a disciplined, autonomous knowledge base maintainer.

---

## 📁 2. Folder Taxonomy & Naming Conventions

All LLM-generated files reside strictly within `wiki/` and follow this modular taxonomy:

```
wiki/
├── index.md                  # Master content catalog (updated on every ingest/query)
├── log.md                    # Append-only chronological operation log
├── sources/                  # Syntheses of ingested raw materials (SRC-001, SRC-002...)
│   └── SRC-xxx - Title.md
├── entities/                 # Concrete actors, organizations, labs, frameworks, hardware
│   ├── Zhejiang University (LIULAB).md
│   ├── OnePoint AI Lab.md
│   ├── Ellis Platform.md
│   ├── Reachy Mini.md
│   └── Rokid Glasses.md
├── concepts/                 # Abstract theories, architectures, and domain models
│   ├── Graph Neural Networks & Molecular Learning.md
│   ├── Directional Message Passing & DimeNet++.md
│   ├── Multi-Agent Orchestration & Meta-Prompting.md
│   ├── Video-as-Code & Remotion.md
│   ├── High Performance Computing & SLURM.md
│   ├── Frontier Firm & Agentic Organization.md
│   └── LLM Wiki Pattern (Karpathy).md
├── projects/                 # Concrete deliverables, technical sheets (FT), benchmarks
│   ├── stage-onepoint/
│   │   ├── FT01 - Agent Video Propale Remotion Lambda.md
│   │   └── ... (FT02 to FT10)
│   ├── stage-zju/
│   │   ├── FT-ZJU01 - Modele Hybride DimeNet++ Transformer.md
│   │   └── ... (FT-ZJU02 to FT-ZJU03)
│   └── personal/
│       ├── Sealy Robot Companion.md
│       └── TinyGrad to WebGPU.md
└── profile/                  # Emilie's professional hub
    ├── Profil & Parcours — Émilie Jiang.md
    ├── Cartographie des Compétences & Stack.md
    └── Expériences Professionnelles.md
```

---

## ⚡ 3. The 3 Core Operations Protocols

Whenever interacting with this vault, the agent executes one of the three foundational operations:

### 📥 Protocol A : INGEST (`ingest`)
*Triggered when a new source document is added to `raw/`.*

1. **Inspection & Extraction :** Read the source thoroughly from `raw/`. Extract core thesis, facts, quantitative metrics, technical architecture, and entity mentions.
2. **Create Source Summary :** Generate `wiki/sources/SRC-xxx - <Title>.md` containing:
   - Metadata (source path, author, date, type).
   - High-density abstract and key takeaways.
   - Direct quotes or data tables.
3. **Compound & Cascade Updates across Wiki :**
   - Identify which existing `concepts/`, `entities/`, or `projects/` pages are impacted.
   - Update those pages to incorporate new insights.
   - If new facts contradict earlier sources, **explicitly flag the contradiction** with a blockquote:
     > [!WARNING] Contradiction / Revision
     > Source X states A, whereas Source Y (more recent) demonstrates B.
   - Create any new entity or concept pages that warrant their own node.
4. **Update `wiki/index.md` :** Insert the new source and all newly created or revised pages into their respective catalog sections with a 1-line summary.
5. **Log Operation in `wiki/log.md` :** Append an entry using the standard prefix:
   ```markdown
   ## [YYYY-MM-DD] ingest | <Source Title>
   - **Source :** `raw/<filename>`
   - **Summary Page :** [[wiki/sources/SRC-xxx - <Title>]]
   - **Updated Pages :** [[wiki/entities/...]], [[wiki/concepts/...]]
   - **Key Contribution :** One-line summary of newly integrated knowledge.
   ```

---

### 🔍 Protocol B : QUERY (`query`)
*Triggered when the user asks a question, requests a comparison, or explores a topic.*

1. **Catalog Lookup :** Consult `wiki/index.md` first to identify candidate pages across sources, concepts, and entities.
2. **Deep Reading & Synthesis :** Read the relevant `wiki/` pages and synthesize a comprehensive answer with explicit wikilinks citations (e.g. `[[FT01]]`, `[[SRC-001]]`).
3. **Filing Back Valuable Insights (Compounding) :**
   - If the answer produces a non-trivial comparison, a novel architecture diagram, or an original synthesis, **file it back into `wiki/`** as a permanent note (e.g. in `wiki/concepts/` or `wiki/synthesis/`).
   - Knowledge generated through discussion must never be lost in transient chat history.
4. **Log Operation in `wiki/log.md` :**
   ```markdown
   ## [YYYY-MM-DD] query | <Query Topic>
   - **Question :** <User Prompt Summary>
   - **Consulted Pages :** [[...]], [[...]]
   - **Filed Artifact :** [[wiki/...]] (if created, otherwise "Direct response")
   ```

---

### 🩺 Protocol C : LINT (`lint`)
*Triggered periodically to audit vault health, consistency, and graph density.*

1. **Contradiction Scan :** Verify that claims across different sources are harmonized or clearly flagged.
2. **Orphan Hunt :** Identify any note with 0 inbound links. Every note must be linked from at least one hub or concept.
3. **Ghost Node Detection :** Detect concepts or entities mentioned repeatedly in text that lack their own dedicated wiki page.
4. **Link Integrity :** Check for broken wikilinks or invalid targets.
5. **Research Gap Suggestions :** Formulate 2 to 3 high-value research questions or missing sources that would enrich the evolving synthesis.
6. **Log Operation in `wiki/log.md` :**
   ```markdown
   ## [YYYY-MM-DD] lint | Wiki Health Check & Gap Analysis
   - **Orphans Resolved :** [...]
   - **New Stub Pages Created :** [...]
   - **Open Gaps Identified :** [...]
   ```

---

## 📝 4. Page Formatting & Frontmatter Standards

Every page in `wiki/` MUST include standard YAML frontmatter:

```yaml
---
type: concept | entity | source | project | profile
title: Title of the Page
created: YYYY-MM-DD
last_modified: YYYY-MM-DD
sources:
  - "[[wiki/sources/SRC-001 - Title]]"
tags:
  - primary-tag
  - secondary-tag
---
```

### Standard Page Structure:
1. **Title & High-Level Abstract :** 2-3 dense sentences explaining what this page is and why it matters.
2. **Core Content :** Structured with numbered points, tables, and Mermaid diagrams. Focus on engineering proofs, mechanisms, and metrics. No fluff.
3. **Contradictions & Open Questions :** Note any contested points or areas needing deeper investigation.
4. **Cross-References (`## 🔗 Liens & Connexions Graphe`) :**
   - Upstream link to parent concept or MOC.
   - Lateral links to related entities or technical sheets.
   - Citation links to primary sources.

---

## 🛠️ 5. Tooling & Productivity Best Practices

- **Obsidian Web Clipper :** Used to clip articles directly into `raw/`.
- **Local Attachment Path :** In Obsidian Settings → Files and links, set attachment path to `raw/assets/`. Bind hotkey `Ctrl+Shift+D` to "Download attachments for current file".
- **Graph View Visuals :** Maintained via `.obsidian/graph.json` with 8 distinct color groups to visualize clusters in real time.
- **Git Compounding :** The wiki is a pure Git repository. Every batch of ingests, queries, and lints is committed with structured semantic messages (`feat(wiki)`, `ingest(...)`, `lint(...)`).
