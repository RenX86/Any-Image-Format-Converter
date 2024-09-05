# Image Converter

This Python-based tool allows you to convert images between various formats such as PNG, JPG, JPEG, GIF, BMP, TIFF, and WebP. The project uses ImageMagick for image processing and supports quality control, making it ideal for optimizing images in bulk.

## Features
- Converts images between multiple formats: `png`, `jpg`, `jpeg`, `gif`, `bmp`, `tiff`, and `webp`, or any format supported by **ImageMagick**
- Allows specifying image quality (0-100) for formats like JPEG.
- Optional output directory selection for organizing converted images.
- Includes a batch script for easy execution on Windows systems.
- Detailed error handling and user-friendly prompts.
- Loop functionality for converting multiple images in a single session.

## Prerequisites

- **Python 3.6** or higher.
- **ImageMagick** command-line tools (`magick`).
- Add ImageMagick to your system `PATH`.

## Installation

1. Clone this repository or download the necessary files:
   ```bash
   git clone https://github.com/RenX86/MultiFormat-Image-Converter.git
Or download the Image-Converter.py and Image-Convert.bat files directly.

2. Install ImageMagick:
   - **Windows**: Download from [ImageMagick](https://imagemagick.org/script/download.php) and add to your `PATH`.
   - **macOS**: Use Homebrew: `brew install imagemagick`.
   - **Linux**: Install via your package manager, e.g., `sudo apt-get install imagemagick`.

3. (Optional for Windows users) Add the script directory to your system `PATH` to run from anywhere:
   - Right-click "This PC" > "Properties".
   - Click "Advanced system settings" > "Environment Variables".
   - Under "System variables", select "Path" > "Edit".
   - Add the full path to your script directory.

## Usage

### Running on Windows

1. Open a command prompt.
2. Navigate to the script directory or run the batch file:
   ```bash
   Image-Converter.bat
   ```
3. Follow the on-screen prompts to:
   - Specify the image file path.
   - Type the output format.
   - Choose the quality level (optional) Press Enter to skip .
   - Specify the output directory (optional) Press Enter to skip.

4. (Optional) Add the batch file in the environment variable PATH then open terminal and type:
    ```bash
    Image-Converter

### Running on macOS/Linux

1. Open a terminal.
2. Navigate to the script directory.
3. Run the Python script directly:
   ```bash
   python Image-Converter.py
   ```
4. Follow the prompts as described above.

## Configuration

You can modify the following settings in `Image-Converter.py`:

- `DEFAULT_QUALITY`: The default image quality (0-100).
- `SUPPORTED_FORMATS`: A list of supported formats for conversion. Add more formats here, almost all the formats supported as it uses **ImageMagick**

## Troubleshooting

- **Python not found**: Ensure Python is installed and added to your `PATH`.
- **ImageMagick not found**: Make sure ImageMagick is installed and the `magick` command is accessible.

## Contributing

Contributions are welcome! Feel free to fork this repository and submit pull requests with improvements or bug fixes.

