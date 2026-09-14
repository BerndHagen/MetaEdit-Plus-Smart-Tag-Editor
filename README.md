<p align="center">
  <img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/metaedit-logo.png" alt="MetaEdit Plus Logo" width="128" />
</p>
<h1 align="center">MetaEdit Plus - Audio &amp; Video Metadata Editor</h1>
<p align="center">
  <b>Edit, identify, review, and organize metadata across complete media libraries.</b><br>
  <b>Work in batches or per file, reconcile online metadata, manage artwork, and preview every change.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Freeware-green?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet/10.0/runtime"><img src="https://img.shields.io/badge/.NET-10.0-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/issues"><img src="https://img.shields.io/github/issues/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor?style=flat-square&color=orange" alt="Open Issues"></a>
</p>

**MetaEdit Plus** is a Windows metadata editor for audio and video files. It can load individual files or recursively discover supported media in folders, then work on the checked selection in Batch Mode or keep independent staged values in Per-File Mode. Its four metadata workspaces expose 38 editable fields, from core tags and credits to release identifiers and sort fields.

The application combines direct tag editing with fingerprint-based identification, release-aware matching, configurable source reconciliation, complete artwork collections, ReplayGain analysis, lyrics lookup, video/chapter tools, format-specific tags, change previews, metadata interchange, reusable rules, library cleanup, and integrity analysis. Potential changes remain reviewable before they are written, while undo/redo snapshots, transaction protection, and quarantine manifests provide recovery paths for destructive-looking workflows.

### **Key Features**

