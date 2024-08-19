# MetaEdit Plus - Smart Tag Editor
MetaEdit Plus is an advanced tool designed to simplify the organization and updating of metadata within digital audio and video files. Metadata includes details such as the title, artist, album, creation date and thumbnail cover. With MetaEdit Plus, users can easily insert, revise or remove this metadata, making it easier to sort, search and manage extensive libraries of media files. The software also supports batch editing, allowing multiple files to be updated simultaneously, saving time and effort.

MetaEdit Plus supports a wide range of file formats. In the Audio Library, it handles formats such as **MP3, WAV, WMA, OGG, FLAC, AAC, M4A and OPUS**. For videos, the supported formats include **MP4, AVI, MKV, MOV, WMV, FLV, WEBM and MPG**. The software's design, inspired by another project called Medio for downloading YouTube videos and extracting audio, ensures a user-friendly experience. The intuitive interface makes it accessible to users of all technical backgrounds.

Developed using Visual Studio 2022, MetaEdit Plus is compatible with the majority of `Windows` operating systems and requires the `.NET Framework 4.7.2` or higher. You can download the required .NET Framework [here](https://dotnet.microsoft.com/en-us/download/dotnet-framework/net472).

# Getting Started

To start tagging your audio and video files, simply follow these steps:

### Initial Setup

1. **Select File Type**: At the top dropdown menu, choose between `Video Library` or `Audio Library` to specify the type of files you are working with.
2. **Choose Format**: From the next dropdown, select the exact format of your files to ensure they are correctly catalogued.
3. **Browse for Files**: Click the `Browse` button to navigate to and select the folder containing your media files. Once loaded, your files will be displayed in the Directory, and the console will show a message confirming the number of files detected.

### Metadata Management

- **Accessing Details Tabs**: Directly above the `Browse` button, you will find two tabs: `Production Details` and `Composition Details`. These tabs allow you to switch between different fields for entering metadata.
- **Adding Thumbnails**: To add a thumbnail to all files in a folder, click on the Picturebox to select an image, or simply drag and drop an image into it.

### Finalizing Your Edits

- **Generate Tags**: After filling in the necessary information, press `Generate Tags` to start the metadata embedding process for your files.
- **Remove Tags**: To strip all metadata from your files, click `Remove Tags`.
- **Archive Inputs**: Use `Archive Inputs` to clear and temorary back up your current inputs.
- **Retrieve Inputs**: Click `Retrieve Inputs` to restore your saved information into the fields.
- **Clear Console**: Press the `Clear Console` button to remove all entries from the console, ensuring a cleaner view.

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

# Copyright 
This software program, **MetaEdit Plus**, is an intellectual creation of me, Bernd Hagen, the author and copyright holder, and is protected by copyright law. This comprehensive copyright notice outlines the terms and conditions governing the use, distribution, and modification of MetaEdit Plus:

1. **License**:  MetaEdit Plus is made available for free download and use without requiring a license. You are granted a limited, non-exclusive, and non-transferable right to use the software in accordance with the terms set forth herein.

2. **Prohibited Modifications**: You are expressly prohibited from modifying, decompiling, disassembling, reverse engineering, or otherwise manipulating MetaEdit Plus in any manner. Any attempts to do so will be deemed a clear violation of this copyright.

3. **Warranty Disclaimer**: MetaEdit Plus is provided *"as is,"* without any warranty of any kind, whether express or implied. This includes, but is not limited to, warranties of merchantability, fitness for a particular purpose, and noninfringement. The author and copyright holder make no guarantees regarding the accuracy, reliability, or performance of the software.

4. **Limitation of Liability**: In no event shall the author or copyright holder be held liable for any claims, damages, or other liabilities, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the software or the use thereof. You expressly understand and agree that you assume all risks associated with the use of MetaEdit Plus.

By downloading, installing, or using MetaEdit Plus, you acknowledge that you have read and understood this copyright notice and agree to abide by its terms and conditions. Failure to comply with these terms may result in legal action and the revocation of your rights to use MetaEdit Plus.

# Screenshots
If you want to see how MetaEdit Plus looks before downloading, check out the screenshots below. The images illustrate the tagging process in step by step. From the initial startup screen to adding tags for your files, these screenshots guide you through the entire process.

| Startup Interface          | Customizing Tags             | Processing Files           |
|------------------------------|------------------------------|------------------------------|
| <img src="https://github.com/BerndHagen/MetaEdit-Tag-Editor/raw/main/img/v1.0.3-metaedit_startup.png" width="300px"> | <img src="https://github.com/BerndHagen/MetaEdit-Tag-Editor/raw/main/img/v1.0.3-metaedit_inputs.png" width="300px"> | <img src="https://github.com/BerndHagen/MetaEdit-Tag-Editor/raw/main/img/v1.0.3-metaedit_generate.png" width="300px"> |