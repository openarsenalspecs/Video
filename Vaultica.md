# Vaultica

**Next-Gen Storage for Timeless Memories**

Vaultica is an open-source, modular photo archiving and personal photobook platform designed to preserve photographs and images using the smallest practical storage footprint while maintaining the ability to regenerate archived images on demand.

Vaultica moves beyond conventional SaaS photo storage by treating the user's archive as a personal, portable data repository. The core system is designed to operate from a local hard drive, NAS, removable storage, or self-hosted environment, with optional cloud and online services available through plugins.

The architecture prioritizes storage efficiency, long-term preservation, portability, privacy, interoperability, and user ownership. Photos are organized chronologically, indexed efficiently, deduplicated where possible, and stored using modern compression technologies such as JPEG XL while preserving the ability to reconstruct the archived image.

---

## Project Goals

Vaultica is designed around several fundamental principles:

- **Minimum practical storage usage**
- **Full-quality image regeneration**
- **Local-first ownership**
- **Open-source architecture**
- **Chronological memory preservation**
- **Portable archives**
- **Efficient deduplication**
- **Metadata preservation**
- **Privacy by default**
- **Optional cloud functionality**
- **Plugin-based extensibility**
- **No mandatory SaaS dependency**
- **Long-term archival compatibility**

Vaultica should remain useful even if every external service, cloud provider, or social-media integration disappears.

---

# Architecture

Vaultica uses a modular architecture consisting of:

### Core

The Core provides the fundamental archive engine and operates independently of optional external services.

### Core Modules

Core modules provide the primary functionality required to create, maintain, browse, regenerate, and protect a Vaultica archive.

### Plugin Modules

Plugin modules extend Vaultica with optional functionality without making external services dependencies of the core archive.

This separation allows users to build anything from a simple local photo archive on a hard drive to a complete self-hosted family memory platform with cloud synchronization, AI processing, and social-media integrations.

---

# Core Modules

## 1. Archive Engine

The Archive Engine is the foundation of Vaultica.

Features:

- Create and manage photo archives.
- Import photographs and images.
- Assign every archived object a unique identifier.
- Maintain persistent relationships between files and metadata.
- Maintain archive integrity.
- Support portable archive locations.
- Support external drives and NAS storage.
- Detect missing or moved archive objects.
- Verify stored objects using cryptographic hashes.
- Maintain archive manifests.
- Support archive health checks.
- Detect corruption.
- Support archive repair and verification.
- Maintain storage statistics.

The archive should remain usable independently of the graphical interface.

---

## 2. Image Storage & Compression Module

The Image Storage Module is responsible for minimizing the physical storage requirements of the archive.

Primary capabilities:

- JPEG XL archival storage.
- Lossless image preservation.
- Configurable compression profiles.
- Efficient encoding and decoding.
- Preservation of supported image metadata.
- Original-format import.
- On-demand reconstruction.
- Temporary export generation.
- Automatic cleanup of temporary regenerated files.

Vaultica should never permanently create unnecessary duplicate versions of an image merely because a user wants to view or share it.

The storage system should distinguish between:

- Archived source object.
- Derived preview.
- Temporary regenerated image.
- Exported image.
- Edited version.

This prevents routine viewing and sharing from unnecessarily increasing archive size.

---

## 3. Deduplication Module

The Deduplication Module prevents identical content from being stored multiple times.

Features:

- Cryptographic content hashing.
- Exact duplicate detection.
- Duplicate references.
- Duplicate file identification.
- Archive-wide deduplication.
- Optional perceptual duplicate detection.
- Duplicate review before removal.
- Safe reference management.
- Storage savings reporting.

Identical images should be represented by a single underlying archive object whenever possible.

---

## 4. Regeneration Module

The Regeneration Module provides Vaultica's fundamental preservation capability.

Features:

- Regenerate archived images on demand.
- Reconstruct images into common formats.
- Preserve original dimensions.
- Preserve supported metadata.
- Generate temporary working copies.
- Generate export-ready copies.
- Validate regenerated output.
- Verify regenerated output against archive metadata.
- Batch regeneration.
- Command-line regeneration.

