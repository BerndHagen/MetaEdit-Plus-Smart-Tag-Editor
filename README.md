<p align="center">
  <img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit.png" alt="MetaEdit Plus Logo" width="128" />
</p>
<h1 align="center">MetaEdit Plus - Smart Tag Editor</h1>
<p align="center">
  <b>Advanced metadata editor for audio and video files with intuitive batch processing capabilities.</b><br>
  <b>Experience a fast, reliable and streamlined tag editor optimized for professional workflows.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Freeware-green?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet/10.0/runtime"><img src="https://img.shields.io/badge/.NET-10.0-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows%2010%2F11-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/issues"><img src="https://img.shields.io/badge/Issues-0_open-orange?style=flat-square" alt="Open Issues"></a>
</p>

**MetaEdit Plus** is a straightforward metadata editing software designed for managing audio and video file information efficiently. Whether you need to organize your music library, add album artwork or process metadata for multiple files simultaneously, MetaEdit Plus provides an essential solution for all your tagging needs. Its clean, intuitive interface allows you to quickly input metadata, manage cover art, and batch process entire directories with just a few clicks.

### **Key Features**

- **Batch Processing:** Apply metadata to multiple files simultaneously with real-time progress tracking and detailed logging
- **Album Artwork Management:** Drag-and-drop cover art with automatic embedding into file metadata (JPG, PNG, GIF, BMP)
- **Performance Monitoring:** Real-time CPU, RAM, and disk usage display with visual graphs during intensive operations
- **Smart Field Validation:** Automatic validation for numeric fields with placeholder text guidance and error prevention
- **Intelligent File Detection:** Automatic scanning and tree-view display of compatible media files in selected directories  
- **Universal Format Support:** Audio and video files across multiple formats with format-specific optimization

### **Supported Formats**

MetaEdit Plus supports a comprehensive range of media formats for both audio and video content:

- **Audio Formats:** `MP3`, `WAV`, `FLAC`, `AAC`, `OGG`, `WMA`
- **Video Formats:** `MP4`, `AVI`, `MKV`, `MOV`, `WMV`, `FLV`

### **Metadata Management**

Complete control over all standard metadata fields is provided through an organized interface designed for efficient workflow:

- **Production Details:** `Performer`, `Year`, `Composer`, `Publisher`, `Album Artist`, `Copyright`
- **Composition Details:** `Track Number`, `Subtitle`, `Beats per Minute`, `Disc Number`, `Description`, `Genre`

Additionally, album artwork embedding is supported directly into file metadata.
  
TagLib# powers robust metadata processing, ensuring compatibility with industry standards and reliable file handling. All metadata operations include automatic validation and detailed logging for transparency and troubleshooting.

**Note on File Processing:** Processing time depends on file count and system specifications. Progress tracking and system performance monitoring are included during operations.

## **Table of Contents**

