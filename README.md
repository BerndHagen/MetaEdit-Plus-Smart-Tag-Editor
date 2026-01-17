<p align="center">
  <img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit.png" alt="MetaEdit Plus Logo" width="128" />
</p>
<h1 align="center">MetaEdit Plus - Smart Tag Editor</h1>
<p align="center">
  <b>Edit metadata on audio and video files with batch processing and field storage.</b><br>
  <b>Apply tags to entire folders, embed album artwork, and save configurations for reuse.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Freeware-green?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet/10.0/runtime"><img src="https://img.shields.io/badge/.NET-10.0-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/issues"><img src="https://img.shields.io/badge/Issues-0_open-orange?style=flat-square" alt="Open Issues"></a>
</p>

**MetaEdit Plus** is a metadata editor for audio and video files. It processes entire folders at once, allowing you to apply tags to all files simultaneously. The application provides 18 metadata fields organized into three tabs, supports field storage with up to 20 saved configurations, and includes real-time system monitoring with CPU, RAM, and disk usage graphs.

### **Key Features**

- **Batch Processing:** Apply metadata changes to all files in a folder at once, with progress tracking in the console output.
- **Album Artwork:** Embed cover images directly into files via drag-and-drop or file browser selection.
- **Field Storage:** Save up to 20 field configurations with timestamps for quick reuse across different sessions.
- **Multi-Format Support:** Edit metadata in 8 audio formats and 6 video formats with full tag support.
- **System Monitoring:** Real-time performance graphs showing CPU, RAM, and disk usage with numerical statistics.
- **Context Menus:** Quick access to copy, paste, clear console, select/remove images, and open folder locations.

### **Supported Formats**

MetaEdit Plus supports a wide range of audio and video formats:

- **Audio Formats:** `MP3`, `WAV`, `FLAC`, `AAC`, `OGG`, `WMA`, `M4A`, `AIFF`
- **Video Formats:** `MP4`, `MKV`, `MOV`, `WMV`, `M4V`, `WEBM`

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
   - [Step 2: Choose Format and Folder](#step-2-choose-format-and-folder)
   - [Step 3: Edit Metadata Fields](#step-3-edit-metadata-fields)
   - [Step 4: Apply Changes](#step-4-apply-changes)
5. [Action Buttons](#action-buttons)
6. [Field Storage System](#field-storage-system)
7. [Keyboard Shortcuts](#keyboard-shortcuts)
8. [Copyright](#copyright)
9. [Screenshots](#screenshots)

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

### **Step 2: Choose Format and Folder**

1. Select the desired file format from the format dropdown (MP3, FLAC, MP4, etc.)
2. Click **Browse** or press `Ctrl+B` to select a folder containing your media files
3. The application will display the number of files found in the console and list them in the file tree

### **Step 3: Edit Metadata Fields**

Navigate through the three tabs to fill in the metadata fields:
- **Production:** Performer, Album Artist, Composer, Conductor, Total Tracks, Publisher
- **Technical:** Release Year, Track Number, Disc Number, BPM, Total Discs, Album
- **Composition:** Genre, Description, Grouping, Copyright, Lyrics, ISRC Code

To add album artwork, click the thumbnail panel or drag an image directly onto it. Supported image formats are JPG, PNG, GIF, and BMP.

### **Step 4: Apply Changes**

Click **Write Tags** to apply all metadata to the files in the selected folder. The console displays the progress for each file and confirms when processing is complete.

## **Action Buttons**

MetaEdit Plus provides five main action buttons for managing metadata:

| Button | Description |
|--------|-------------|
| **Write Tags** | Applies all current metadata fields and album artwork to every file in the selected folder |
| **Remove Tags** | Strips all metadata from files in the selected folder, leaving them with no tags |
| **Store Fields** | Saves the current field configuration with a timestamp for later use |
| **Restore Fields** | Opens a dropdown menu to select and load a previously saved configuration |
| **Clear Console** | Clears all messages from the console output panel |

## **Field Storage System**

The field storage system allows you to save and reuse metadata configurations:

1. **Saving:** Fill in the fields you want to save, then click **Store Fields**. The configuration is saved with a field counter and timestamp (e.g., "4 Fields - 04:43 PM").
2. **Loading:** Click **Restore Fields** to see a dropdown of all saved configurations. Use arrow keys to navigate and Enter to select, or click directly on an entry.
3. **Capacity:** Up to 20 configurations can be stored. When the limit is reached, the oldest entry is automatically removed.
4. **Duplicate Detection:** The system uses content hashing to prevent saving identical configurations multiple times.
5. **New Session:** Press `F12` or `Ctrl+N` to clear all fields and start fresh.

## **Keyboard Shortcuts**

MetaEdit Plus provides keyboard shortcuts for faster workflow:

| Shortcut | Alternative | Function |
|----------|-------------|----------|
| `Ctrl+G` | `F1` | Write Tags |
| `Ctrl+R` | `F2` | Remove Tags |
| `Ctrl+L` | `F3` | Clear Console |
| `Ctrl+T` | `F4` | Restore Fields |
| `Ctrl+S` | `F5` | Store Fields |
| `Ctrl+B` | `F6` | Browse Folder |
| `Ctrl+N` | `F12` | New Session |

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
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_startup.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_startup.png" alt="Initial View" width="300"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_inputs.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_inputs.png" alt="Directory Scan" width="300"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_generate.png"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_generate.png" alt="Tag Generation" width="300"></a></td>
  </tr>
</table>