The archive should always distinguish between **stored archival data** and **regenerated presentation or export files**.

---

## 5. Metadata Module

The Metadata Module manages information associated with every image.

Supported metadata may include:

- Original filename.
- Date taken.
- Time taken.
- Date imported.
- Date saved.
- Camera manufacturer.
- Camera model.
- Lens information.
- Exposure information.
- Orientation.
- GPS coordinates.
- Location.
- Copyright information.
- Embedded descriptions.
- User-created tags.
- Albums.
- Events.
- Favorites.
- Ratings.
- Notes.

Vaultica should preserve original metadata whenever technically possible while allowing users to add independent archival metadata.

---

## 6. Chronological Archive Module

The Chronological Archive Module transforms a collection of images into a timeline.

Primary organization:

- Year
- Month
- Day
- Time
- Event

Features:

- Automatic date extraction.
- EXIF-based date detection.
- File-date fallback.
- Import-date fallback.
- Manual date correction.
- Time correction.
- Time-zone correction.
- Date conflict resolution.
- Undated-image queue.
- Chronological sorting.

Users should be able to browse their archive according to when photographs were taken rather than simply when they were uploaded.

---

## 7. Memory Catalog Module

The Memory Catalog is the heart of Vaultica's personal photobook experience.

Features:

- Daily memory pages.
- Monthly memory views.
- Yearly memory views.
- Lifetime timeline.
- Calendar navigation.
- Daily photo counts.
- Memory thumbnails.
- Favorite memories.
- Important dates.
- Event groupings.
- First/last photograph indicators.
- Memory highlights.
- Personal notes.
- Captions.

A user should be able to select a date such as:

**August 11**

and see photographs from August 11 across multiple years.

This allows Vaultica to become a chronological visual record of a person's life rather than merely a file-management application.

---

## 8. Personal Photobook Module

The Personal Photobook Module provides an interactive representation of the user's archive.

Features:

- Digital photobook.
- Day-by-day browsing.
- Month-by-month browsing.
- Yearly books.
- Lifetime books.
- Automatic chronological layouts.
- Captions.
- Notes.
- Event titles.
- Favorites.
- Cover images.
- Page generation.
- Printable photobooks.
- Digital photobooks.
- PDF generation.
- Slideshow generation.

Users should be able to create a photobook from:

- One day.
- Multiple days.
- A month.
- A year.
- A custom date range.
- An event.
- Selected photographs.
- Their entire archive.

---

## 9. Search & Index Module

The Search Module provides fast discovery without requiring users to manually browse the archive.

Search capabilities:

- Date.
- Time.
- Date range.
- Location.
- Camera.
- Lens.
- Filename.
- Tags.
- Events.
- Albums.
- Favorites.
- Ratings.
- Captions.
- Notes.
- Metadata.

The search index should remain lightweight and should never require storing duplicate copies of the underlying photographs.

---

## 10. Preview & Thumbnail Module

The Preview Module provides fast browsing without repeatedly decoding full-resolution photographs.

Features:

- Thumbnail generation.
- Multiple preview sizes.
- Cached previews.
- Lazy loading.
- Progressive loading.
- Preview cleanup.
- Cache rebuilding.
- Configurable cache size.
- Automatic cache eviction.

Previews should be treated as disposable derived data rather than permanent archival objects.

If a preview is deleted, Vaultica must be able to regenerate it.

---

## 11. Sharing & Export Module

The Sharing and Export Module allows users to select and distribute photographs without permanently duplicating archive data.

Selection methods:

- Single image.
- Multiple individual images.
- Entire day.
- Multiple days.
- Date range.
- Month.
- Year.
- Event.
- Album.
- Search results.
- Favorites.

Export capabilities:

- JPEG.
- PNG.
- TIFF.
- JPEG XL.
- Original supported format.
- PDF.
- Slideshow.
- Photobook.

Exports should be generated from the archive on demand.

---

## 12. Security & Privacy Module

Security is part of the core architecture.

Features:

