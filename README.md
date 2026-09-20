<p align="center">
  <img src="images/metaedit-logo.png" alt="MetaEdit Plus Logo" width="128" />
</p>
<h1 align="center">MetaEdit Plus - Audio & Video Metadata Editor</h1>
<p align="center">
  <b>Edit, review, organize, and automate metadata across audio and video libraries.</b><br>
  <b>Work locally with complete staging, recovery, artwork, analysis, and batch workflows.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Freeware-green?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet/10.0/runtime"><img src="https://img.shields.io/badge/.NET-10.0-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/issues"><img src="https://img.shields.io/github/issues/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor?style=flat-square&color=orange" alt="Report Issues"></a>
</p>

**MetaEdit Plus** is a professional Windows metadata editor for audio and video collections. It combines direct field editing with reviewed batch operations, complete artwork collections, filename automation, provider-assisted identification, library analysis, import and export, ReplayGain measurement, lyrics, chapters, persistent indexes, and guarded studio jobs.

### **Key Features**

- **Batch and Per-File Editing:** Apply deliberate shared values to checked files or maintain independent staged changes for each selected file.
- **Review Before Write:** Metadata, artwork, lyrics, rules, imports, and analysis results enter one staged review path before any file is changed.
- **Auto Tag:** Identify one recording or map an album release with AcoustID, MusicBrainz, optional Discogs, and iTunes evidence.
- **Text and Filename Automation:** Transform fields, extract tags from filenames, build filenames from tags, or rearrange existing filename parts with collision checks.
- **Rule Studio:** Combine guarded conditions and ordered actions, preview every result, and save reusable local rule presets.
- **Clean & Organize:** Build resumable metadata and path plans, review conflicts, and commit through backup and rollback protection.
- **Library Health:** Find unreadable tags, missing fields, album inconsistencies, numbering problems, artwork differences, and duplicate evidence without changing media.
- **Complete Artwork Collections:** Add, replace, reorder, describe, inspect, export, and remove embedded pictures without flattening unrelated artwork.
- **Transfer and Reporting:** Review CSV or text imports and export CSV, JSON, HTML, text, and playlist documents.
- **Lyrics, Chapters, and Video Metadata:** Search and stage lyrics, edit supported chapter structures, and work with contextual video fields.
- **Loudness and ReplayGain:** Measure decoded audio and stage ReplayGain 2 track and album values without normalizing or re-encoding it.
- **Persistent Libraries and Layouts:** Index chosen folders locally, create reusable Library and editor layouts, and save field sets and container mappings.
- **Studio Automation:** Run versioned dry-run, commit, watch-folder, and redacted-diagnostics jobs from `MetaEdit.Automation.exe`.
- **Local-First Privacy:** All editing works without an account. Optional cloud sync is off by default and covers portable tag preferences only.

> **Looking for a specific workflow?** The complete feature reference below explains scope, staging, write safety, automation, supported formats, optional tools, and current boundaries.

### **Supported Formats**

- **Audio:** `MP3`, `WAV`, `FLAC`, `OGG`, `OGA`, `OPUS`, `WV`, `WMA`, `AAC`, `M4A`, `M4B`, `AIF`, `AIFF`, `APE`, `DSF`, `MKA`, `MPC`, `MPP`, `OFR`, `OFS`, `SPX`, `TAK`, `TTA`.
- **Video:** `MP4`, `MKV`, `MOV`, `WMV`, `M4V`, `WEBM`.

Metadata, artwork, and chapter support depends on the media container. MetaEdit disables unsupported write operations instead of silently dropping data.

### **Available Metadata Fields**

The editor groups 56 standard fields into five configurable sections:

- **Core:** title, subtitle/version, artist/performer, genre, BPM, initial key, album, album artist, track number and total, disc number and total.
- **Credits:** composer, conductor, performer role, description, grouping/work, remixed by, comment, lyrics.
- **Release:** release year and original release date, status, type, media type and country, publisher/label, copyright, license, ISRC, barcode, catalog number.
- **IDs & Sorting:** MusicBrainz recording, release, release group, artist, release artist and disc IDs; title, album, artist, album artist and composer sort values; Amazon catalog ID.
- **Technical:** date tagged, media length, language, encoded by, encoder settings, reference loudness, and ReplayGain track/album gain, peak and range.

