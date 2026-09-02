# LifeCreator
**Create From Life.**
- HTML Mirror:  [https://roxanneardary.com/lifecreator-specification/](https://roxanneardary.com/lifecreator-specification/)  

---

## Overview

LifeCreator is an AI-powered personal memory and creative platform designed to transform everyday experiences into lasting memories and creative works. Users can capture moments through voice, text, photographs, video, and other media, organize them chronologically, and transform them into images, photo collections, videos, stories, compilations, and keepsakes.

LifeCreator treats the user's memory archive as the permanent source while treating generated media as representations and creative derivatives of that archive. Every memory, generated work, edit, compilation, and derivative can maintain its relationship to the original source, allowing users to preserve context, chronology, provenance, and creative history while retaining control over how their life is represented.

## Core Principles

- Modular architecture
- User-controlled memory and creative workflows
- Preservation of original source material
- Traceable relationships between memories and generated works
- User control over AI-generated representations
- Independent creation from generated media
- Chronological organization of personal memories
- Support for multiple media types
- Editable and reusable creative assets
- Platform-specific publishing preparation
- Long-term archival preservation
- Extensible functionality through optional modules
- Open source licensing and attribution

---

## Core Modules

### Capture Module

The Capture Module provides the primary means of recording experiences and memories.

Features include:

- Voice input
- Text input
- Photograph input
- Video input
- Audio input
- Multiple inputs within a single memory
- Automatic date and time association
- User-entered dates and times
- Location information when available and authorized
- Descriptions and contextual information
- Attachments and supporting media
- Draft memories
- Private memories
- Memory editing
- Memory deletion and archival controls

### Memory Module

The Memory Module organizes captured experiences into a persistent personal memory system.

The memory hierarchy should support:

- Moment
- Scene
- Day
- Week
- Month
- Year
- Multi-year period
- Life archive

The module should allow individual memories to belong to multiple contextual collections without requiring duplicate source material.

### Special Notes Module

The Special Notes Module allows users to identify information that requires special attention or should remain associated with a memory.

Features include:

- Personal notes
- Important events
- Milestones
- People
- Places
- Anniversaries
- Personal observations
- Instructions for future generations
- Always include designations
- Do not include designations
- User-defined importance levels

Special notes should remain distinct from AI-generated interpretations.

### Multimodal Interpretation Module

The Multimodal Interpretation Module analyzes captured material to identify useful context while maintaining a distinction between source material and AI interpretation.

Features include:

- Speech transcription
- Image analysis
- Video analysis
- Text interpretation
- Scene identification
- Event identification
- People and object recognition when enabled
- Context extraction
- Date and time interpretation
- Topic identification
- Memory relationship detection
- Searchable metadata generation

AI-generated interpretations should be identifiable as interpretations and must not silently become part of the user's factual source record.

### Daily Output Module

The Daily Output Module allows users to determine how each day is represented.

Users may independently choose:

- Single image
- Photo collection
- Video
- Multiple daily formats
- No daily output
- User-created custom output

Daily outputs should be generated from the memories and source materials associated with that day.

Users should be able to regenerate, edit, replace, or create additional daily representations without modifying the underlying memories.

### Memory Reconstruction Module

The Memory Reconstruction Module creates representations of memories using available source material.

The module should support:

- Documentary reconstruction
- Interpretive reconstruction
- Creative reconstruction
- Scene generation
- Image generation
- Video generation
- Narrative generation
- Audio representation
- User-selected generation parameters

Generated content must remain distinguishable from original source material.

### Creative Generation Module

The Creative Generation Module allows users to transform memories into original works.

Users should be able to create:

- Images
- Illustrations
- Artwork
- Short videos
- Long-form videos
- Animated scenes
- Stories
- Narratives
- Visual sequences
- Other supported creative works

Generated works should be treated as independent assets that retain a relationship to their source memories.

### Independent Creation Module

The Independent Creation Module allows any generated image, video, scene, or other creative work to become the starting point for additional creations.

Users should be able to:

- Create new artwork from generated images
- Create new videos from generated images
- Create images from generated videos
- Create videos from generated videos
- Expand individual scenes
- Create alternate interpretations
- Combine multiple generated works
- Create entirely new works from archived material

New creations must not overwrite their source assets.

### Style Module

The Style Module provides independent control over the artistic representation of memories and generated works.

Style selection may be applied to:

- Individual images
- Individual scenes
- Videos
- Daily outputs
- Monthly compilations
- Yearly compilations
- Entire collections
- Individual creative derivatives

Changing a style should create a new representation while preserving the original.

### Scene and Media Editing Module

The Scene and Media Editing Module provides user control over generated and captured media.

Features include:

- Scene editing
- Image editing
- Video editing
- Cropping
- Composition changes
- Object modification
- Background modification
- Scene expansion
- Scene removal
- Text overlays
- Captions
- Audio changes
- Narration changes
- Transition editing
- Sequence editing
- Style changes

Edits should preserve the relationship between the edited work and its source.

### Highlight and Importance Module

The Highlight and Importance Module allows users to determine which memories deserve greater representation.

Features include:

- Importance ratings
- Highlight designation
- Favorite designation
- Always include
- Never include
- Personal significance
- Event significance
- User-defined categories
- AI-suggested highlights subject to user control

AI suggestions must not override explicit user preferences.

### Compilation Module

The Compilation Module combines memories and creative works into larger representations.

Supported compilation levels include:

- Daily replay
- Weekly collection
- Monthly highlights
- Yearly compilation
- Multi-year compilation
- Life compilation

Users should be able to determine which memories, periods, people, events, styles, and media types are included.

### Daily Replay Module

The Daily Replay Module creates an interactive or linear representation of a selected day.

Features may include:

- Chronological playback
- Original media
- Generated media
- Voice recordings
- Written entries
- Special notes
- Scene transitions
- Captions
- Narration
- User-selected music
- Alternate visual representations

### Monthly Highlight Module

The Monthly Highlight Module creates a representation of a selected month based on user preferences and importance settings.

Users should be able to choose:

- Images
- Photo collections
- Video
- Stories
- Mixed-media presentations
- Multiple versions
- Artistic styles
- Duration
- Included memories

### Annual Compilation Module

The Annual Compilation Module creates comprehensive representations of a selected year.

Features include:

- Year-in-review videos
- Image collections
- Highlight reels
- Chronological presentations
- Thematic collections
- Major events
- Milestones
- User-selected memories
- Multiple artistic versions

### Provenance Module

The Provenance Module maintains the relationship between original memories and generated works.

A provenance chain may include:

- Original voice recording
- Original photograph
- Original video
- Original text
- Memory record
- AI interpretation
- Generated image
- Generated video
- User edit
- Creative derivative
- Compilation
- Social media version

The system should preserve source relationships without requiring users to expose private metadata when sharing a finished work.

### Timestamp and Metadata Module

The Timestamp and Metadata Module maintains chronological and contextual information.

Features include:

- Date
- Time
- Time zone
- Location when available and authorized
- Source timestamp
- User-adjusted timestamp
- Creation timestamp
- Modification timestamp
- Generation timestamp
- Publication timestamp
- Custom metadata

### Social Publishing Module

The Social Publishing Module prepares creative works for publication across supported social media platforms.

The module should maintain platform requirement profiles that can be updated independently of the core system.

Platform profiles may define:

- Aspect ratio
- Resolution
- Dimensions
- Maximum duration
- Minimum duration
- File size
- File format
- Image requirements
- Video requirements
- Audio requirements
- Caption requirements
- Title requirements
- Thumbnail requirements
- Subtitle requirements
- Safe areas
- Other publishing requirements

The system should generate platform-specific versions from a master creative work rather than modifying the master.

### Archive Module

The Archive Module provides long-term preservation of the user's memory and creative history.

The archive should preserve:

- Original memories
- Original media
- Generated media
- Edited media
- Creative derivatives
- Daily outputs
- Monthly compilations
- Annual compilations
- Notes
- Metadata
- Timestamps
- Provenance
- Generation history
- User modifications
- Style information
- Publishing versions

Original source material should remain recoverable independently from generated representations.

### Export Module

The Export Module allows users to create portable copies of their memories and creative works.

Supported exports may include:

- Individual memories
- Complete days
- Monthly collections
- Yearly collections
- Creative works
- Videos
- Images
- Stories
- Compilations
- Metadata
- Provenance information
- Complete archives

Exported materials should remain usable independently of the LifeCreator system whenever practical.

---

## Optional Plugin Modules

LifeCreator may support optional plugin modules that extend functionality without making those capabilities mandatory for the core system.

### Image Generation Plugin

Provides AI image generation capabilities for memories, scenes, creative derivatives, and compilations.

### Video Generation Plugin

Provides AI video generation, animation, scene expansion, and video transformation.

### Voice Generation Plugin

Provides synthetic narration and other generated voice capabilities.

### AI Narration Plugin

Creates narrated versions of memories, daily replays, compilations, and stories.

### Music Generation Plugin

Creates or applies generated music to creative works and compilations.

### Style Library Plugin

Provides additional artistic styles and user-created style collections.

### Social Platform Plugin

Adds support for specific social media platforms and their publishing requirements.

### Photo Book Plugin

Transforms memories and generated works into printable or digital photo books.

### Digital Scrapbook Plugin

Creates interactive scrapbook-style collections from memories and creative works.

### Physical Keepsake Plugin

Provides formats for physical products and other tangible memory objects.

### Local AI Plugin

Allows compatible AI generation and interpretation systems to operate locally.

### Cloud AI Provider Plugin

Allows users to connect compatible external AI generation services without making any provider part of the core system.

### Family Sharing Plugin

Allows users to selectively share memories and collections with family members or other authorized people.

### Collaborative Memories Plugin

Allows multiple authorized users to contribute to shared memories and collections.

### Multiple Language Plugin

Provides multilingual transcription, translation, narration, and creative generation.

### VR and 3D Memory Plugin

Provides immersive and three-dimensional representations of selected memories and scenes.

---

## User Control

LifeCreator must prioritize user control over automated generation.

Users should be able to:

- Review AI interpretations
- Edit memories
- Reject AI-generated interpretations
- Regenerate creative works
- Select artistic styles
- Create independent derivatives
- Preserve original media
- Determine what is included in compilations
- Control special notes
- Control publishing versions
- Export their archive
- Delete selected content
- Delete complete collections
- Control sharing
- Control connected generation services

## Source and Generated Content Separation

LifeCreator must distinguish between:

- User-provided source material
- User-written information
- AI interpretations
- AI-generated content
- User-edited content
- User-created derivative works
- Published versions

AI-generated material must not be presented as an original factual record unless the user explicitly chooses to treat it as such.

## Creative Lineage

Every creative derivative should maintain a relationship to the work from which it was created.

A user should be able to trace a finished work back through its creative lineage to the underlying memory and, where available, the original source material.

The lineage system should support branching creative histories so that multiple works can be created from the same source without overwriting one another.

## Privacy and Ownership

LifeCreator should provide users with control over their personal memory archive and the representations generated from it.

The system should support:

- Private memories
- Selective sharing
- User-controlled exports
- Source preservation
- Deletion controls
- Generation history
- Provenance controls
- Provider selection where supported
- Local processing where supported

## Core Philosophy

LifeCreator is built around the principle that **the memory is the permanent object and generated media are representations of the memory**.

A single experience may produce many images, videos, stories, artistic interpretations, compilations, and social versions without requiring the original experience to be duplicated or altered.

LifeCreator transforms the personal archive from a passive record into a creative source. Users can capture life as it happens, preserve it over time, revisit it through different representations, and continually create new works from the experiences that make up their lives.

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
  - [https://roxanneardary.com/lifecreator/](https://roxanneardary.com/lifecreator/)  

---

## License & Notice Requirements

LifeCreator is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- LifeCreator specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