- Local archive protection.
- Encryption support.
- Secure archive keys.
- Access controls.
- Private archives.
- Optional encrypted metadata.
- Secure temporary files.
- Secure deletion of temporary exports.
- Session management.
- Audit logging.
- Archive integrity verification.

Vaultica should not require users to upload their photographs to an external service.

---

## 13. Backup & Recovery Module

The Backup Module protects the archive against hardware failure, accidental deletion, corruption, and disaster.

Features:

- Local backup.
- External-drive backup.
- NAS backup.
- Incremental backup.
- Differential backup.
- Archive verification.
- Backup verification.
- Restore testing.
- Recovery manifests.
- Backup scheduling.
- Multiple backup destinations.
- Backup health reporting.

Vaultica should support the principle that a photograph is not considered safely archived until it exists in more than one physical location.

---

## 14. Versioning Module

Versioning allows users to preserve edits without destroying the archival source.

Features:

- Original preservation.
- Edited versions.
- Version history.
- Metadata history.
- Edit relationships.
- Version comparison.
- Restore previous version.
- Branching versions.
- Version deletion controls.

The system should avoid storing complete duplicate images when an efficient representation of the change is possible and reliable.

---

## 15. Storage Optimization Module

The Storage Optimization Module continuously evaluates archive efficiency.

Features:

- Storage usage analysis.
- Compression analysis.
- Duplicate analysis.
- Preview cache analysis.
- Unused-data detection.
- Orphan detection.
- Temporary-file cleanup.
- Compression recommendations.
- Archive optimization.
- Storage savings reports.

The module should clearly distinguish between **safe-to-remove derived data** and **irreplaceable archival data**.

---

## 16. CLI Module

Vaultica should provide a command-line interface for automation and advanced users.

Example operations:

- Import.
- Archive.
- Search.
- Tag.
- Export.
- Regenerate.
- Verify.
- Backup.
- Restore.
- Optimize.
- Deduplicate.
- Generate photobooks.
- Generate reports.
- Inspect metadata.

The CLI should provide access to core functionality without requiring the graphical application.

---

## 17. API Module

Vaultica should expose a documented API for integrations.

Capabilities may include:

- Archive management.
- Image lookup.
- Metadata retrieval.
- Search.
- Import.
- Export.
- Regeneration.
- Album management.
- Event management.
- Memory retrieval.
- Backup management.
- Plugin communication.

The API should respect the same authentication, permissions, and privacy controls as the primary application.

---

# Optional Plugin Modules

Plugins extend Vaultica without expanding the required core installation.

## Cloud Storage Plugins

Optional providers may include:

- S3-compatible storage.
- Nextcloud.
- WebDAV.
- Network storage.
- Self-hosted object storage.
- Encrypted cloud repositories.

Cloud functionality must remain optional.

Vaultica should never require a specific cloud provider to operate.

---

## Social Media Plugins

Optional plugins may provide integrations with supported platforms such as:

- Facebook.
- Instagram.
- Flickr.
- Other compatible social platforms.

Capabilities may include:

- Individual image sharing.
- Multi-image sharing.
- Album publishing.
- Caption transfer.
- Hashtag transfer.
- Date-based publishing.
- Privacy controls.

Social platforms should never become part of the core archive format.

---

## Messaging & Communication Plugins

Optional integrations may support:

- Email.
- Messaging platforms.
- Share links.
- Secure transfer.
- Local network sharing.

Images should be regenerated temporarily for transmission rather than permanently duplicated in the archive.

---

## RAW Camera Plugins

Optional RAW plugins may support additional camera formats.

Capabilities:

- RAW ingestion.
- RAW metadata extraction.
- RAW preview generation.
- RAW-to-JPEG XL archival workflows.
- Camera-specific metadata.
- RAW regeneration/export workflows.

---

## AI Metadata Plugin

AI functionality should remain optional and modular.

Potential capabilities:

- Automatic tagging.
- Object recognition.
- Scene recognition.
- Face detection.
- Face clustering.
- Landmark recognition.
- Image descriptions.
- Event identification.
- Similar-image discovery.

AI processing should support local models whenever possible so users are not required to upload personal photographs to external AI services.

---

## OCR Plugin