Custom Fields and Format-Specific Tags handle additional supported text keys. The transfer schema also retains legacy MusicIP PUID compatibility.

## **Table of Contents**

1. [System Requirements](#system-requirements)
   - [Minimum Requirements](#minimum-requirements)
   - [Recommended Requirements](#recommended-requirements)
2. [Third-Party Libraries](#third-party-libraries)
3. [Installation](#installation)
4. [Authentication, Cloud Sync, and Privacy](#authentication-cloud-sync-and-privacy)
5. [Getting Started Guide](#getting-started-guide)
   - [Step 1: Open Media](#step-1-open-media)
   - [Step 2: Define the Scope](#step-2-define-the-scope)
   - [Step 3: Edit or Analyze](#step-3-edit-or-analyze)
   - [Step 4: Review Changes](#step-4-review-changes)
   - [Step 5: Write Tags](#step-5-write-tags)
6. [Edit Modes](#edit-modes)
   - [Sources and Checked Files](#sources-and-checked-files)
   - [Batch Mode](#batch-mode)
   - [Per-File Mode](#per-file-mode)
   - [Columns and Persistent Libraries](#columns-and-persistent-libraries)
7. [Change Preview and Safety](#change-preview-and-safety)
   - [Staging and Preview](#staging-and-preview)
   - [Write Tags](#write-tags)
   - [Remove All Tags](#remove-all-tags)
   - [Process Log](#process-log)
8. [Auto-Tag Feature](#auto-tag-feature)
   - [Per-File Identification](#per-file-identification)
   - [Batch Release Matching](#batch-release-matching)
   - [Providers](#providers)
9. [Text Tools](#text-tools)
   - [Find and Replace](#find-and-replace)
   - [Case and Whitespace](#case-and-whitespace)
10. [File Pattern Tool](#file-pattern-tool)
   - [Tags from Filename](#tags-from-filename)
   - [Filename from Tags](#filename-from-tags)
   - [Filename from Filename](#filename-from-filename)
11. [Metadata Import and Export](#metadata-import-and-export)
   - [Import](#import)
   - [Export](#export)
12. [Rule Studio](#rule-studio)
13. [Clean & Organize](#clean--organize)
14. [Library Integrity](#library-integrity)
15. [Advanced Media Tools](#advanced-media-tools)
   - [Artwork Collection Manager](#artwork-collection-manager)
   - [Custom and Format-Specific Fields](#custom-and-format-specific-fields)
   - [Chapter Editor and Video Details](#chapter-editor-and-video-details)
   - [Lyrics Lookup](#lyrics-lookup)
   - [Loudness and ReplayGain](#loudness-and-replaygain)
16. [Action Buttons](#action-buttons)
17. [Undo and Redo](#undo-and-redo)
18. [Field Storage System](#field-storage-system)
19. [Studio Automation](#studio-automation)
20. [Settings](#settings)
21. [Cloud Settings Sync](#cloud-settings-sync)
22. [Keyboard Shortcuts](#keyboard-shortcuts)
23. [Sidebar](#sidebar)
24. [Context Menus](#context-menus)
25. [Current Boundaries](#current-boundaries)
26. [Troubleshooting](#troubleshooting)
   - [A Command Is Disabled](#a-command-is-disabled)
   - [Search Lyrics Is Disabled](#search-lyrics-is-disabled)
   - [Auto Tag Found No Confident Match](#auto-tag-found-no-confident-match)
   - [Artwork or Chapters Cannot Be Written](#artwork-or-chapters-cannot-be-written)
   - [A Write Failed](#a-write-failed)
27. [Updating Software](#updating-software)
28. [Copyright](#copyright)
29. [Screenshots](#screenshots)

## **System Requirements**

### **Minimum Requirements**

- **Operating System:** Windows 10 version 1809 or later, 64-bit
- **Processor:** Dual-core x64 processor at 1.5 GHz
- **RAM:** 4 GB
- **Display:** 1280 × 720 recommended; minimum window size 800 × 600 device-independent pixels
- **Storage:** 500 MB plus temporary space for recovery snapshots and reports
- **Software:** No separate .NET installation is required by the self-contained package

### **Recommended Requirements**

- **Operating System:** Windows 10/11 version 21H2 or later, 64-bit
- **Processor:** Quad-core x64 processor at 2.0 GHz or higher
- **RAM:** 8 GB or higher; 16 GB for very large libraries
- **Display:** 1920 × 1080 or higher
- **Storage:** SSD with free space for the largest planned batch and recovery data

MetaEdit Plus is a native Windows WPF application. Linux, macOS, Wine, and Bottles are not supported release targets.

## **Third-Party Libraries**

| Component | Version | Used For | License |
|---|---:|---|---|
| [TagLib#](https://github.com/mono/taglib-sharp) | 2.3.0 | Common audio/video metadata, properties, and artwork | LGPL 2.1 |
| [ATL](https://github.com/Zeugma440/atldotnet) | 7.16.0 | Additional metadata adapters, including OptimFROG, Speex, TAK, and TTA | LGPL 3.0 |
| [NAudio](https://github.com/naudio/NAudio) | 2.3.0 | Audio decoding and playback | MIT |
| [NAudio.Vorbis](https://github.com/naudio/Vorbis) | 1.6.0 | Ogg/Vorbis decoding | MIT |
| [Microsoft.Data.Sqlite](https://learn.microsoft.com/dotnet/standard/data/sqlite/) | 10.0.11 | Private local persistent-library indexes | MIT |
| [Chromaprint](https://acoustid.org/chromaprint) | bundled `fpcalc` | Acoustic fingerprints for AcoustID lookup | MIT/LGPL |

Optional external installations retain their own licenses:

- **FFmpeg/ffprobe** extends decoding, stream inspection, and MP4-family chapter replacement.
- **MKVToolNix** enables embedded chapter replacement for Matroska and WebM.

When an optional tool is unavailable, MetaEdit keeps the dependent command disabled and explains the prerequisite. Ordinary tag editing remains available.

## **Installation**

1. Open the [Releases](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/releases) page.
2. Download the Windows x64 installer published for the selected release.
3. Run the installer and review the destination and optional components.
4. Launch **MetaEdit Plus** from the Start Menu or Desktop shortcut.

## **Authentication, Cloud Sync, and Privacy**

MetaEdit is fully usable without signing in. Settings, layouts, field sets, mappings, rules, persistent indexes, recovery jobs, and workspace state are stored in the current Windows user's local application-data area.

[Arctisoft Studio Hub](https://github.com/BerndHagen/Arctisoft-Studio-Hub) sign-in is optional. In v2.0.0:

- cloud sync is **off by default**;
- enabling it requires a signed-in Studio account and explicit confirmation;
- only portable tag preferences, artwork policy, and Auto Tag source order are synchronized;
- media, artwork bytes, file paths, credentials, indexes, recovery data, field sets, layouts, mappings, and Rule Studio presets remain local;
- disabling sync cancels pending preference uploads and leaves the local copy usable;
- MetaEdit does not award XP or convert editing activity into engagement rewards.

The application contacts online services only when a requested feature needs them, such as Auto Tag, Lyrics Lookup, optional cloud sync, account session maintenance, or support links. Provider queries can include metadata, fingerprints, or identifiers required by that provider.

## **Getting Started Guide**

### **Step 1: Open Media**

Choose **Open Media Files**, **Open Media Folder**, or **Open Playlist**. Folder discovery is recursive. Loading a new source rebuilds the checked scope without allowing stale workflow results to target the new library.

### **Step 2: Define the Scope**

Use the Library checkboxes to include or exclude files. The header checkbox is available only when real rows exist. Select **Batch Mode** for deliberate shared edits or **Per-File Mode** for independent values.

### **Step 3: Edit or Analyze**

Enter values directly, manage artwork, or open Auto Tag, Text Tools, Library Health, Lyrics, ReplayGain, or another workflow. Analysis commands do not write media.

### **Step 4: Review Changes**

Open **Preview Staged Changes** and inspect the exact file, field, current value, and proposed value. Search and change-kind filters affect only the review.

### **Step 5: Write Tags**

Choose **Write Tags** when the review is correct. Keep the application open until the Process Log reports completion or a per-file failure.

## **Edit Modes**

### **Sources and Checked Files**

MetaEdit accepts files, recursive folders, and local M3U/M3U8 playlists. Duplicate paths are normalized before the Library is built. Source replacement preserves committed recovery history while clearing only confirmed staged state.

A checked row is eligible for scope-based work. Clearing a row excludes it without changing the file. Library search supports filenames and metadata expressions with Boolean operators, presence checks, comparisons, and guarded regular expressions.

### **Batch Mode**

Batch Mode applies only fields the user deliberately changes to checked files. Mixed source values are represented separately so an untouched blank does not become a batch clear.

### **Per-File Mode**

Per-File Mode maintains a separate staged state for each file. Previous and Next commands update both the selected editor target and the highlighted Library row.

### **Columns and Persistent Libraries**

Named Library layouts control visible columns, widths, order, sorting, and expression columns. Persistent Libraries register selected folders in a private local SQLite index. Rescan reads changed entries; removing a registration never removes media files.

## **Change Preview and Safety**

### **Staging and Preview**

Editor values, artwork, provider choices, lyrics, ReplayGain measurements, rules, and imports are proposals until they enter the shared change set. Closing an analysis workspace does not write tags.

### **Write Tags**

Write Tags validates scope and file eligibility before mutation. Failures are reported per file. Writes preserve untouched standard fields, extended text values, and complete artwork collections where supported.

### **Remove All Tags**

Remove All Tags is a reviewed destructive operation with the same preflight and recovery boundary. It remains disabled until an eligible checked scope exists.

Undo is a recovery feature, not a substitute for independent backups of valuable media.

### **Process Log**

The Process Log is an operational record, not a second status dashboard. Its default columns show the event sequence, time, severity, task, and complete message. **Choose Columns** can add scope or progress, file or target, and the raw event when deeper diagnosis is needed. Filters and column choices change only the view; **Clear Process Log** removes retained events and becomes unavailable when the log is empty.

## **Auto-Tag Feature**

Auto Tag uses one review model in both editing modes. Identification does not stage or write by itself.

### **Per-File Identification**

Per-File Mode fingerprints selected audio, queries enabled sources, and shows confidence, provenance, conflicts, metadata choices, and artwork choices.

### **Batch Release Matching**

Batch Mode identifies one release for the checked album scope, loads a selected MusicBrainz edition, maps files one-to-one to tracks, and allows manual reassignment. A mixed folder is not automatically split into release jobs.

### **Providers**

| Provider | Role |
|---|---|
| **AcoustID** | Acoustic-fingerprint lookup evidence |
| **MusicBrainz** | Recording, release, edition, identity, and track mapping data |
| **Discogs** | Optional catalog evidence using a personal token stored in Windows Credential Manager |
| **iTunes** | Supplemental catalog and artwork evidence |

Provider requests are bounded and cancellable. Online catalogs, ambiguity, and service limits can prevent a confident result. **Stage Results** transfers reviewed choices into the editor; **Write Tags** remains separate.

## **Text Tools**

### **Find and Replace**

Transform selected fields with literal or bounded regular-expression replacement, whole-word matching, and optional prefixes or suffixes. **Build Preview** evaluates the checked scope before staging; the result table shows the original value, proposed value, and any validation issue for each file.

### **Case and Whitespace**

Apply case conversion or Unicode whitespace normalization to selected fields. Review the changed rows, then choose **Stage Metadata** to move only the reviewed proposals into the normal Change Review. This does not write media until **Write Tags** is used.

## **File Pattern Tool**

### **Tags from Filename**

Capture structured filename parts into metadata fields with a named pattern. Parsed values remain proposals until reviewed and staged.

### **Filename from Tags**

Build filenames with a bounded format expression. MetaEdit sanitizes invalid path characters and rejects duplicate destinations before a transactional rename.

### **Filename from Filename**

Capture and rearrange up to nine existing filename parts. Swaps, chains, and case-only renames use the same collision-checked rollback plan.

The shared expression engine supports standard fields, safe file pseudo-fields, optional sections, nested string operations, comparisons, arithmetic, Boolean logic, metadata value/count helpers, and bounded regular expressions.

## **Metadata Import and Export**

### **Import**

- reviewed CSV import using the standard transfer schema;
- reviewed line-pattern text import;
- sequential or explicit filename/path matching;
- exact matched, skipped, empty, and preserved-value reporting;
- staging through Change Review and Write Tags.

### **Export**

- CSV and structured JSON;
- escaped HTML and tab-separated text;
- relative M3U8, compatible M3U, and grouped M3U8 playlists;
- formatted text through **Copy as Text**, with optional grouping and live expression preview.

Reports are written atomically. CSV output preserves literal apostrophes while protecting spreadsheet consumers from formula interpretation.

## **Rule Studio**

Rule Studio combines **All** or **Any** conditions with ordered actions across the checked scope. It supports text, numeric, presence, and pattern checks, then set, copy, clear, transform, format, and sequence actions.

Dry Preview shows matches, proposed changes, and failures. Applying a rule stages metadata. Sequence counters can reset by folder or metadata field and advance only for matching files. Rule presets are local and exchangeable as JSON.

## **Clean & Organize**

Clean & Organize builds a resumable plan for checked media. It can inspect evidence, normalize metadata, propose destination folders, and create rename or move work.

Analysis, conflict review, destination review, and commit are separate steps. Conflicts require a decision. Commit creates transaction backups and rolls back completed steps if a later operation fails.

## **Library Integrity**

Library Health analyzes files without changing them. Findings cover readability, required fields, album consistency, track/disc numbering and gaps, artwork consistency, moved files, exact byte duplicates, and metadata-and-duration candidates.

Excluding a finding changes only the review scope. It never deletes or quarantines media. Findings and exclusions can be exported.

## **Advanced Media Tools**

### **Artwork Collection Manager**

The editor displays the selected picture type and offers quick replacement or removal. **Manage Collection** opens every embedded picture in stored order.

Users can add or replace bytes, set type and description, reorder or remove images, and inspect dimensions, encoded size, format, aspect ratio, color depth, resolution, pixel format, color profile, alpha, frame count, pixel count, and orientation.

Artwork remains staged until Write Tags. Copy/Paste Metadata transfers the complete collection. Format support is container-dependent.

### **Custom and Format-Specific Fields**

Custom Fields works across the checked scope and distinguishes common, mixed, and missing values. Inline edits stage changes; explicit deletion prevents an empty cell from becoming an accidental write.

Format-Specific Tags edits supported native text entries for one selected file:

- ID3v2 user-text fields;
- Xiph/Vorbis comment keys;
- APEv2 text items;
- MP4 `com.apple.iTunes` freeform fields;
- ASF text descriptors;
- supported Matroska simple tags.

The final row creates another entry as needed. Empty cells display a visual dash that is never written. Unsupported binary or structured values remain preserved.

### **Chapter Editor and Video Details**

Chapter Editor validates start/end order, duration, identifiers, URLs, and overlap conditions for one selected file. Sidecar import and export remain available.

- **Matroska/WebM:** embedded replacement uses MKVToolNix when available.
- **MP4/M4V/MOV:** embedded replacement uses FFmpeg stream-copy handling when available.

Video Details exposes contextual TV/movie fields and stream properties without duplicating common editor fields. Complete nested Matroska editions and generalized subsong authoring are outside the current scope.

### **Lyrics Lookup**

Lyrics Lookup requires a selected audio file and track title. Artist and album improve ranking but are optional. It searches LRCLIB, ranks candidates using metadata and duration, distinguishes plain and synchronized lyrics, and previews from the start.

A candidate can be staged or exported as UTF-8 TXT/LRC. Changing tracks clears stale results, and late network responses cannot overwrite the new selection.

### **Loudness and ReplayGain**

Loudness & ReplayGain decodes checked audio, calculates gated integrated loudness, and derives ReplayGain 2 values referenced to -18 LUFS. It reports track gain/peak/range and album evidence.

Applying results stages tags only. MetaEdit does not normalize or re-encode audio. This is not a certified broadcast delivery validator and does not author ADM metadata.

## **Action Buttons**

The bottom action bar follows the open page. Start with the page's source or analysis command, inspect the results, then stage or commit only when that action becomes available. Hover a disabled action to see what is missing. Result filters change the view, not the media.

- **Editor:** use **Preview Changes** to inspect the staged file/value pairs, then **Write Tags** to commit them. **Reset Changes** discards the current staged proposal.
- **Auto Tag:** use **Identify File** or **Identify Release** to gather evidence, review the match and artwork choices, then **Stage Results** to transfer selected values into editor staging.
- **Text Tools and Rule Studio:** build a preview, inspect changed rows and errors, then stage the reviewed metadata. Rename plans use their own collision-checked commit path.
- **Clean & Organize:** analyze the plan, review conflicts and destinations, then commit the ready plan. Export Plan records the review without moving files.
- **Library Health:** scan, switch among all, required, album and duplicate findings, or export the evidence. Exclusions affect the review scope only.
- **Transfer Tags:** review an import source before staging it, or choose an export format and write a report. Export never modifies media tags.
- **ReplayGain and Lyrics:** analyze or search first, then stage the chosen gain values or lyrics. **Write Tags** in the editor remains the final commit step.

## **Undo and Redo**

Supported write operations capture metadata, extended text fields, and the complete ordered artwork collection before mutation. Up to 20 history levels are retained. A new divergent operation clears redo history, and a failed recovery snapshot prevents a write from starting. Undo supports recovery from an unintended edit, but important media should also have an independent backup.

## **Field Storage System**

- **Editor Layouts:** show, hide, and reorder fields within five standard sections.
- **Library Layouts:** control columns, widths, order, sorting, and expression columns with bounded widths.
- **Field Sets:** save reusable non-empty values and complete artwork collections; restore previews before staging.
- **Container Mappings:** map fields to validated native ID3v2, Xiph, APEv2, MP4, ASF, and Matroska keys.
- **Text Export Templates:** save Copy as Text expressions and grouping rules.
- **Profile Backup:** export a versioned, bounded ZIP with supported preferences and reusable definitions.

Profile restore is validated and transactional. Credentials, account sessions, shared tools, private indexes, media, and incomplete operations are excluded.

## **Studio Automation**

`MetaEdit.Automation.exe` ships beside the desktop application for guarded studio-library jobs. New jobs are review-only: a write requires both `AllowCommit: true` in the reviewed job and an explicit `--commit` argument.

```powershell
MetaEdit.Automation.exe init job.json C:\Incoming C:\Delivered C:\Reports studio-library-flac-v1
MetaEdit.Automation.exe dry-run job.json
MetaEdit.Automation.exe run job.json --commit
MetaEdit.Automation.exe watch job.json [--commit]
MetaEdit.Automation.exe diagnostics support-bundle.zip
```

Jobs are bounded to 1–500 files per transaction. Dry runs validate metadata and destinations and record source hashes without changing media. Commit mode rechecks identity, creates backups, validates output, and records source/output SHA-256 evidence. Watch mode ignores reparse points, system files, unstable files, and unchanged blocked inputs.

The first delivery profiles cover FLAC/Vorbis Comments and MP3/ID3 studio libraries. They do not claim broadcaster, archive, or streaming certification. Diagnostics are redacted and exclude settings values, credentials, metadata, media, and media paths.

## **Settings**

Settings control:

- ID3v2.3 or ID3v2.4 policy and compatible text encoding;
- ID3v1, ID3v2, and APE retention for MP3;
- artwork maximum edge, JPEG quality, PNG handling, and default type;
- enabled Auto Tag sources and priority;
- optional Discogs credentials in Windows Credential Manager;
- optional Studio Hub preference sync and software update channel;
- local persistent-library and profile behavior.

Settings are validated and written atomically. At least one MP3 tag container and one valid Auto Tag source must remain enabled.

## **Cloud Settings Sync**

Cloud preference sync is **off by default**. The **Application Services** settings section offers **This device only** and **Sync with Studio Hub**. Sync requires a signed-in Studio account and explicit confirmation. Only portable tag preferences, artwork policy, and Auto Tag source order are synchronized. Media, artwork bytes, paths, credentials, indexes, recovery data, field sets, layouts, mappings, and Rule Studio presets remain on this device. Turning sync off cancels pending preference uploads and leaves the local copy usable.

## **Keyboard Shortcuts**

Press **Ctrl+Shift+P** or **F1** to open Command Center. It searches the complete command catalog, remembers recent commands, and explains unavailable commands.

| Shortcut | Command |
|---|---|
| `Ctrl+Shift+P` or `F1` | Command Center |
| `Ctrl+N` | Start New Session |
| `Ctrl+O` | Open Media Files |
| `Ctrl+Shift+O` | Open Media Folder |
| `F5` | Refresh Loaded Source |
| `Ctrl+F` | Focus Library Search |
| `Ctrl+S` | Write Tags |
| `Ctrl+Shift+S` | Save Field Set |
| `Ctrl+Z` | Undo |
| `Ctrl+Y` or `Ctrl+Shift+Z` | Redo |
| `Ctrl+Alt+A` | Auto Tag |
| `Ctrl+Shift+T` | Text Tools |
| `Ctrl+,` | Settings |
| `Alt+F4` | Exit |

Menus expose the same source, edit, metadata, workflow, view, and help commands. Text fields use MetaEdit's custom Cut/Copy/Paste context menu with standard repeated right-click placement.

## **Sidebar**

The left sidebar opens the editor and workflow pages. The Library beside it shows the current files, checked scope, search, and selected file. Selecting a new source refreshes the open workflow when its data is ready; it does not stage or write changes. The right inspector summarizes the current page and selected result.

## **Context Menus**

Right-click a text field for MetaEdit's Cut, Copy, Paste, and Select All menu. Right-click a Library row, table, or artwork preview for commands relevant to that target. Menu entries are enabled only when the current selection supports them. The Command Center and menu bar provide keyboard and pointer access to the same application commands.

## **Current Boundaries**

MetaEdit v2.0.0 does not claim:

- a public plugin SDK or signed third-party extension model;
- optical-disc TOC lookup;
- complete BWF `bext`, iXML, ADM, PBCore, or EBUCore authoring and conformance;
- complete nested Matroska edition or generalized subsong editing;
- certified broadcast loudness-delivery reports;
- multi-user project locking, approval, or facility audit trails;
- Linux or macOS support.

Online provider availability, catalog completeness, and rate limits remain outside MetaEdit's control.

## **Troubleshooting**

### **A Command Is Disabled**

Hover it. MetaEdit reports the prerequisite, such as loading files, checking a scope, selecting a file, completing analysis, choosing a destination, or installing an optional tool.

### **Search Lyrics Is Disabled**

Select an audio file and provide a track title. Artist and album are optional. Search remains disabled during an active request or source change.

### **Auto Tag Found No Confident Match**

Verify decodable audio, internet access, and enabled providers, then try a more precise query. The release may not exist in the selected catalog.

### **Artwork or Chapters Cannot Be Written**

The container may not support the structure, or FFmpeg/MKVToolNix may be unavailable. MetaEdit explains blocked writes and offers sidecars where applicable.

### **A Write Failed**

Read the Process Log and keep the application open while reviewing recovery information. Preserve original media and include a redacted log when reporting the issue.

## **Updating Software**

MetaEdit can check for updates independently of Arctisoft Studio Hub. In **Settings → Application Services**, choose **Stable releases**, **Preview releases**, or **Manual checks only**. Use **Help → Check for Updates** to check at any time. A newer version appears in the main window; MetaEdit verifies the download and publisher signature before starting the installer. The optional Hub can also manage installed Arctisoft applications centrally.

You can always install a newer version manually from the official [Releases](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/releases) page. Keep a profile backup and an independent media backup before major upgrades.

## **Copyright**

MetaEdit Plus is proprietary freeware and is protected by international copyright laws.

1. **License:** You are granted a non-exclusive, non-transferable license to use MetaEdit Plus for personal and commercial purposes.

2. **Original Installer Distribution:** The original, unmodified installer may be shared. Modified installers, repackaged builds, sale, rental, and sublicensing require prior written permission.

3. **Modifications Prohibited:** Modification, decompiling, reverse engineering, disassembly, or derivative work is prohibited without prior written consent.

4. **Third-Party Components:** MetaEdit uses the libraries and optional tools listed in [Third-Party Libraries](#third-party-libraries). Their respective licenses continue to apply.

5. **Warranty Disclaimer:** MetaEdit Plus is provided *"as is,"* without warranties of any kind. The author assumes no liability for damages resulting from use.

6. **Limitation of Liability:** The author is not responsible for indirect, special, incidental, or consequential damages arising from use.

7. **Termination:** The license may be terminated if these terms are violated. Upon termination, all use must cease and copies must be deleted.

The application is fully usable without signing in. Arctisoft Studio Hub is an optional account and application manager. By using MetaEdit Plus, you agree to the terms in the [LICENSE](LICENSE).

Report defects through [GitHub Issues](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/issues). Questions and workflow discussions belong in [Discussions](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/discussions).

## **Screenshots**

The screenshots show the application using generated audio fixtures and fictional metadata. No commercial audio is included. Click an image to view it at full size.

<table>
  <tr>
    <th align="left">MetaEdit Plus - Metadata Editor</th>
    <th align="left">MetaEdit Plus - Auto Tag</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-01-editor.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-01-editor.png" alt="MetaEdit Plus Metadata Editor" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-02-auto-tag.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-02-auto-tag.png" alt="MetaEdit Plus Auto Tag" width="450"></a></td>
  </tr>
  <tr>
    <th align="left">MetaEdit Plus - Text Tools</th>
    <th align="left">MetaEdit Plus - Clean & Organize</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-03-text-tools.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-03-text-tools.png" alt="MetaEdit Plus Text Tools" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-04-clean-organize.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-04-clean-organize.png" alt="MetaEdit Plus Clean & Organize" width="450"></a></td>
  </tr>
  <tr>
    <th align="left">MetaEdit Plus - Library Health</th>
    <th align="left">MetaEdit Plus - Lyrics Lookup</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-05-library-health.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-05-library-health.png" alt="MetaEdit Plus Library Health" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-06-lyrics.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-06-lyrics.png" alt="MetaEdit Plus Lyrics Lookup" width="450"></a></td>
  </tr>
  <tr>
    <th align="left">MetaEdit Plus - Transfer Tags</th>
    <th align="left">MetaEdit Plus - ReplayGain Analysis</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-07-transfer-tags.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-07-transfer-tags.png" alt="MetaEdit Plus Transfer Tags" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-08-replaygain.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-08-replaygain.png" alt="MetaEdit Plus ReplayGain Analysis" width="450"></a></td>
  </tr>
  <tr>
    <th align="left">MetaEdit Plus - Change Review</th>
    <th align="left">MetaEdit Plus - Command Center</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-09-change-review.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-09-change-review.png" alt="MetaEdit Plus Change Review" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-10-command-center.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/showcase-10-command-center.png" alt="MetaEdit Plus Command Center" width="450"></a></td>
  </tr>
</table>