1. [System Requirements](#system-requirements)
   - [Minimum Requirements](#minimum-requirements)
   - [Recommended Requirements](#recommended-requirements)
2. [Third-Party Libraries](#third-party-libraries)
   - [TagLib#](#taglib)
   - [System.Management](#systemmanagement)
   - [Additional Information](#additional-information)
3. [Keyboard Shortcuts and Workflow](#keyboard-shortcuts-and-workflow)
4. [Performance Monitoring Features](#performance-monitoring-features)
5. [Main Operations](#main-operations)
6. [Getting Started Guide](#getting-started-guide)
   - [Step 1: Configure Your Library](#step-1-configure-your-library)
   - [Step 2: Process Your Files](#step-2-process-your-files)
7. [Main Operations](#main-operations)
8. [Field Management System](#field-management-system)
9. [Copyright](#copyright)
10. [Screenshots](#screenshots)

## **System Requirements**

### **Minimum Requirements**
- **Operating System:** Windows 10/11 (64-bit)
- **Processor:** Dual-core processor, 1.5 GHz or higher
- **RAM:** 4 GB
- **Graphics:** DirectX 11 compatible (integrated graphics acceptable)
- **Software:** .NET 10.0 Runtime
  - [Download .NET 10.0 Runtime](https://dotnet.microsoft.com/download/dotnet/10.0/runtime)
- **Storage:** 20 MB of free disk space

### **Recommended Requirements**
- **Operating System:** Windows 10/11 (64-bit)
- **Processor:** Quad-core processor, 2.0 GHz or higher
- **RAM:** 8 GB or higher
- **Software:** .NET 10.0 Runtime
- **Storage:** 50 MB of free disk space

## Third-Party Libraries

Two main third-party libraries handle metadata processing and system monitoring:

### TagLib#

TagLib# is a .NET library for reading and writing metadata in media files. It provides robust support for various audio and video formats with reliable tag management capabilities. MetaEdit Plus automatically uses the latest compatible TagLib# version to ensure optimal performance and format support.

- **Website:** [TagLib# GitHub Repository](https://github.com/mono/taglib-sharp)
- **License:** TagLib# is licensed under the LGPL, allowing free use and distribution.

### System.Management

System.Management is a .NET namespace that provides access to management information and management events about the system, devices, and applications. Real-time performance monitoring and system resource tracking during batch operations are powered by System.Management integration.

- **Website:** [System.Management Documentation](https://docs.microsoft.com/en-us/dotnet/api/system.management)
- **License:** System.Management is part of the .NET ecosystem and follows Microsoft's licensing terms.

### Additional Information

For more details about TagLib# and System.Management, including their capabilities and licensing, check their official documentation:

- **TagLib# Documentation:** [TagLib# API Reference](https://github.com/mono/taglib-sharp/tree/main/docs)
- **System.Management Documentation:** [Microsoft Documentation](https://docs.microsoft.com/en-us/dotnet/api/system.management)

If you have questions or issues related to these libraries, please [open an issue](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/issues) on GitHub.

## **Keyboard Shortcuts and Workflow**

Comprehensive keyboard shortcuts are included to maximize productivity and streamline your metadata editing workflow. These shortcuts work globally throughout the interface.

| Shortcut | Alternative | Function | Description |
|----------|-------------|----------|-------------|
| `Ctrl+G` | `F1` | Write Tags | Apply metadata to all files in the current directory |
| `Ctrl+R` | `F2` | Delete Tags | Remove all metadata from files in the current directory |
| `Ctrl+L` | `F3` | Clear Console | Clear the console output and log history |
| `Ctrl+T` | `F4` | Restore Fields | Load previously stored field configurations |
| `Ctrl+S` | `F5` | Store Fields | Save current field configurations for future use |
| `Ctrl+B` | `F6` | Browse Folder | Open folder browser to select media directory |

## **Performance Monitoring Features**

Built-in performance monitoring helps you track system resource usage during intensive batch operations:

- **CPU Usage:** Track processor utilization during metadata processing operations
- **RAM Usage:** Monitor memory consumption to prevent system slowdowns
- **Disk Usage:** Observe storage device activity during file operations
- **Performance Graphs:** Visual representation of system resource trends over time with live updating charts

## **Main Operations**

MetaEdit Plus provides five core functions for comprehensive metadata management:

**Write Tags:** Applies all configured metadata fields from both Production and Composition tabs to every file in the selected directory. Each file receives the entered metadata values, an automatic title based on filename, and thumbnail embedding if artwork is selected. Progress is tracked with detailed console logging.

**Delete Tags:** Completely removes all existing metadata from files in the current directory, including text fields, numeric properties, and embedded artwork, returning files to their original untagged state.

**Store Fields:** Saves all currently entered field data and selected thumbnail image to memory for later use. Multiple configurations can be stored (up to 20) and are displayed with timestamps showing the number of fields saved.

**Restore Fields:** Opens a dropdown showing previously stored field configurations with timestamps. Selecting an entry instantly restores all saved field data and thumbnail image, repopulating all interface elements with saved data for repeated use across different directories.

**Clear Console:** Resets the console output area by removing all logged messages and reports while preserving current session data and field configurations.

## **Getting Started Guide**

Follow these steps to start managing your media metadata efficiently:

### **Step 1: Configure Your Library**

1. **Select Library Type**
   - Launch **MetaEdit Plus** and choose between `Audio Library` or `Video Library` from the dropdown menu.

2. **Choose File Format**
   - Select your preferred file format from the available options (MP3, MP4, etc.).

### **Step 2: Process Your Files**

1. **Browse Directory**
   - Click the **Browse** button or use `Ctrl+B` to select a folder containing your media files.
   - A file tree will populate with all compatible files found in the directory.

2. **Configure Metadata Fields**

   - **Production Details Tab:**
     - Enter performer, year, composer, publisher, album artist, and copyright information.
     - Use the intelligent placeholder system to guide your input.
     
   - **Composition Details Tab:**
     - Configure track numbers, subtitles, BPM, disc numbers, descriptions, and genre information.
     - Numeric fields include automatic validation to prevent errors.
     
3. **Add Album Artwork**
   - Click the thumbnail area to browse for cover art images.
   - Alternatively, drag and drop image files directly onto the thumbnail.
   - Supported formats include JPG, PNG, GIF, and BMP.

4. **Apply Changes**
   - Click **Write Tags** or press `Ctrl+G` to apply metadata to all files in the directory.
   - **Monitor Progress:** Watch the console output for real-time processing information and completion status.
   - **Handle Errors:** Review any error messages for files that couldn't be processed.

**Note:** If you encounter processing errors, ensure files are not in use by other applications and that you have write permissions to the target directory. Processing will continue for remaining files even if individual files encounter errors.

## **Field Management System**

Smart input features prevent common data entry errors:

- **Smart Placeholders:** Contextual placeholder text guides data entry and is automatically excluded from processing
- **Input Validation:** Numeric fields (Year, Track Number, Disc Number, BPM) only accept valid numbers
- **Format Consistency:** TagLib# ensures metadata follows industry standards across all files

## **Copyright**

This software is the intellectual property of the Author and is protected by international copyright laws. This copyright notice outlines the key terms governing the use, distribution, and modification of the software:

1. **License**: You are granted a revocable, non-exclusive, non-transferable license to download, install, and use the software for personal and commercial purposes free of charge.

2. **Modifications Prohibited**: Any modification, decompiling, reverse-engineering, or derivative work based on the software is strictly prohibited without the Author's prior written consent.

3. **Distribution**: Redistribution of the software is permitted only in its original, unmodified form. When redistributing MetaEdit Plus, appropriate credit to the Author is required, including a link to the original source.

4. **Third-Party Libraries**: MetaEdit Plus uses third-party libraries like TagLib# (LGPL) and System.Management (.NET ecosystem). Please review and comply with their respective licenses.

5. **Warranty Disclaimer**: MetaEdit Plus is provided *"as is,"* without warranties of any kind, express or implied. The Author assumes no liability for damages resulting from the use of the software.

6. **Limitation of Liability**: The Author is not responsible for any indirect, special, incidental, or consequential damages arising out of the use or inability to use the software.

7. **Termination**: The license to use this software may be terminated if the terms of this notice are violated. Upon termination, all use must cease and copies must be deleted.

By using MetaEdit Plus, you agree to these terms and conditions. For full details on licensing terms and further information, please refer to the [LICENSE](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/blob/main/LICENSE) file.

## **Screenshots**

If you'd like a preview of MetaEdit Plus before downloading, the screenshots below show the application's interface and features. Note that future updates may introduce additional functionality and interface improvements.

<table>
  <tr>
    <th>MetaEdit Plus - Initial View</th>
    <th>MetaEdit Plus - Directory Scan</th>
    <th>MetaEdit Plus - Tag Generation</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_startup.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_startup.png" alt="MetaEdit Main Interface" width="300"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_inputs.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_inputs.png" alt="MetaEdit Production Details" width="300"></a></td>
    <td><a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_generate.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/raw/main/img/v1.0.8-metaedit_generate.png" alt="MetaEdit Composition Details" width="300"></a></td>
  </tr>
</table>
