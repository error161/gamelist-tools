# Gamelist Tools

A collection of tools to manage and generate gamelist XML files for retro gaming frontends.

## Introduction

Managing emulation ROMs involves not only organizing game files but also enhancing the gaming experience by associating them with visual assets like box art, covers, and screenshots. This enrichment process, known as "scraping," entails collecting metadata and media from various databases to provide detailed information and visuals for each game. Tools like [Skraper](https://skraper.net) facilitate this process by automating the retrieval and association of such data, ensuring a comprehensive and visually appealing game library but the support for UNIX system is still limited.
The Gamelist Tools project aims to bridge this gap by providing a set of scripts and utilities designed to work seamlessly on UNIX-like systems. These tools are tailored for users who prefer command-line interfaces and seek to automate the generation of gamelist XML files, making it easier to manage their game collections.

The GameList Tools aims to streamline the organization and customization of your game library by providing tools that help generate and manage gamelist files, making it easier to integrate ROMs and their associated media into your favorite emulation frontend.

## Features
- **Gamelist Generator**: A Bash script to create an XML gamelist from ZIP files in a specified directory.
- Automatically extracts game names from filenames.
- Matches games with corresponding images in a given folder.
- Supports custom output file paths.

## Installation
Clone the repository:
```sh
git clone https://github.com/yourusername/gamelist-tools.git
cd gamelist-tools
```

## Usage
Run the script with the following options:
```sh
./gamelist_generator --output-file <output_file> --images-folder <images_folder> <directory>
```

### Options:
- `-o, --output-file` → Specify the output XML file (default: `gamelist.xml`)
- `-i, --images-folder` → Specify the folder containing game images
- `<directory>` → The directory containing game ZIP files

### Example:
```sh
./gamelist_generator -o my_gamelist.xml -i images_folder roms
```
This generates `my_gamelist.xml`, using ZIP files from the `roms` directory and matching images from `images_folder`.

## Roadmap
- Additional tools for gamelist management
- Support for more metadata extraction
- GUI or interactive mode

## License
This project is licensed under the MIT License.