- **Checked-File Processing:** Load files or folders recursively, filter by media format, and control scope with the file checklist.
- **Batch and Per-File Editing:** Share staged values across a selection or maintain a separate edit state for each file.
- **38 Metadata Fields:** Edit core metadata, credits and notes, release and rights data, MusicBrainz identifiers, and sort fields.
- **Review Before Write:** Inspect staged field-level changes before committing them to media files.
- **Auto Tag:** Identify audio with Chromaprint/AcoustID and reconcile configurable MusicBrainz and iTunes evidence, including confidence and conflict feedback.
- **Release Matching:** Select an exact MusicBrainz edition and map checked files one-to-one to its tracklist before staging batch metadata.
- **Artwork Choices:** Compare embedded or online cover choices, see meaningful release context, and select the artwork to stage.
- **Artwork Collections:** Add, replace, remove, reorder, inspect, copy, and paste multiple embedded images without flattening picture types or descriptions.
- **Format-Specific Tags:** Select an applied field, then edit ID3 user text, Xiph comments, APE text, MP4 freeform fields, or ASF text descriptors with real multi-value support.
- **Loudness & ReplayGain:** Measure gated BS.1770/EBU R128 loudness and write non-destructive ReplayGain 2 track/album tags.
- **Lyrics Lookup:** Rank LRCLIB candidates by identity and duration, preview plain or synchronized lyrics, stage a choice, or export a sidecar.
- **Video Details:** Edit video-specific TV/movie tags, inspect streams, and manage chapter markers with sidecar and container-aware workflows.
- **Text Tools:** Find and replace exact text, convert case across selected fields, and review every proposed value.
- **File Patterns:** Extract tags from filenames or generate sanitized filenames from metadata placeholders.
- **Metadata Interchange:** Import CSV and export reviewed selections as CSV, structured JSON, or portable M3U8 playlists.
- **Rule Studio:** Build reusable all/any condition sets and ordered actions, enable or reorder individual steps, exchange JSON presets, preview matches, and stage the result.
- **Clean & Organize:** Run a resumable identification and normalization pipeline with progress, estimates, review, backup, and rollback protection.
- **Library Integrity:** Detect exact duplicates, matching decoded audio, and related releases with cached background analysis and recoverable quarantine.
- **Undo and Redo:** Restore complete metadata and artwork snapshots for up to 20 operations.
- **Field Sets:** Save up to 50 field and artwork configurations for reuse during the current session.
- **Media Inspection:** Open track and artwork information, play an audio preview, search the file list, and monitor system performance.
- **Responsive Desktop UI:** Tool windows adapt to available space while retaining keyboard navigation and accessible interaction feedback.
- **Optional Studio Hub Sync:** Share supported preferences through [Arctisoft Studio Hub](https://github.com/BerndHagen/Arctisoft-Studio-Hub) when a Hub session is available.

### **Supported Formats**

MetaEdit Plus supports a wide range of audio and video formats:

- **Audio Formats:** `MP3`, `WAV`, `FLAC`, `OGG`, `WMA`, `M4A`, `AIFF`
- **Video Formats:** `MP4`, `MKV`, `MOV`, `WMV`, `M4V`, `WEBM`

> **Note:** Raw AAC is not part of the selectable format list. For AAC audio, use the supported M4A container.

> **Format Limitations:** Some formats have limited metadata support. WAV has limited tag support and thumbnail embedding may not work. AIFF supports basic metadata only. WebM has limited tag field support. MOV metadata support varies depending on how the file was created.

> **Chapter Tools:** Sidecar import/export is built in. Embedded Matroska/WebM chapter updates require an installed MKVToolNix; embedded MP4/M4V/MOV chapter updates require FFmpeg/ffprobe. MetaEdit detects these tools and disables unsupported write actions with an explanation.

### **Available Metadata Fields**

MetaEdit Plus provides 38 metadata fields organized into four workspaces:

- **Core Metadata:** Title, Subtitle, Performer, Genre, BPM, Initial Key, Album, Album Artist, Track Number, Track Count, Disc Number, Disc Count
- **Credits & Notes:** Composer, Conductor, Performer Role, Remixed By, Grouping, Description, Lyrics
- **Release & Rights:** Year, Release Status, Release Type, Release Country, Publisher, Copyright, ISRC, Amazon ID
- **IDs & Sorting:** MusicBrainz Track, Release, Release Group, Artist, Release Artist, and Disc IDs; Title, Album, Performer, Album Artist, and Composer sort values

Artwork is managed alongside the fields and can be inspected separately through Artwork Information or the complete collection manager. Container-specific fields that do not belong in the standard 38-field workspace remain available through Format-Specific Tags and Video Details. Whether every field can be represented depends on the tag capabilities of the selected media format.

## **Table of Contents**

1. [System Requirements](#system-requirements)
   - [Minimum Requirements](#minimum-requirements)
   - [Recommended Requirements](#recommended-requirements)
2. [Third-Party Libraries](#third-party-libraries)
   - [TagLib#](#taglib)
   - [Chromaprint and fpcalc](#chromaprint-and-fpcalc)
   - [NAudio and LRCLIB](#naudio-and-lrclib)
3. [Installation](#installation)
4. [Getting Started Guide](#getting-started-guide)
   - [Step 1: Select Library Type](#step-1-select-library-type)
   - [Step 2: Choose Format and Select Files](#step-2-choose-format-and-select-files)
   - [Step 3: Edit Metadata Fields](#step-3-edit-metadata-fields)
   - [Step 4: Apply Changes](#step-4-apply-changes)
5. [Edit Modes](#edit-modes)
   - [Batch Mode (Default)](#batch-mode-default)
   - [Per-File Mode](#per-file-mode)
6. [Change Preview and Safety](#change-preview-and-safety)
7. [Auto-Tag Feature](#auto-tag-feature)
   - [Supported Databases](#supported-databases)
   - [How It Works](#how-it-works)
   - [Metadata Choices](#metadata-choices)
   - [Artwork Choices](#artwork-choices)
   - [Batch Release Matching](#batch-release-matching)
8. [Text Tools](#text-tools)
   - [Find & Replace](#find--replace)
   - [Case Conversion](#case-conversion)
   - [File Pattern (within Text Tools)](#file-pattern-within-text-tools)
9. [File Pattern Tool](#file-pattern-tool)
   - [Tag from Filename](#tag-from-filename)
   - [Filename from Tags](#filename-from-tags)
10. [Metadata Import and Export](#metadata-import-and-export)
   - [Export](#export)
   - [Import](#import)
11. [Rule Studio](#rule-studio)
12. [Clean & Organize](#clean--organize)
13. [Library Integrity](#library-integrity)
14. [Advanced Media Tools](#advanced-media-tools)
    - [Artwork Collection Manager](#artwork-collection-manager)
    - [Format-Specific Tags](#format-specific-tags)
    - [Loudness and ReplayGain](#loudness-and-replaygain)
    - [Lyrics Lookup](#lyrics-lookup)
    - [Video Details](#video-details)
15. [Action Buttons](#action-buttons)
16. [Undo and Redo](#undo-and-redo)
    - [How It Works](#how-it-works-1)
    - [What Gets Restored](#what-gets-restored)
    - [Console Feedback](#console-feedback)
17. [Field Storage System](#field-storage-system)
18. [Settings](#settings)
    - [ID3v2 Version](#id3v2-version)
    - [Text Encoding](#text-encoding)
    - [Cover Image Settings](#cover-image-settings)
    - [Tag Retention](#tag-retention)
    - [Auto-Tag Settings](#auto-tag-settings)
19. [Cloud Settings Sync](#cloud-settings-sync)
    - [How It Works](#how-it-works-2)
    - [Synced Settings](#synced-settings)
20. [Keyboard Shortcuts](#keyboard-shortcuts)
21. [Sidebar](#sidebar)
22. [Context Menus](#context-menus)
    - [Text Fields](#text-fields)
    - [Console Output](#console-output)
    - [Thumbnail Panel](#thumbnail-panel)
    - [Path Bar](#path-bar)
    - [File List (Per-File Mode only)](#file-list-per-file-mode-only)
23. [Copyright](#copyright)
24. [Screenshots](#screenshots)

## **System Requirements**

### **Minimum Requirements**
- **Operating System:** Windows 10 or Windows 11, 64-bit
- **Storage:** Enough space for the installed application, temporary working data, and any backups or quarantine copies created by library workflows
- **Software:** No separate .NET installation is required by the self-contained release

### **Recommended Requirements**
- **Operating System:** A currently supported 64-bit version of Windows 10 or Windows 11
- **Storage:** An SSD and sufficient free space for large-library backup or quarantine operations
- **Network:** Internet access when using Auto Tag or optional Studio Hub synchronization
- **Optional Tools:** MKVToolNix for no-remux Matroska chapters; FFmpeg/ffprobe for MP4-family chapter inspection and stream-copy replacement

**Note:** MetaEdit Plus is a Windows desktop application built with WPF on .NET 10. The distributed application is self-contained; Linux and macOS builds are not provided.

## **Third-Party Libraries**

MetaEdit Plus uses the following third-party libraries:

### TagLib#

**TagLib#** is a .NET library for reading and writing metadata in media files. It provides support for various audio and video formats and handles tag formats such as ID3v1, ID3v2, APE, Xiph Comments, and more. MetaEdit Plus uses TagLib# for all metadata operations.

- **Website:** [TagLib# GitHub Repository](https://github.com/mono/taglib-sharp)
- **Version used by MetaEdit Plus 2.0:** 2.3.0

For more details about TagLib# including its capabilities and supported formats, check the official documentation:

- **TagLib# Documentation:** [TagLib# API Documentation](https://github.com/mono/taglib-sharp#readme)

### Chromaprint and fpcalc

**fpcalc**, the command-line fingerprint utility from the Chromaprint project, is bundled for acoustic identification. Auto Tag uses its fingerprint output when querying AcoustID; it does not identify tracks by filename alone.

- **Website:** [AcoustID / Chromaprint](https://acoustid.org/chromaprint)

The application also uses the .NET `System.Management` package for Windows performance information. Online metadata is obtained through service APIs.

### NAudio and LRCLIB

**NAudio 2.3.0** and **NAudio.Vorbis.Latest 1.6.0** provide floating-point sample decoding for the ReplayGain analysis workflow. MetaEdit measures the decoded signal and writes gain metadata; it does not alter or re-encode the audio stream.

**LRCLIB** supplies plain and synchronized lyrics candidates through its public API. Results are reviewed before a selected value is staged, and the lookup can also export `.txt` or `.lrc` sidecars.

- **NAudio:** [GitHub repository](https://github.com/naudio/NAudio)
- **LRCLIB:** [API documentation](https://lrclib.net/docs)

For chapter editing, MetaEdit detects existing installations of **MKVToolNix** and **FFmpeg/ffprobe**. These tools are optional: chapter sidecar import/export still works without them. MKVToolNix enables no-remux Matroska chapter updates; FFmpeg enables stream-copy chapter updates for MP4-family containers.

If you have questions or issues related to these libraries, please [open an issue](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/issues) on GitHub.

## **Installation**

1. Download the latest release from the [Releases](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/releases) page.
2. Run the installer and follow the setup wizard.
3. Launch MetaEdit Plus from the Start Menu or Desktop shortcut.

## **Getting Started Guide**

### **Step 1: Select Library Type**

When you open MetaEdit Plus, select **Audio Library** or **Video Library**. The adjacent format selector can show every supported format in that library or narrow discovery to one extension.

### **Step 2: Choose Format and Select Files**

1. Select a library and either an all-formats option or a specific format.
2. Click **Add Folder** or press `Ctrl+B` to choose a folder. Folder discovery includes supported files in subfolders.
3. Alternatively, drop supported files or a folder onto the application. The detected media type updates the library and format controls.
4. Review the discovered list and uncheck anything that must remain outside the current operation. Ctrl-click selects multiple rows; press `Space` to include or exclude the selected group together.

The active source can be either one folder tree or an explicit set of files. Selecting a different source clears the existing source after MetaEdit Plus gives you a chance to keep any unwritten staged changes.

### **Step 3: Edit Metadata Fields**

Navigate through the four workspaces to fill in the required fields:

- **Core Metadata** for the identity and sequence of a track
- **Credits & Notes** for contributors and descriptive text
- **Release & Rights** for release state, territory, publisher, rights, and catalog identifiers
- **IDs & Sorting** for MusicBrainz identities and library sort values

To add artwork, choose an image from the artwork panel or drag an image onto it. The artwork context menu also provides removal and detailed image information.

### **Step 4: Apply Changes**

Click **Preview Changes** to review staged differences, then **Write Tags** to commit them to the checked scope. The activity console reports progress and the final outcome. Empty fields and retained tag families are handled according to the active mode and Settings.

## **Edit Modes**

MetaEdit Plus offers two editing modes accessible via the dropdown at the top of the application:

### **Batch Mode** (Default)

In Batch Mode, all metadata changes are applied to every file in the folder simultaneously:

- Fields are shared across all files
- Write Tags applies staged values to the checked files
- Remove Tags removes metadata from the checked files
- Shared album or release values can be entered once
- Ideal for albums where all tracks share the same metadata

> **Note:** In Batch Mode, only non-empty fields are written. Fields left blank will not overwrite existing metadata in the files, allowing you to selectively update specific tags while preserving others.

### **Per-File Mode**

In Per-File Mode, each file has its own individual metadata fields:

- Click on a file in the list to edit its specific metadata
- Changes are cached automatically when switching between files
- Write Tags processes the staged files in the checked scope
- Remove Tags only affects the currently selected file
- Auto-Tag applies results only to the file where it was initiated

> **Note:** In Per-File Mode, all fields are written including empty ones. Clearing a field and writing tags will remove that metadata from the file.

**Context Menu:** In Per-File Mode, right-click on the file list to access:
- **Copy Metadata:** Copies all metadata fields and thumbnail from the selected file
- **Paste Metadata:** Applies copied metadata to the currently selected file
- **Remove Metadata:** Strips all metadata from the selected file and reloads it

This allows you to duplicate or remove metadata between files while still making individual adjustments. Changing the selected file does not silently discard its staged state.

## **Change Preview and Safety**

MetaEdit Plus separates editing from committing. Text tools, file patterns, Rule Studio, CSV import, and the main editor present proposed changes before the final write whenever the workflow can change several files.

- **Preview Changes** lists the affected file and the old and proposed field values.
- **Reset Changes** discards staged edits without writing them.
- **Undo/Redo** stores complete tag and artwork snapshots for supported write operations.
- **Clean & Organize** uses preflight review, backups, transaction state, and rollback protection.
- **Library Integrity** moves selected findings to quarantine and writes a recovery manifest; it does not delete them.

Previews describe the current staged operation. They do not change the checked-file scope, and closing a preview does not write anything.

## **Auto-Tag Feature**

MetaEdit Plus includes an identification and reconciliation workspace for audio metadata. Click **Auto Tag** in the sidebar or press `Ctrl+A` to fingerprint the relevant audio and inspect the result before staging it in the editor.

### **Supported Databases**

Auto Tag combines the following sources:

| Database | Description |
|----------|-------------|
| **AcoustID** | Audio fingerprinting service that identifies tracks by their acoustic signature |
| **MusicBrainz** | Comprehensive open-source music database with millions of releases |
| **iTunes** | Music catalog used for additional metadata evidence and artwork enrichment |

In **App Settings > Auto Tag Settings**, enable the desired sources directly and choose their priority from the adjacent dropdown. Priority influences tie-breaking, but source reliability, match confidence, and cross-source agreement remain part of reconciliation. MusicBrainz must remain enabled for the release-aware batch matcher because its edition and tracklist model comes from MusicBrainz.

### **How It Works**

1. Check the audio files that belong to the operation.
2. Click **Auto Tag** in the sidebar.
3. MetaEdit Plus queries each enabled source in the configured order. AcoustID uses a Chromaprint fingerprint when it is enabled and available.
4. Returned evidence is reconciled into a best result without treating preference as stronger than reliable identity evidence.
5. Review confidence, source coverage, conflicts, metadata choices, and artwork choices.
6. Apply the chosen result to the editor, adjust anything necessary, and use **Preview Changes** before writing.

**Note:** Fingerprinting identifies the audio content rather than trusting the filename. A successful fingerprint is evidence, not an instruction to write immediately; the result still remains reviewable.

### **Metadata Choices**

The Identification section summarizes which services contributed and whether they agree. A reconciled field with more than one source value is interactive: it shows a choice indicator, responds to hover and keyboard focus, and opens a single selector where the preferred value can be chosen. Choosing the field again closes that selector.

Values are presented as metadata, source, and confidence information rather than as an undifferentiated technical string. Fields without alternatives remain ordinary read-only results.

### **Artwork Choices**

Auto Tag is not limited to one image. It first adds the best reconciled cover when one is available, then checks up to eight matching MusicBrainz releases for downloadable front covers. The number actually shown depends on the releases returned by the services and whether those releases expose usable cover art. A selector containing only one item therefore means that no additional downloadable choice was returned for that identification; it is not a one-artwork product limit.

Each choice uses a readable label with its resolution and, when available, release date, country, or edition disambiguation. The selector states how many choices are available. Selecting a different entry updates the staged artwork but does not write it until the normal write workflow is completed.

**Cancel:** During a checked-file Auto Tag queue, a visible **Stop Auto Tag** action appears beside the log tools. `Escape` is also supported while the application has keyboard focus.

**Auto-Tag Workflow:** **Review Current Scope** identifies the selected file in Per-File Mode and opens release matching in Batch Mode. **Identify Checked Files** identifies every checked file independently, switches to Per-File Mode so track-specific fields cannot leak between files, reports per-file progress, and respects service rate limits.

### **Batch Release Matching**

Batch Mode does not assume that every checked file should receive one track's title, composer, identifiers, or artwork. Instead, release matching searches MusicBrainz releases, lets the user select the exact edition, downloads its media and tracklist, and proposes a one-to-one file mapping.

Mapping evidence combines existing track numbers, titles, filenames, and duration. Every row shows its confidence and reason, and its track selector can override the proposal. Assigning a track to another file automatically removes the duplicate assignment. Unmatched files remain unchanged. Accepting the reviewed map stages independent per-file values; optional release artwork is added only to matched files that have no artwork.

## **Text Tools**

The Text Tools window groups three bulk transformations and a shared target-field selector. Open it from the sidebar or press `Ctrl+H`. Its Change Preview presents each file, field, current value, and proposed value in one integrated report rather than applying changes immediately.

### **Find & Replace**

Search and replace text across any selected editable metadata fields:

- Enter the exact text to find and its replacement.
- Choose fields through **Target Fields**; the selector covers the 38 metadata fields rather than a fixed eight-field subset.
- Matching is ordinal and case-sensitive, so a differently capitalized value is not changed accidentally.
- Review the proposed value for each affected file before confirming the operation. Confirmed Text Tools transformations write the affected files directly and create an undo snapshot.

### **Case Conversion**

Convert text case across metadata fields. Four modes are available:

| Mode | Example |
|------|---------|
| **Original** | Leaves the original casing unchanged |
| **Title Case** | `hello world` becomes `Hello World` |
| **UPPERCASE** | `hello world` becomes `HELLO WORLD` |
| **lowercase** | `HELLO WORLD` becomes `hello world` |


Select the metadata fields to convert and preview the results before applying. The same target selection is used by Find & Replace and Case Conversion.

### **File Pattern** (within Text Tools)

The Filename Pattern section can extract tags from filenames or generate filenames from tags using supported placeholders. Its operation and pattern are kept in a separate section because they affect file identity rather than ordinary text replacement.

## **File Pattern Tool**

The File Pattern Tool provides two-way conversion between filenames and metadata tags using customizable patterns. Open it via `Ctrl+Shift+T` (Tag from Filename) or `Ctrl+Shift+R` (Filename from Tags).

### **Tag from Filename**

Extract metadata from filenames using pattern placeholders:

| Placeholder | Field |
|-------------|-------|
| `%artist%` / `%performer%` | Performer |
| `%albumartist%` | Album Artist |
| `%album%` | Album |
| `%year%` | Release Year |
| `%genre%` | Genre |
| `%track%` / `%tracknumber%` | Track Number |
| `%disc%` / `%discnumber%` | Disc Number |
| `%composer%` | Composer |
| `%conductor%` | Conductor |
| `%publisher%` | Publisher |
| `%description%` / `%comment%` | Description |
| `%copyright%` | Copyright |
| `%grouping%` | Grouping |
| `%bpm%` | Beats Per Minute |
| `%isrc%` | ISRC Code |

These are the placeholders accepted by the current filename parser; fields outside this table remain editable elsewhere but are not filename-pattern variables.

**Example:** The pattern `%artist% - %album% - %track% %title%` applied to `Pink Floyd - The Wall - 01 In The Flesh.mp3` extracts the performer, album, track number, and title.

### **Filename from Tags**

Rename files based on their existing metadata using the same pattern placeholders. A preview shows the current and proposed filename and identifies missing data. Generated names are sanitized for Windows filename rules, and confirmed rename plans are preflighted and executed transactionally so swaps, chains, and case-only changes do not overwrite one another.

## **Metadata Import and Export**

The CSV Import / Export window manages the complete checked-file scope through the same metadata schema used by the editor. Choose the operation first; import also keeps the chosen CSV source in that Operation section.

### **Export**

1. Choose the default field set, all fields, or a custom selection.
2. Set **Rows shown in review** to 5, 10, 20, 50, 100, or All and inspect the independently scrollable report.
3. Click **Export...** and choose CSV metadata, JSON metadata, or an M3U8 playlist.

`FilePath` and `Filename` are always included in metadata exports for stable identity. Export Review gives every selected metadata field its own aligned field/value row beneath the file identity. The row selector changes only how many files are displayed in that review: selecting 20 while 200 files are checked still exports all 200 checked files. CSV values use the shared encoder, including quoting and spreadsheet-formula safety. JSON preserves the selected field names in a structured array. M3U8 uses UTF-8, writes `EXTINF` duration/display entries, and prefers relative paths from the playlist location for portability.

### **Import**

1. Select **Import metadata**, browse to a CSV file, and let MetaEdit Plus parse its header.
2. Rows are resolved by full path when available or by an unambiguous filename match.
3. Review the full row report and the matched, skipped, and duplicate-target totals.
4. Click **Import to Files** to write recognized metadata columns to resolved files.

The CSV file must include a full-path column (`FilePath`, `Path`, or `FullPath`) or a filename column (`Filename`, `File`, or `Name`). Header aliases are accepted for compatibility. An ambiguous filename is skipped instead of being guessed, and a repeated row for the same target is disclosed in the duplicate-target count. CSV import creates an undo snapshot before it writes.

## **Rule Studio**

Rule Studio is intended for repeatable, conditional metadata work across checked files. It uses the same field labels as the rest of MetaEdit Plus and keeps rule structure, execution order, and dry-run evidence visible.

1. Name the rule or load a saved preset.
2. Choose **Match all conditions** or **Match any condition**.
3. Add conditions from the section-header action. Conditions can compare Filename or any metadata field using equals, not-equals, contains, starts/ends with, empty/not-empty, regular expressions, list membership, or numeric greater/less-than checks.
4. Add sequential actions and arrange their order. Actions can set or clear a value, copy another field, find/replace, regex replace, prepend/append, set only when empty, normalize whitespace or Unicode, change case, sort/deduplicate multi-values, or generate padded sequence numbers.
5. Run **Dry Preview** to inspect the outcome and explanation for every checked file.
6. Use **Stage Changes** to return matched results to the main editor, then review them before Write Tags.

Each condition and action is presented as a contained editor card with an enable checkbox and anchored duplicate, reorder, or remove controls, while the section header owns the add action. Presets retain complex rule definitions locally and through optional cloud sync, and can be imported or exported as JSON.

## **Clean & Organize**

Clean & Organize builds a reviewed library plan before it changes tags or paths. Choose an existing destination folder and a folder/filename pattern such as `%albumartist%\%album%\%track% - %title%`.

The analysis pipeline fingerprints, identifies, reconciles, normalizes, validates destinations, and preflights every checked file. Its checkpoint summary reports job state, total files, ready and remaining counts, the last checkpoint, and an estimated remaining time. A real progress bar adds current file, percentage, and active stage feedback.

Analysis state is saved so an interrupted job can resume from completed checkpoints. The Review section lists source evidence, conflicts, planned tag changes, fingerprints, failures, and exact destination paths. **Atomic Commit** becomes available only after the job is ready for review; it creates transaction backups and rolls the complete job back if a commit step fails.

## **Library Integrity**

Library Integrity analyzes the checked selection automatically when its window opens. Evidence is cached persistently and invalidated when the relevant file changes, so reopening the workflow can reuse unchanged work instead of rescanning every byte from the beginning.

It distinguishes three kinds of evidence:

- **Exact duplicate:** the complete file is byte-identical according to its SHA-256 hash.
- **Same decoded audio:** the audio content matches even when the container or tags differ.
- **Related release/version:** release identifiers and technical properties indicate a relationship without claiming that the files are duplicates.

Groups show filenames, metadata completeness, artwork presence, technical properties, concise hashes, and a recommended copy where the evidence supports one. Files are never deleted by this workflow. Only explicitly selected redundant copies can be moved to a user-chosen quarantine folder, and a recovery manifest records every original and quarantine path.

## **Advanced Media Tools**

The **More** menu enables advanced actions only when the current selection and media type can use them. Per-file tools require Per-File Mode; loudness analysis operates on checked audio files.

### **Artwork Collection Manager**

**Manage Artwork Collection** opens every embedded image in its stored order, including picture type, description, format, dimensions, and size. Add or replace an image, choose its semantic type, edit its description, reorder it, or remove it. The result remains staged until the normal Write Tags workflow.

Quick Choose/Remove Artwork targets only the picture type selected in Settings and preserves all other picture types. Copy/Paste Metadata transfers the full collection rather than only the visible front cover.

### **Format-Specific Tags**

**Format-Specific Tags** exposes fields outside the standard editor without flattening the container. The applied-field list provides selection and removal; the adjacent editor shows only the selected field, its container, and its values:

- ID3v2 user-text (`TXXX`) fields
- Xiph/Vorbis comment fields
- APEv2 text items
- MP4 `com.apple.iTunes` freeform fields
- ASF text descriptors

Enter one value per line to preserve actual multi-value fields. Unknown or binary data is displayed as read-only and retained. Only added, edited, renamed, or removed fields are changed.

### **Loudness and ReplayGain**

**Loudness & ReplayGain** decodes every checked audio file and measures K-weighted integrated loudness with BS.1770/EBU R128 absolute and relative gating. Results show integrated LUFS, ReplayGain 2 track gain referenced to −18 LUFS, and sample peak. When requested, album gain is calculated by Album plus Album Artist grouping.

Applying the reviewed result writes ReplayGain track gain/peak and, when applicable, album gain/peak tags. The audio samples are never normalized or re-encoded. Analysis can be stopped; partial measurements are not applied.

### **Lyrics Lookup**

**Lyrics Lookup** uses the selected audio file's title, performer, album, and duration to search LRCLIB. Candidates are ranked by metadata similarity and duration, disclose plain/synchronized availability, and remain selectable. Choose synchronized lyrics when available or plain text, then stage the preview in the main editor. **Export Sidecar** writes UTF-8 `.lrc` or `.txt` without staging a tag.

### **Video Details**

**Video Details** presents container, dimensions, duration, video codecs, and video-specific TV/movie fields such as show, season, episode, network, director, producer, screenwriter, content rating, and keywords. Common title, subtitle, description, genre, year, and copyright fields stay exclusively in the main editor, avoiding two competing places for the same tag.

Chapter rows contain start, optional end, title, ordering, and removal controls. Simple chapter text and FFmetadata sidecars can be imported or exported for every supported video. Embedded chapter capability is container-aware:

- Matroska/WebM chapter replacement is enabled when MKVToolNix is detected and does not remux streams.
- MP4/M4V/MOV chapter replacement is enabled when FFmpeg is detected; streams are copied to a validated temporary container before the original is atomically replaced.

When the relevant tool is unavailable, MetaEdit explains the limitation and keeps sidecar workflows available instead of attempting unsafe container byte editing.

## **Action Buttons**

The main workspace keeps frequent actions visible and moves less frequent workflows into **More** when space is limited:

| Button | Description |
|--------|-------------|
| **Auto Tag** | Opens fingerprint identification, source reconciliation, metadata choices, and artwork choices. |
| **Text Tools** | Opens find/replace, case conversion, target fields, and filename patterns. |
| **Preview Changes** | Reviews staged metadata and artwork differences without writing them. |
| **Remove Tags** | Removes metadata from the selected mode and checked scope after creating recovery history. |
| **Write Tags** | Validates and writes the staged metadata and artwork for the selected mode and checked scope. |
| **Save Set / Restore Set** | Stores or restores a reusable field and artwork configuration. |
| **CSV Tools** | Opens reviewed CSV import plus CSV, JSON, and M3U8 export. |
| **More** | Opens Clear/Reset, collection-aware Copy/Paste Metadata, Format-Specific Tags, Video Details, Lyrics Lookup, Loudness & ReplayGain, field sets, interchange, Rule Studio, Clean & Organize, and Library Integrity as allowed by the current scope. |

The action cards respond to the available window width. Controls that move into **More** remain the same operation; changing the window size does not change processing scope.

## **Undo and Redo**

MetaEdit Plus includes a multi-level undo and redo system that can reverse or reapply complete tag operations. Covered workflows create a full standard and extended-tag snapshot of affected files before changing them, including every embedded artwork item and ReplayGain field.

### **How It Works**

- Press `Ctrl+Z` to undo the last tag operation. All files affected by that operation are restored to their previous state.
- Press `Ctrl+Y` to redo an undone operation, reapplying the changes that were reversed.
- Up to **20 undo/redo levels** are supported, so you can step back through multiple operations.
- The redo history is cleared whenever a new tag operation is performed.

### **What Gets Restored**

Each undo/redo snapshot captures the complete metadata state of every file involved in the operation:
- All metadata represented by the editor's tag model, including its 38 exposed fields
- Embedded artwork collections (including image data, order, picture type, and description)
- Extended text fields in supported tag containers

This means that undoing a **Remove Tags** operation will fully restore all stripped metadata and artwork, and undoing a **Write Tags** operation will revert files to their exact state before writing.

### **Console Feedback**

The console displays progress for each undo/redo action, including the name of the operation being reversed, the number of files restored, and how many undo steps remain.

## **Field Storage System**

The field storage system allows you to save and reuse metadata configurations:

1. **Saving:** Fill in the fields you want to save, then click **Store Fields**. The configuration is saved with a field counter and timestamp (e.g., "4 Fields - 04:43 PM").
2. **Loading:** Click **Restore Fields** to see a dropdown of all saved configurations. Use arrow keys to navigate and Enter to select, or click directly on an entry.
3. **Capacity:** Up to 50 configurations can be stored. When the limit is reached, the oldest entry is automatically removed.
4. **Duplicate Detection:** The system uses content hashing to prevent saving identical configurations multiple times.
5. **New Session:** Press `F12` or `Ctrl+N` to clear all fields and start fresh.

## **Settings**

Click the **Settings** icon in the sidebar to open the settings dialog:

### **ID3v2 Version**
- **ID3v2.3** (Default): Best compatibility with Windows Explorer and most media players
- **ID3v2.4**: Modern version with better Unicode support, recommended for international characters

### **Text Encoding**
- **UTF-16** (Default): Best compatibility with ID3v2.3 and Windows media tools
- **UTF-16 BE**: Big-endian Unicode where required by the target software
- **UTF-8**: Available with ID3v2.4
- **Latin1**: Legacy ISO-8859-1 encoding

### **Cover Image Settings**
- **Max Image Size:** Keep the original dimensions or constrain the longest dimension to 300, 500, 800, 1000, 1500, or 2000 pixels. The default is 500 pixels.
- **JPEG Quality:** Choose 70, 80, 85, 90, 95, or 100 percent. The default is 85 percent.
- **Picture Type:** Other, Front Cover, Back Cover, Artist, or Band Logo.
- **PNG Handling:** Convert opaque PNG artwork to JPEG or keep its original PNG representation. Transparency prevents destructive JPEG conversion.

### **Tag Retention**
Control which existing tags are preserved when writing new metadata:
- **Keep ID3v1 Tags**: Preserve legacy ID3v1 tags for older devices
- **Keep ID3v2 Tags**: Preserve modern ID3v2 tags (recommended)
- **Keep APE Tags**: Preserve APE tags used by some audio players

At least one MP3 tag family must remain enabled. Settings validation also prevents UTF-8 from being selected with ID3v2.3.

### **Auto-Tag Settings**
- **Auto Tag workflow:** Choose **Review Current Scope** for an interactive selected-file or batch release review, or **Identify Checked Files** for independent track-by-track identification of the checked scope.
- **Metadata sources:** Enable AcoustID, MusicBrainz, and iTunes and arrange their priority. At least one source must remain enabled; MusicBrainz is required for release matching.

## **Cloud Settings Sync**

MetaEdit Plus supports optional synchronization of tag settings through **[Arctisoft Studio Hub](https://github.com/BerndHagen/Arctisoft-Studio-Hub)**. When a valid Hub session exists, supported preferences are synchronized and can be restored on another Windows device using the same account.

### **How It Works**

1. Sign in to **[Arctisoft Studio Hub](https://github.com/BerndHagen/Arctisoft-Studio-Hub)** on your computer
2. MetaEdit Plus reads the shared authentication session automatically
3. On launch, your cloud settings are loaded and merged with local settings
4. When you save your settings, they are synced to the cloud in the background

### **Synced Settings**

The following settings are synced:
- ID3v2 Version
- Text Encoding
- Cover Image Settings (max size, JPEG quality, picture type, PNG conversion)
- Tag Retention Options
- Auto Tag workflow
- Enabled metadata sources and their priority

**Note:** Cloud sync is optional. If no active [Arctisoft Studio Hub](https://github.com/BerndHagen/Arctisoft-Studio-Hub) session is found, MetaEdit Plus continues with local settings only.

## **Keyboard Shortcuts**

MetaEdit Plus provides keyboard shortcuts for faster workflow:

| Shortcut | Alternative | Function |
|----------|-------------|----------|
| `Ctrl+G` | `F1` | Write Tags |
| `Ctrl+R` | `F2` | Remove Tags |
| `Ctrl+L` | `F3` | Clear Console |
| `Ctrl+T` | `F4` | Restore Fields |
| `Ctrl+S` | `F5` | Store Fields |
| `Ctrl+B` | `F6` | Browse Files |
| `Ctrl+A` | `F7` | Auto-Tag |
| `Ctrl+N` | `F12` | New Session |
| `Ctrl+H` | - | Open Text Tools |
| `Ctrl+F` | - | Search Files |
| `Ctrl+Shift+T` | - | Tag from Filename |
| `Ctrl+Shift+R` | - | Filename from Tags |
| `Ctrl+Z` | - | Undo Last Operation |
| `Ctrl+Y` | - | Redo Last Operation |
| `Space` | - | Toggle inclusion for the selected library rows |
| `Tab` | `Shift+Tab` | Cycle Through Fields when a metadata field is focused |
| `Escape` | - | Cancel Auto-Tag / Clear Focus |

Standard list and dropdown navigation also supports the expected arrow, Home, End, Enter, and Space behavior when the relevant control has keyboard focus.

## **Sidebar**

The left sidebar provides quick access to the main application functions:

| Icon | Function | Description |
|------|----------|-------------|
| **New Session** | `Ctrl+N` / `F12` | Clears all metadata fields, resets the file list, and starts a fresh editing session |
| **Open Files** | — | Opens a multi-select file dialog for supported audio and video files |
| **Auto Tag** | `Ctrl+A` / `F7` | Opens fingerprint identification and source reconciliation |
| **Text Tools** | `Ctrl+H` | Opens find and replace, case conversion, target fields, and filename patterns |
| **CSV Import / Export** | — | Opens reviewed CSV workflows for the checked scope |
| **App Settings** | — | Configures tag containers, encoding, artwork processing, Auto Tag scope, enabled sources, and source priority |
| **Arctisoft Studio Hub** | — | Opens the optional Studio Hub companion experience |
| **Exit App** | — | Closes the application |

`Ctrl+B` / `F6` activates the separate **Add Folder** workflow. The Library panel also provides **Add Files**, **Add Folder**, drag and drop, search, and the include-all checkbox.

## **Context Menus**

MetaEdit Plus provides context menus (right-click) in several areas:

### **Text Fields**
Right-click on any metadata text field to access:
- **Cut Content** - Cut the selected text to clipboard
- **Copy Content** - Copy the selected text to clipboard
- **Paste Content** - Paste text from clipboard into the field

### **Console Output**
Right-click on the console area to access:
- **Copy Console** - Copy all console output to clipboard
- **Clear Console** - Clear all messages from the console

### **Thumbnail Panel**
Right-click on the album artwork panel to access:
- **Choose Artwork** - Open a file dialog to choose an image
- **Manage Artwork Collection** - Review and edit all embedded pictures, types, descriptions, and ordering
- **Remove Artwork** - Remove the staged artwork
- **Artwork Information** - Inspect format, dimensions, size, picture type, and processing behavior

### **Path Bar**
Right-click on the folder path bar to access:
- **Open Source Location** - Open the current source in Windows Explorer
- **Copy Source** - Copy the displayed source path or source description

### **File List** (Per-File Mode only)
Right-click on a file in the list to access:
- **Play Audio Preview / Stop Audio Preview** - Audition supported audio without leaving the editor
- **Copy Metadata** - Copy all metadata fields and the complete artwork collection from the selected file
- **Paste Metadata** - Stage the copied metadata and artwork collection on the selected file
- **Remove Metadata** - Strip all metadata from the selected file
- **Track Information** - Inspect file identity, media properties, and tags for the selected file

## **Copyright**

This software is freeware. You may use it for personal and commercial purposes.

Redistribution is permitted only in its original form with credit to the author.

Modification, decompiling, or reverse-engineering is prohibited without prior written consent.

MetaEdit Plus is provided "as is" without warranty. The author is not liable for any damages resulting from use.

See the [LICENSE](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/blob/main/LICENSE) file for full terms.

## **Screenshots**

If you'd like a preview of MetaEdit Plus before downloading, the screenshots below show the application's features. Note that future updates may introduce additional functionality.

<table>
  <tr>
    <th>MetaEdit Plus - Initial View</th>
    <th>MetaEdit Plus - Directory Scan</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/screenshot-startup.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/screenshot-startup.png" alt="Initial View" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/screenshot-inputs.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/screenshot-inputs.png" alt="Directory Scan" width="450"></a></td>
  </tr>
  <tr>
    <th>MetaEdit Plus - Tag Generation</th>
    <th>MetaEdit Plus - App Settings</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/screenshot-generate.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/screenshot-generate.png" alt="Tag Generation" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/screenshot-settings.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/images/screenshot-settings.png" alt="App Settings" width="450"></a></td>
  </tr>
</table>
