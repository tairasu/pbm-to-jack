# PBM to Jack Converter

## Overview

This project provides a single HTML file to convert PBM (Portable Bitmap) files to Jack language functions, specifically designed for the [Nand2Tetris](https://www.nand2tetris.org/) project. The tool reads a PBM file and generates a Jack function to draw the image in memory.

## Requirements

- The PBM file must be of type P1 (plain PBM format).
- The image width must be a multiple of 16 pixels.

## Usage

1. Open the `index.html` file in a web browser.
2. Select a PBM file.
3. The converted Jack code will be displayed in the output textarea.

## How It Works

1. The user selects a PBM file.
2. The file is read and processed:
    - Comments and empty lines are filtered out.
    - The file type is checked to ensure it's P1.
    - The image dimensions are extracted and validated.
    - The pixel data is concatenated into a single string.
3. The pixel data is processed column by column, converting each 16-bit wide column into a signed decimal integer.
4. A Jack function is generated to draw the image in memory.


## Contributions

Contributions are welcome. Please fork the repository and submit a pull request with your improvements.

## License

This project is licensed under the MIT License.