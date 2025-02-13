<p align="center">
  <img src="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/blob/f65dcaa1163a518506a3580ee0b87e1e4cf664b6/img/v1.0.3-metaedit.png" alt="MetaEdit Plus Logo" width="128" />
</p>
<h1 align="center">MetaEdit Plus - Smart Tag Editor</h1>
<p align="center">
  <b>Effortlessly manage, edit and organize metadata for your audio and video files.</b><br>
  <b>Experience a powerful and user-friendly tag editor optimized for efficiency.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Freeware-red?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet-framework/net472"><img src="https://img.shields.io/badge/.NET-4.7.2-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">&nbsp;&nbsp;<a href="https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/issues"><img src="https://img.shields.io/github/issues/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor?style=flat-square&color=orange" alt="Open Issues"></a>
</p>

MetaEdit Plus is an advanced tool designed to streamline the organization and updating of metadata in digital audio and video files. Metadata is information embedded within a file that provides details such as the title, artist, album, creation date and thumbnail cover. With MetaEdit Plus, users can effortlessly insert, revise or remove this metadata, simplifying the process of sorting, searching and managing large collections of media files. The software also offers batch editing capabilities, allowing multiple files to be updated at once, which saves a lot of time.

MetaEdit Plus supports a broad range of file formats. For audio, it works with formats like **MP3, WAV, WMA, OGG, FLAC, AAC, M4A, and OPUS**, while for video files, it supports **MP4, AVI, MKV, MOV, WMV, FLV, WEBM, and MPG**. Inspired by my Medio project, which is for downloading YouTube videos and extracting audio, MetaEdit Plus features a user-friendly design that ensures accessibility for users of all technical levels.

