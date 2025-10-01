# WaterMarkAdd

A simple Python script to add a watermark to images.

## Description

This script takes a folder of images, a logo, and an output folder as input. It then adds the logo to the top-right corner of each image with 70% opacity and saves the watermarked images to the output folder.

## Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/krishnauprety/WaterMarkAdd.git
    ```
2.  Install the dependencies using Poetry:
    ```bash
    poetry install
    ```

## Usage

1.  Place your images in the `images` folder.
2.  Place your logo in the root folder and name it `logo.png`.
3.  Run the script:
    ```bash
    poetry run python main.py
    ```
4.  The watermarked images will be saved in the `output` folder.

## Configuration

You can change the input folder, output folder, and logo path by editing the following lines in `main.py`:

```python
if __name__ == "__main__":
    main_image_folder = "images"      # Folder with input images
    logo_path = "logo.png"            # Path to your logo image (must be PNG)
    output_folder = "output"          # Folder to save watermarked images

    add_logo_watermark(main_image_folder, logo_path, output_folder)
```
