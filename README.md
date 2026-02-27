<p align="center">
  <img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.1.5-metaedit.png" alt="MetaEdit Plus Logo" width="128" />
</p>
<h1 align="center">MetaEdit Plus - Smart Tag Editor</h1>
<p align="center">
  <b>Edit metadata on audio and video files with batch processing and field storage.</b><br>
  <b>Apply tags to entire folders, embed album artwork, and save configurations for reuse.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Freeware-green?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet/10.0/runtime"><img src="https://img.shields.io/badge/.NET-10.0-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/issues"><img src="https://img.shields.io/badge/Issues-0_open-orange?style=flat-square" alt="Open Issues"></a>
</p>

**MetaEdit Plus** is a metadata editor for audio and video files. It processes entire folders at once, allowing you to apply tags to all files simultaneously, or edit files individually in Per-File Mode. The application provides 18 metadata fields organized into three tabs, supports field storage with up to 50 saved configurations, features automatic metadata lookup from online databases, and includes real-time system monitoring with CPU, RAM, and disk usage graphs.

### **Key Features**

- **Batch Processing:** Apply metadata changes to all files in a folder at once, with progress tracking in the console output.
- **Per-File Mode:** Edit metadata for individual files separately, with automatic caching of unsaved changes when switching between files.
- **Auto-Tag:** Automatically fetch metadata from AcoustID, MusicBrainz, and VGMdb databases using audio fingerprinting technology.
- **Album Artwork:** Embed cover images directly into files via drag-and-drop, with automatic compression to 500px and JPEG 85% quality.
- **Field Storage:** Save up to 50 field configurations with timestamps for quick reuse across different sessions.
- **Copy/Paste/Remove Metadata:** Copy metadata from one file and paste it to another, or remove all metadata from a selected file, via right-click context menu in Per-File Mode.
- **Settings Dialog:** Configure ID3v2 version (2.3/2.4), text encoding (UTF-8/UTF-16/Latin1), cover image settings, tag retention options, and auto-tag scope.
- **Auto-Update:** Check for new versions directly from the application with one-click update installation.
- **Multi-Format Support:** Edit metadata in 7 audio formats and 6 video formats with full tag support.
- **System Monitoring:** Real-time performance graphs showing CPU, RAM, and disk usage with numerical statistics.
- **Context Menus:** Quick access to copy, paste, clear console, select/remove images, copy/paste/remove metadata, and open folder locations.

### **Supported Formats**

MetaEdit Plus supports a wide range of audio and video formats:

- **Audio Formats:** `MP3`, `WAV`, `FLAC`, `OGG`, `WMA`, `M4A`, `AIFF`
- **Video Formats:** `MP4`, `MKV`, `MOV`, `WMV`, `M4V`, `WEBM`

> **Note:** Raw AAC files are not supported as they lack a proper tag container. Please use M4A (AAC in MP4 container) instead.

### **Available Metadata Fields**

MetaEdit Plus provides 18 metadata fields organized into three tabs:

- **Production:** Performer, Album Artist, Composer, Conductor, Total Tracks, Publisher
- **Technical:** Release Year, Track Number, Disc Number, Beats Per Minute, Total Discs, Album
- **Composition:** Genre, Description, Grouping, Copyright, Lyrics, ISRC Code

Additionally, album artwork can be embedded directly into files through the thumbnail panel. The file title is automatically set to the filename during tag generation.

## **Table of Contents**

