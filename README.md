# Gamelist Tools

A collection of tools to manage and generate gamelist XML files for retro gaming frontends.

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
./generate_gamelist.sh --output-file <output_file> --images-folder <images_folder> <directory>
```

### Options:
- `-o, --output-file` → Specify the output XML file (default: `gamelist.xml`)
- `-i, --images-folder` → Specify the folder containing game images
- `<directory>` → The directory containing game ZIP files

### Example:
```sh
./generate_gamelist.sh -o my_gamelist.xml -i images_folder roms
```
This generates `my_gamelist.xml`, using ZIP files from the `roms` directory and matching images from `images_folder`.

## Roadmap
- Additional tools for gamelist management
- Support for more metadata extraction
- GUI or interactive mode

## License
This project is licensed under the MIT License.