Optional OCR functionality may identify and index text appearing in photographs.

Capabilities:

- Document recognition.
- Text extraction.
- Searchable image text.
- Receipt recognition.
- Sign recognition.
- Scanned-photo indexing.

---

## AI Photo Restoration Plugin

Optional restoration tools may provide:

- Scratch removal.
- Noise reduction.
- Upscaling.
- Color restoration.
- Sharpening.
- Old-photo restoration.
- Scan cleanup.

Restoration output must remain separate from the archival source.

---

## Geolocation Plugin

Optional geolocation capabilities may provide:

- Reverse geocoding.
- Place-name identification.
- Map views.
- Location clustering.
- Travel timeline generation.

---

## Timeline & Storytelling Plugin

Optional storytelling capabilities may generate:

- Animated timelines.
- Memory videos.
- Slideshow presentations.
- Year-in-review videos.
- Travel stories.
- Event stories.
- Automatic visual narratives.

---

## Photobook Template Plugin

Users and contributors should be able to create custom photobook layouts.

Possible formats:

- PDF.
- Printable books.
- Digital books.
- EPUB.
- Slideshow.
- Web-based books.

Templates should be installable independently from the core application.

---

## Synchronization Plugin

Optional synchronization plugins may provide:

- Device-to-device synchronization.
- Peer-to-peer synchronization.
- Encrypted synchronization.
- LAN synchronization.
- Internet synchronization.
- Selective synchronization.
- Folder synchronization.

---

## Collaboration Plugin

Optional collaborative functionality may support:

- Shared albums.
- Family archives.
- Multiple users.
- Contributor permissions.
- Shared events.
- Shared comments.
- Collaborative tagging.
- Shared photobooks.

---

## Import Plugin Framework

The plugin architecture should allow future import sources without modifying the core archive engine.

Potential sources include:

- Local folders.
- External drives.
- Cameras.
- SD cards.
- Phones.
- Existing photo-management applications.
- Social-media exports.
- Cloud exports.
- Network shares.

---

# Storage Model

Vaultica should follow a content-addressed archival approach where practical.

Each archival object should have:

- Unique object identifier.
- Content hash.
- Storage location.
- Encoding information.
- Original format information.
- Metadata reference.
- Version information.
- Integrity information.

The database should store relationships and indexes rather than unnecessary copies of image data.

Derived content such as thumbnails, previews, regenerated exports, and temporary files should be independently identifiable and disposable.

---

# Regeneration Model

Vaultica's fundamental storage philosophy is:

**Store the smallest reliable archival representation and regenerate everything else when needed.**

The system should avoid permanently storing:

- Multiple thumbnail sizes unless configured.
- Repeated exports.
- Temporary sharing files.
- Duplicate photographs.
- Duplicate previews.
- Unnecessary converted copies.

Instead:

**Archive → Decode → Regenerate → Export**

This keeps the archive compact while retaining practical accessibility.

---

# Archive Integrity

Vaultica should provide tools to verify that an archive remains healthy over time.

Integrity capabilities:

- Hash verification.
- Object verification.
- Metadata verification.
- Archive manifest verification.
- Missing-object detection.
- Corruption detection.
- Backup verification.
- Regeneration testing.

Users should be able to periodically perform an archive health check and receive a clear report.

---

# Disaster Recovery

Vaultica should support recovery from:

- Lost computers.
- Failed hard drives.
- Lost phones.
- Accidental deletion.
- Corrupted storage.
- Natural disasters.
- Theft.
- Migration to new hardware.

The archive should be portable enough that users can restore their collection to a replacement computer or storage device without being dependent on Vaultica's servers.

---

# User Interface

The primary interface should be organized around memories rather than folders.

Primary views:

- Home.
- Today.
- Calendar.
- Timeline.
- Years.
- Months.
- Days.
- Events.
- Albums.
- Favorites.
- Search.
- Photobook.
- Storage.
- Backups.
- Settings.

The daily memory view should be one of the defining features of Vaultica.

---

# Selection System

Vaultica should provide a unified selection system throughout the application.

Users should be able to:

- Select one image.
- Select multiple individual images.
- Select all images from a day.
- Select multiple days.
- Select a date range.
- Select an entire month.
- Select an entire year.
- Select an event.
- Select search results.
- Invert selection.
- Add/remove individual photographs from a selection.

The same selection should be usable for:

- Export.
- Sharing.
- Photobook generation.
- Backup.
- Download.
- Social publishing.
- Metadata editing.

---

# Extensibility

Plugins should have access to controlled APIs for:

- Importing.
- Exporting.
- Metadata.
- Search.
- Storage.
- Regeneration.
- Events.
- Albums.
- Sharing.
- AI processing.
- Photobook generation.

Plugins should not require modification of the Vaultica core.

This allows Vaultica to evolve without turning the core application into a collection of service-specific dependencies.

---

# Cross-Platform Support

Vaultica should target:

- Windows.
- macOS.
- Linux.

Optional deployment targets may include:

- Docker.
- NAS platforms.
- Self-hosted servers.
- Web interfaces.
- Mobile companion applications.

---

# Accessibility

Vaultica should support:

- Keyboard navigation.
- Screen readers.
- Adjustable interface sizing.
- High-contrast interfaces.
- Accessible image descriptions.
- Configurable thumbnails.
- Reduced-motion preferences.
- Internationalization.

---

# Localization

Vaultica should support community-maintained translations.

Localization should cover:

- Interface text.
- Dates.
- Times.
- Calendars.
- Metadata labels.
- Export interfaces.
- Accessibility text.
- Documentation.

---

# Developer Tooling

The repository should provide:

- Automated testing.
- Unit tests.
- Integration tests.
- Storage tests.
- Regeneration tests.
- Metadata tests.
- Deduplication tests.
- Backup/restore tests.
- Plugin tests.
- API tests.
- Cross-platform build pipelines.
- GitLab CI/CD.
- Development documentation.
- Architecture documentation.

---

# Data Portability

Vaultica archives should not intentionally lock users into the application.

Users should be able to:

- Export photographs.
- Export metadata.
- Export albums.
- Export events.
- Export photobooks.
- Export archive manifests.
- Move archives between drives.
- Restore archives on another system.
- Access supported archival objects independently of the UI.

Vaultica should prioritize open, documented, and durable data structures wherever practical.

---

# Privacy

Vaultica follows a local-first privacy model.

The core application should not require:

- An account with Vaultica.
- A subscription.
- A proprietary cloud service.
- Remote processing.
- Advertising.
- Mandatory telemetry.

Optional online services should be isolated behind plugins and clearly identified to the user.

---

# Configuration

Users should be able to configure:

- Archive location.
- Backup locations.
- Compression level.
- Preview cache size.
- Thumbnail settings.
- Metadata handling.
- Deduplication behavior.
- Encryption.
- Automatic backups.
- Automatic optimization.
- Plugin permissions.
- AI processing.
- Export defaults.
- Privacy settings.

---

# Performance Goals

Vaultica should prioritize:

- Low memory usage.
- Efficient CPU utilization.
- Minimal disk usage.
- Fast thumbnail browsing.
- Lazy image decoding.
- Incremental indexing.
- Incremental backups.
- Background processing.
- Parallel processing where appropriate.
- Graceful operation with very large archives.

The architecture should be capable of supporting archives containing hundreds of thousands or millions of photographs.  

---

# Development Principles

Vaultica development should follow these principles:

1. **Core functionality must not depend on optional services.**
2. **Plugins must remain independently installable.**
3. **Archived photographs must never be unnecessarily duplicated.**
4. **Derived files should be regeneratable whenever practical.**
5. **Original archival information must be protected from destructive operations.**
6. **Privacy should be the default.**
7. **Local storage should remain a first-class deployment model.**
8. **Cloud services should remain optional.**
9. **Open and documented interfaces should be preferred.**
10. **Storage efficiency should be treated as a primary feature.**
11. **Large archives must remain practical to operate.**
12. **Every major archival operation should be verifiable.**

---

# Roadmap

## Phase 1 — Archive Foundation