This tool, created with Visual Studio 2022, is compatible with most Windows operating systems and requires [.NET Framework 4.7.2](https://dotnet.microsoft.com/en-us/download/dotnet-framework/net472) or higher.

## Table of Contents

1. [System Requirements](#system-requirements)
    - [Minimum Requirements](#minimum-requirements)
    - [Recommended Requirements](#recommended-requirements)
2. [Getting Started](#getting-started)
    - [Initial Setup](#initial-setup)
    - [Metadata Management](#metadata-management)
    - [Finalizing Your Edits](#finalizing-your-edits)
3. [Updating Software](#updating-software)
4. [Third-Party Libraries](#third-party-libraries)
5. [Copyright](#copyright)
6. [Screenshots](#screenshots)

## System Requirements

### Minimum Requirements
- **Operating System:** Windows 7 or higher
- **Processor:** Dual-core processor (e.g., Intel Pentium or AMD Athlon)
- **RAM:** 2 GB
- **Storage:** 10 MB of free disk space for the application
- **Software:** .NET Framework 4.7.2 or higher
    - [Download .NET Framework 4.7.2](https://dotnet.microsoft.com/download/dotnet-framework/net472)

### Recommended Requirements
- **Operating System:** Windows 7 or higher
- **Processor:** Intel Core i5 or AMD Ryzen 5
- **RAM:** 4 GB or higher
- **Storage:** 10 MB of free disk space for the application
- **Software:** .NET Framework 4.8 or higher
    - [Download .NET Framework 4.8](https://dotnet.microsoft.com/download/dotnet-framework/net48)

## Getting Started

To start tagging your audio and video files, simply follow these steps:

### Initial Setup

1. **Select File Type**: At the top dropdown menu, choose between `Video Library` or `Audio Library` to specify the type of files you are working with.
2. **Choose Format**: From the next dropdown, select the exact format of your files to ensure they are correctly catalogued.
3. **Browse for Files**: Click the `Browse` button to navigate to and select the folder containing your media files. Once loaded, your files will be displayed in the Directory and the console will show a message confirming the number of files detected.

### Metadata Management

- **Accessing Details Tabs**: Directly above the `Browse` button, you will find two tabs: `Production Details` and `Composition Details`. These tabs allow you to switch between different fields for entering metadata.
- **Adding Thumbnails**: To add a thumbnail to all files in a folder, click on the Picturebox to select an image, or simply drag and drop an image into it.

### Finalizing Your Edits

- **Generate Tags**: After filling in the necessary information, press `Generate Tags` to start the metadata embedding process for your files.
- **Remove Tags**: To strip all metadata from your files, click `Remove Tags`.
- **Archive Inputs**: Use `Archive Inputs` to clear and temorary back up your current inputs.
- **Retrieve Inputs**: Click `Retrieve Inputs` to restore your saved information into the fields.
- **Clear Console**: Press the `Clear Console` button to remove all entries from the console.

## Updating Software

To ensure optimal performance and stability when editing metadata with MetaEdit Plus - Smart Tag Editor, it's important to use the latest version of the software. Updates provide enhanced features and resolve issues that could affect the software's functionality. The Build Number version can be found in a small window of the application, which can be used to check for the latest version available on this [GitHub Repository](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/releases/tag/v1.0.3-metaedit).

To update your MetaEdit Plus - Smart Tag Editor software, follow these steps:

1. Download the latest version from the repository and save it to your device.
2. Extract the contents from the downloaded **ZIP** folder and run the MetaEdit Plus setup to start the installation process.
3. Follow the on-screen instructions to complete the installation, replacing any old files with the new updates.
4. After installation is complete, open the application.

For optimal performance, ensure that the installation path is set to `C:\Users\...\AppData\Local\Arctisoft-Studio\MetaEdit Plus - Smart Tag Editor` during setup. This helps avoid potential issues and ensures that features are not blocked due to a lack of administrative rights.

## Third-Party Libraries

MetaEdit leverages several third-party libraries to enhance its functionality. One key library used in the application is **TagLib**, which plays a crucial role in handling metadata for media files.

- **TagLib:** TagLib is a library for reading and editing metadata in audio files. It is used by MetaEdit to manage and manipulate tags such as artist, album, and genre information, facilitating better organization and search capabilities for media files.

  - **Website:** [TagLib Official Website](https://taglib.org)
  - **License:** TagLib is licensed under the GNU LGPL (Lesser General Public License).

For more details about TagLib, including its features and licensing, please refer to the [TagLib documentation](https://taglib.org/documentation.html).

If you have any questions or issues regarding the use of TagLib with MetaEdit, feel free to [open an issue](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/issues) on GitHub.

## Copyright 
This software is the intellectual property of the Author and is protected by international copyright laws. By using MetaEdit Plus, you explicitly agree to the following terms:

### License Terms
- Free for personal, non-commercial use only
- No redistribution rights except for promotional purposes
- Non-transferable, revocable license
- Subject to immediate termination for violations

### Legal Protections
1. **Intellectual Property**: All rights, including copyrights, patents, and trade secrets, remain exclusively with the Author.
2. **Indemnification**: Users must indemnify the Author against any claims arising from their use of the software.
3. **Data Protection**: Users are responsible for compliance with data protection laws in their jurisdiction.
4. **Jurisdiction**: Any disputes fall under the exclusive jurisdiction of courts in the Author's jurisdiction.

### Liability and Warranties
- Provided "AS IS" without any warranties
- No liability for any damages or losses
- Users assume all risks associated with use
- Author disclaims all implied warranties

For complete terms, see the [LICENSE](https://github.com/BerndHagen/MetaEdit-Plus-Smart-Tag-Editor/blob/main/LICENSE) file.

## Screenshots
If you want to see how MetaEdit Plus looks before downloading, check out the screenshots below. The images illustrate the tagging process in step by step. From the initial startup screen to adding tags for your files, these screenshots guide you through the entire process.

| MetaEdit - Opening Screen | MetaEdit - Select Directory    | MetaEdit - Generating Tags  |
|------------------------------|------------------------------|------------------------------|
| <img src="https://github.com/BerndHagen/MetaEdit-Tag-Editor/raw/main/img/v1.0.3-metaedit_startup.png" width="300px"> | <img src="https://github.com/BerndHagen/MetaEdit-Tag-Editor/raw/main/img/v1.0.3-metaedit_inputs.png" width="300px"> | <img src="https://github.com/BerndHagen/MetaEdit-Tag-Editor/raw/main/img/v1.0.3-metaedit_generate.png" width="300px"> |
