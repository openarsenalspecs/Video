# Vaultica

**Tagline:** Next-Gen Storage for Timeless Memories

Vaultica is an open-source, lightweight, and fully regeneratable photo archive and personal photobook application. It allows you to efficiently store, organize, and share your photos with minimal storage usage while preserving every detail.

---

## Features

### Core Features
- Lossless storage using **JPEG XL (.jxl)** for minimal footprint.
- Automatic **date/time archiving** (EXIF or manual override).
- **Daily / Monthly / Yearly photobook view** for memory browsing.
- **Deduplication** to avoid duplicate storage.
- **Metadata extraction & indexing** (EXIF, GPS, camera, tags).
- **Individual photo sharing** (export, email, social media).
- **Bulk export & share** by selection or date range.
- **Hybrid storage:** Local archive + optional encrypted cloud backup.
- **Calendar-style memory catalog** with thumbnail previews.
- **Full regeneration** of original photos on demand.

### Open Source / Community-Focused Features
- **Plugin/Extension Support** for:
  - New image importers (social media, RAW formats).
  - Export destinations (Instagram, Facebook, Flickr, Pinterest).
  - Custom photobook templates (PDF, slideshow, EPUB).
- **Cross-Platform Build Scripts** (Windows, macOS, Linux).
- **Docker image** for easy deployment.
- **Command-Line Interface (CLI)** for automation.
- **Localization / Multi-language support**.
- **Community contributions** for tagging, event categorization, and photobook templates.

### Advanced Archiving & Efficiency
- **Delta storage** for burst shots and edited images.
- **Thumbnail caching** for fast browsing.
- **Auto-compression profiles:** high efficiency vs fast access.
- **Smart indexing:** track favorites, events, and custom tags.

### AI & Advanced Search
- **Face recognition** for recurring people tagging.
- **Object recognition / auto-tagging** (pets, landscapes, events).
- **Date/location clustering** for event identification.

### Versioning & Rollback
- **Photo versioning** to track edits or metadata changes.
- **Undo / rollback** to original image.

### Backup & Sync
- **Incremental backup** to local NAS or cloud.
- **Peer-to-peer encrypted sync** between multiple devices.

### Developer-Focused Features
- **RESTful API** for automation and integration with other apps.
- **CLI commands** for batch import/export, regeneration, and archiving.
- **Support for additional lossless formats** (FLIF, QOI) via plugins.
- **SQLite or JSON metadata storage** for easy scripting.
- **CI/CD pipeline** for automated builds, testing, and packaging.
- **Automated testing** for import/export & lossless regeneration validation.

### Optional “Moonshot” Features
- **Memory Timelines:** Auto-generated animated timeline videos/slideshows.
- **Collaborative Albums:** Multiple contributors syncing photos in a shared repository.
- **AI Photo Restoration:** Open-source AI enhancements for old photos/scans.

---

## Installation

1. Clone the repository:
   git clone https://gitlab.com/Roxanne_Ardary/Vaultica.git
2. Follow platform-specific instructions in `/docs/INSTALL.md`.
3. Optional: Build Docker image for deployment.
4. Import your photos and start organizing your memories.

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
  - [https://roxanneardary.com/vaultica/](https://roxanneardary.com/vaultica/)

---

## License & Notice Requirements

Vaultica is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Vaultica specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Ensure attribution headers are included where applicable.
5. Submit a pull request for review.

---

## Contributors

See `notice.md` for full contributor tracking and attribution.