- Archive Engine
- JPEG XL storage
- Metadata extraction
- Hashing
- Deduplication
- Chronological organization
- Regeneration
- SQLite indexing
- Basic CLI

## Phase 2 — Memory Experience

- Calendar
- Daily memories
- Timeline
- Search
- Favorites
- Albums
- Events
- Thumbnail caching
- Personal photobook

## Phase 3 — Sharing & Backup

- Export engine
- Batch selection
- Date-range selection
- Photobook export
- Backup engine
- NAS support
- External-drive support
- Encryption

## Phase 4 — Developer Platform

- REST API
- Plugin framework
- Plugin SDK
- Documentation
- GitLab CI/CD
- Cross-platform packaging

## Phase 5 — Optional Intelligence

- Local AI tagging
- Face clustering
- Object recognition
- OCR
- Event detection
- Similar-image discovery
- Photo restoration

## Phase 6 — Optional Connectivity

- Cloud storage plugins
- Social-media plugins
- Messaging plugins
- Synchronization plugins
- Collaboration plugins
- Mobile companion applications

---

# Feature Checklist

## Core Archive

- [ ] Archive Engine
- [ ] JPEG XL archival storage
- [ ] Lossless regeneration
- [ ] Content hashing
- [ ] Deduplication
- [ ] Metadata preservation
- [ ] Chronological organization
- [ ] Archive integrity verification
- [ ] Storage optimization
- [ ] Archive health reports

## Memory Catalog

- [ ] Daily memories
- [ ] Monthly memories
- [ ] Yearly memories
- [ ] Lifetime timeline
- [ ] Calendar view
- [ ] Events
- [ ] Albums
- [ ] Favorites
- [ ] Captions
- [ ] Notes

## Photobook

- [ ] Personal photobook
- [ ] Daily photobooks
- [ ] Monthly photobooks
- [ ] Yearly photobooks
- [ ] Custom photobooks
- [ ] PDF export
- [ ] Digital book export
- [ ] Slideshow generation
- [ ] Custom templates

## Search

- [ ] Date search
- [ ] Date-range search
- [ ] Metadata search
- [ ] Location search
- [ ] Tag search
- [ ] Event search
- [ ] Album search
- [ ] Similar-image search

## Sharing & Export

- [ ] Individual selection
- [ ] Multi-selection
- [ ] Day selection
- [ ] Date-range selection
- [ ] Month selection
- [ ] Year selection
- [ ] Event selection
- [ ] Search-result selection
- [ ] JPEG export
- [ ] PNG export
- [ ] TIFF export
- [ ] JPEG XL export
- [ ] Original-format export

## Backup

- [ ] Local backup
- [ ] External-drive backup
- [ ] NAS backup
- [ ] Incremental backup
- [ ] Backup verification
- [ ] Restore
- [ ] Disaster recovery
- [ ] Multiple backup destinations

## Optional Plugins

- [ ] Cloud storage
- [ ] Nextcloud
- [ ] S3
- [ ] Social media
- [ ] Email
- [ ] Messaging
- [ ] RAW formats
- [ ] OCR
- [ ] AI tagging
- [ ] Face clustering
- [ ] Object recognition
- [ ] Geolocation
- [ ] AI restoration
- [ ] Synchronization
- [ ] Collaboration
- [ ] Photobook templates

---

# Contributing

Contributions are welcome.

Developers are encouraged to contribute:

- Core modules.
- Plugin modules.
- Storage optimizations.
- Performance improvements.
- Importers.
- Exporters.
- Metadata support.
- UI improvements.
- Accessibility.
- Localization.
- Documentation.
- Testing.
- Security improvements.

Before implementing a new capability, contributors should determine whether it belongs in the **Core**, a **Core Module**, or an **Optional Plugin**.

Features that require external services should generally be implemented as plugins rather than incorporated into the core archive.

See `CONTRIBUTING.md` for contribution procedures and requirements.

---

# Vaultica

**Next-Gen Storage for Timeless Memories**

Vaultica is designed to make personal photo preservation independent of storage providers, subscriptions, and proprietary platforms.

**Store less. Preserve more. Regenerate when needed. Remember forever.**

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
