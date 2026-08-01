# RenderSmith

Your studio for infinite worlds.

RenderSmith is a Human-in-the-Loop AI system for generating visual scenes, decomposing them into persistent named assets, and recomposing them into modular, expandable worlds. It transforms generated imagery into a structured, reusable visual system where every asset has identity, memory, and reusability across infinite environments.

Instead of generating isolated images or videos, RenderSmith builds a **persistent visual world graph** composed of named assets, modular blocks, and continuously expandable environments.

---

# 🧠 Core Concept

RenderSmith turns AI-generated media into:

- Named, persistent visual assets
- Structured scene graphs
- Modular world blocks
- Infinite spatial expansion systems
- Reusable identity-locked components

Every approved scene becomes a **reusable world seed** rather than a one-off output.

---

# 🎨 Full Feature List

## 1. Human-in-the-Loop Scene Approval System
- AI generates initial images or video scenes
- Human approves canonical scenes for persistence
- Only approved scenes enter the RenderSmith system
- Rejected outputs are regenerated or iterated

---

## 2. Scene Decomposition Engine
- Breaks approved scenes into individual assets
- Instance-level segmentation of all elements
- Semantic labeling of objects and environments
- Depth estimation and spatial relationship mapping
- Converts scenes into structured scene graphs

---

## 3. Persistent Asset System
- Each object becomes a reusable asset
- Assets are stored independently of scenes
- Includes geometry, appearance, and semantic metadata

---

## 4. Dual Representation (2D + 3D Assets)
- Multi-angle 2D canonical representations
- 3D reconstruction using NeRF / Gaussian splats / hybrid methods
- View-consistent identity preservation across angles

---

## 5. Behavior & Animation Library
- Extracted or generated motion patterns
- Reusable animation packs:
  - idle cycles
  - walking cycles
  - interaction behaviors
- Physics-based behavior tagging

---

## 6. User Naming System
- Users assign names to assets after approval
- Names act as stable semantic references
- Supports:
  - simple naming (e.g., “Mara”)
  - scoped naming (world/project-based)
  - versioned naming (Mara@v1, Mara@latest)

---

## 7. Immutable Asset Versioning
- Assets are locked after approval
- Changes create new versions instead of overwriting
- Full historical lineage is preserved

---

## 8. Asset Inheritance System
- Assets can inherit properties from parent assets
- Supports controlled variation:
  - geometry inheritance
  - material inheritance
  - animation inheritance
- Enables structured variations without duplication

---

## 9. Modular World Graph System
- Worlds are structured as connected graphs
- Composed of spatial blocks
- Supports infinite expansion in all directions

---

## 10. Modular Scene Block System
- Worlds divided into reusable blocks:
  - streets
  - interiors
  - districts
- Each block contains:
  - layout rules
  - assets
  - environmental constraints

---

## 11. Seamless World Continuity Engine
- Maintains continuity across blocks
- Ensures:
  - consistent perspective
  - lighting alignment
  - spatial coherence

---

## 12. Global World Rules Engine
- Defines world-wide constraints:
  - style
  - architecture
  - lighting
  - material palettes
- Ensures coherence across expansions

---

## 13. Procedural Variation Engine
- Generates unique but consistent environments per block
- Prevents repetition while maintaining world identity

---

## 14. Persistent Asset Injection System
- Named assets persist across all scenes and worlds
- Automatically adapted into new environments
- Maintains identity consistency

---

## 15. Semantic + Visual Search Engine
- Search assets via:
  - names
  - tags
  - embeddings
  - visual similarity
- Hybrid retrieval system

---

## 16. Scene Recomposition Engine
- Rebuild new scenes from existing assets
- Supports:
  - prompt-based composition
  - manual layout control
  - AI-assisted arrangement

---

## 17. Visual World Graph Database
- Stores assets, blocks, and worlds as interconnected graphs
- Tracks:
  - relationships
  - reuse patterns
  - version history

---

## 18. Modular Asset Injection System
- Assets can be placed into any scene or block
- Automatically adapts:
  - scale
  - lighting
  - perspective

---

## 19. Compression & Latent Storage System
- Stores assets as compact latent representations
- Includes:
  - embeddings
  - sparse geometry encoding
  - delta updates between versions

---

## 20. Cross-Scene Identity Consistency Engine
- Prevents drift in:
  - character identity
  - object structure
  - materials
- Ensures stable reuse across worlds

---

## 21. Multi-Scene Continuity System
- Tracks asset presence across multiple scenes
- Maintains narrative continuity and reuse history

---

## 22. World Building Layer
- Named worlds define structured environments:
  - Neon City
  - Forest District
  - Industrial Harbor
- Contains:
  - blocks
  - assets
  - rulesets

---

## 23. Infinite Expansion System
- Enables continuous world generation (walkable environments)
- Each new block:
  - is unique
  - remains consistent with world rules
  - maintains spatial continuity

---

## 24. API + Programmatic Access Layer
- Full programmatic access to:
  - assets
  - worlds
  - blocks
  - versions
- Enables external integrations

---

## 25. Asset Export Layer
- Export system components to external formats:
  - video renders
  - 3D asset packages
  - scene graphs
  - reusable libraries
- Compatible with external engines and pipelines

---

## 26. Provenance / Audit Trail System
- Tracks full lifecycle of assets and worlds:
  - origin scene
  - generation model version
  - approval history
  - modification lineage
- Ensures traceability and reproducibility

---

## 27. Identity Lock System
- Approved assets become immutable references
- Names always resolve to canonical versions
- Changes require version branching

---

# 🧩 System Summary

RenderSmith is a modular visual world engine where AI-generated scenes are decomposed into persistent, named, and versioned assets. These assets are organized into spatial blocks and expandable world graphs, enabling infinite, coherent, and continuously navigable environments with full identity preservation and exportability.

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/rendersmith/](https://roxanneardary.com/rendersmith/)

---

## License & Notice Requirements

RenderSmith is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- RenderSmith specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
