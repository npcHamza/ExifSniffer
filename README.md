# ExifSniffer

![Banner](https://raw.githubusercontent.com/npcHamza/ExifSniffer/refs/heads/main/banner.png)

**ExifSniffer** is a command-line tool designed to display the EXIF metadata of image files in the current directory. It provides an interactive interface for users to select an image file and view its detailed metadata in a formatted table.

## Features

- Lists all image files (`.jpg`, `.jpeg`, `.png`) in the current directory.
- Displays EXIF data in a readable, color-coded table format using `rich` and `colorama` libraries.
- Provides an ASCII art banner and an intuitive selection menu for a smooth user experience.

## Prerequisites

Make sure you have the following Python libraries installed:

```bash
pip install rich colorama exif Pillow
```

## Usage

1. Clone this repository and navigate to the directory:

   ```bash
   git clone https://github.com/npcHamza/ExifSniffer.git
   cd ExifSniffer
   ```

2. Run the script:

   ```bash
   python exif_sniffer.py
   ```

3. The script will display a banner, list all available image files in the directory, and prompt you to select an image file. 

4. After selecting an image file by its number, the EXIF metadata will be displayed in a detailed table.

## Example Output

```
Select a file to view its EXIF data:
┏━━━━━┳━━━━━━━━━━━━━━━┓
┃ No. ┃ File Name     ┃
┣━━━━━╋━━━━━━━━━━━━━━━┫
┃ 1   ┃ image1.jpg    ┃
┃ 2   ┃ image2.jpeg   ┃
┃ 3   ┃ photo.png     ┃
┗━━━━━┻━━━━━━━━━━━━━━━┛

Select a number (or 'q' to quit): 1

EXIF data for image1.jpg:
┏━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━┓
┃ Tag         ┃ Value         ┃
┣━━━━━━━━━━━━━╋━━━━━━━━━━━━━━━┫
┃ Model       ┃ Canon EOS 5D  ┃
┃ DateTime    ┃ 2024:11:10    ┃
┃ ...         ┃ ...           ┃
┗━━━━━━━━━━━━━┻━━━━━━━━━━━━━━━┛
```