1. [System Requirements](#system-requirements)
   - [Minimum Requirements](#minimum-requirements)
   - [Recommended Requirements](#recommended-requirements)
2. [Third-Party Libraries](#third-party-libraries)
   - [TagLib#](#taglib)
3. [Installation](#installation)
4. [Getting Started Guide](#getting-started-guide)
   - [Step 1: Select Library Type](#step-1-select-library-type)
   - [Step 2: Choose Format and Select Files](#step-2-choose-format-and-select-files)
   - [Step 3: Edit Metadata Fields](#step-3-edit-metadata-fields)
   - [Step 4: Apply Changes](#step-4-apply-changes)
5. [Edit Modes](#edit-modes)
6. [Auto-Tag Feature](#auto-tag-feature)
7. [Action Buttons](#action-buttons)
8. [Field Storage System](#field-storage-system)
9. [Settings](#settings)
10. [Keyboard Shortcuts](#keyboard-shortcuts)
11. [Copyright](#copyright)
12. [Screenshots](#screenshots)

## **System Requirements**

### **Minimum Requirements**
- **Operating System:** Windows 10 (64-bit) version 1809 or later
- **Processor:** Dual-core processor at 1.5 GHz
- **RAM:** 4 GB
- **Storage:** 150 MB of free disk space
- **Software:** .NET 10.0 Runtime ([Download](https://dotnet.microsoft.com/download/dotnet/10.0/runtime)) - **Not required as application is self-contained**

### **Recommended Requirements**
- **Operating System:** Windows 10/11 (64-bit) version 21H2 or later
- **Processor:** Quad-core processor at 2.0 GHz or higher
- **RAM:** 8 GB or higher
- **Storage:** 200 MB of free disk space on SSD
- **Software:** .NET 10.0 Runtime ([Download](https://dotnet.microsoft.com/download/dotnet/10.0/runtime)) - **Not required as application is self-contained**

**Note:** MetaEdit Plus is designed exclusively for Windows. Linux and macOS are not supported. The .NET 10.0 Runtime is bundled directly in the installer, allowing MetaEdit Plus to start immediately without requiring separate installation.

## **Third-Party Libraries**

MetaEdit Plus uses one main third-party library to handle metadata reading and writing: **TagLib#**.

### TagLib#

**TagLib#** is a .NET library for reading and writing metadata in media files. It provides support for various audio and video formats and handles tag formats such as ID3v1, ID3v2, APE, Xiph Comments, and more. MetaEdit Plus uses TagLib# for all metadata operations.

- **Website:** [TagLib# GitHub Repository](https://github.com/mono/taglib-sharp)
- **License:** TagLib# is licensed under the LGPL (GNU Lesser General Public License), allowing free use in both open-source and proprietary applications.

For more details about TagLib# including its capabilities and supported formats, check the official documentation:

- **TagLib# Documentation:** [TagLib# API Documentation](https://github.com/mono/taglib-sharp#readme)

If you have questions or issues related to this library, please [open an issue](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/issues) on GitHub.

## **Installation**

1. Download the latest release from the [Releases](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/releases) page.
2. Run the installer and follow the setup wizard.
3. Launch MetaEdit Plus from the Start Menu or Desktop shortcut.

## **Getting Started Guide**

### **Step 1: Select Library Type**

When you open MetaEdit Plus, select either **Audio Library** or **Video Library** from the dropdown at the top left. This determines which file formats are available in the format selector.

### **Step 2: Choose Format and Select Files**

1. Select the desired file format from the format dropdown (MP3, FLAC, MP4, etc.)
2. Click **Browse** or press `Ctrl+B` to select media files for editing
3. The application will display the number of files found in the console and list them in the file panel

**Drag & Drop:** You can also drag files or folders directly onto the file list panel:
- **Dragging a folder:** Loads all matching files from that folder
- **Dragging files from the same folder:** Adds them to the existing list (duplicates are skipped)
- **Dragging files from a different folder:** Replaces the entire list with the new files

**Note:** All files in the list must be from the same directory. Files from different folders cannot be mixed.

### **Step 3: Edit Metadata Fields**

Navigate through the three tabs to fill in the metadata fields:
- **Production:** Performer, Album Artist, Composer, Conductor, Total Tracks, Publisher
- **Technical:** Release Year, Track Number, Disc Number, BPM, Total Discs, Album
- **Composition:** Genre, Description, Grouping, Copyright, Lyrics, ISRC Code

To add album artwork, click the thumbnail panel or drag an image directly onto it. Supported image formats are JPG, PNG, GIF, and BMP.

### **Step 4: Apply Changes**

Click **Write Tags** to apply all metadata to the files in the selected folder. The console displays the progress for each file and confirms when processing is complete.

## **Edit Modes**

MetaEdit Plus offers two editing modes accessible via the dropdown at the top of the application:

### **Batch Mode** (Default)

In Batch Mode, all metadata changes are applied to every file in the folder simultaneously:

- Fields are shared across all files
- Write Tags applies changes to all files at once
- Remove Tags removes metadata from all files
- Auto-Tag searches once and applies to all files
- Ideal for albums where all tracks share the same metadata

### **Per-File Mode**

In Per-File Mode, each file has its own individual metadata fields:

- Click on a file in the list to edit its specific metadata
- Changes are cached automatically when switching between files
- Write Tags only writes files that have been modified
- Remove Tags only affects the currently selected file
- Auto-Tag applies results only to the file where it was initiated

**Context Menu:** In Per-File Mode, right-click on the file list to access:
- **Copy Metadata:** Copies all metadata fields and thumbnail from the selected file
- **Paste Metadata:** Applies copied metadata to the currently selected file
- **Remove Metadata:** Strips all metadata from the selected file and reloads it

This allows you to quickly duplicate or remove metadata between files while still making individual adjustments.

## **Auto-Tag Feature**

MetaEdit Plus includes an automatic metadata lookup feature that searches online databases to find album and track information. Click the **Auto** icon in the sidebar or press `Ctrl+A` to initiate a search.

### **Supported Databases**

The Auto-Tag feature searches the following sources in order until a match is found:

| Database | Description |
|----------|-------------|
| **AcoustID** | Audio fingerprinting service that identifies tracks by their acoustic signature |
| **MusicBrainz** | Comprehensive open-source music database with millions of releases |
| **VGMdb** | Specialized database for video game, anime, and soundtrack music |

### **How It Works**

1. Select files in your folder
2. Click the **Auto** icon in the sidebar
3. The application generates an audio fingerprint and searches databases
4. Found metadata and album artwork are automatically populated into the fields
5. Review and modify the results as needed
6. Click **Write Tags** to apply the metadata

**Note:** Auto-Tag uses AcoustID fingerprinting technology (powered by Chromaprint) to identify audio files by their acoustic signature. This provides more accurate results than filename-based searches. VGMdb is specifically used for video game and anime soundtracks.

## **Action Buttons**

MetaEdit Plus provides five main action buttons for managing metadata:

| Button | Description |
|--------|-------------|
| **Write Tags** | Applies all current metadata fields and album artwork. In Batch Mode, writes to all files. In Per-File Mode, writes only modified files. |
| **Remove Tags** | Strips all metadata from files. In Batch Mode, removes from all files. In Per-File Mode, removes only from the selected file. |
| **Store Fields** | Saves the current field configuration with a timestamp for later use (fields are preserved, not cleared) |
| **Restore Fields** | Opens a dropdown menu to select and load a previously saved configuration |
| **Clear Console** | Clears all messages from the console output panel |
| **Undo** | Reverses the last tag operation. Supports multiple undo levels for Write Tags, Remove Tags, and Auto-Tag. |
| **Redo** | Re-applies an undone tag operation. Available after using Undo. |

## **Field Storage System**

The field storage system allows you to save and reuse metadata configurations:

1. **Saving:** Fill in the fields you want to save, then click **Store Fields**. The configuration is saved with a field counter and timestamp (e.g., "4 Fields - 04:43 PM").
2. **Loading:** Click **Restore Fields** to see a dropdown of all saved configurations. Use arrow keys to navigate and Enter to select, or click directly on an entry.
3. **Capacity:** Up to 50 configurations can be stored. When the limit is reached, the oldest entry is automatically removed.
4. **Duplicate Detection:** The system uses content hashing to prevent saving identical configurations multiple times.
5. **New Session:** Press `F12` or `Ctrl+N` to clear all fields and start fresh.

## **Settings**

Click the **Settings** icon in the sidebar or press `Ctrl+Shift+S` to open the settings dialog:

### **ID3v2 Version**
- **ID3v2.3** (Default): Best compatibility with Windows Explorer and most media players
- **ID3v2.4**: Modern version with better Unicode support, recommended for international characters

### **Text Encoding**
- **UTF-8** (Default): Universal encoding supporting all characters
- **UTF-16**: Alternative encoding for special character sets
- **Latin1**: Legacy encoding for maximum compatibility with older software

### **Cover Image Settings**
- **Max Image Size**: Maximum pixel dimension for embedded artwork (default: 500px)
- **JPEG Quality**: Compression quality percentage for JPEG images (default: 85%)
- **Picture Type**: Choose the tag picture type (Front Cover, Back Cover, Artist, Band, etc.)
- **Convert PNG**: Automatically convert PNG images to JPEG to reduce file size, or keep as PNG

### **Tag Retention**
Control which existing tags are preserved when writing new metadata:
- **Keep ID3v1 Tags**: Preserve legacy ID3v1 tags for older devices
- **Keep ID3v2 Tags**: Preserve modern ID3v2 tags (recommended)
- **Keep APE Tags**: Preserve APE tags used by some audio players

### **Auto-Tag Settings**
- **Auto-Tag Scope**: Choose between "Selected File Only" (applies auto-tag results only to the current file) and "All Files in List" (applies to every file in the list)

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
| `Ctrl+Z` | — | Undo Last Operation |
| `Ctrl+Y` | — | Redo Last Operation |
| `Ctrl++` | — | Zoom In |
| `Ctrl+-` | — | Zoom Out |
| `Ctrl+0` | — | Reset Zoom |
| `Escape` | — | Clear Focus |

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
    <th>MetaEdit Plus - Tag Generation</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.1.5-metaedit_startup.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.1.5-metaedit_startup.png" alt="Initial View" width="300"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.1.5-metaedit_inputs.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.1.5-metaedit_inputs.png" alt="Directory Scan" width="300"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.1.5-metaedit_generate.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.1.5-metaedit_generate.png" alt="Tag Generation" width="300"></a></td>
  </tr>
</table>
