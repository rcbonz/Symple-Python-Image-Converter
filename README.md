# Symple-Python-Image-Converter
Convert and/or resize images easily.

### How it works
Basic code with PIL lib that handles the inputs.

### Functionalities
1. Convert image
2. Resize image
3. Flip image horizontally
4. Flip image vertically
5. Transpose and transverse image
6. Rotate image 90, 180 or 270 degrees
7. Supports bmp, dds, dib, eps, gif, ico, jpeg, jpg, pcx, png, tiff, webp (not all tested)

### Requirements
```
pip install Pillow
```

### Usage
```
Usage:
    python3 simpleImageConverter.py -i <inputfile> -o <outputfile> -x <outwidth> -y <outheight>
    python3 simpleImageConverter.py -i <inputfile> -f <format> -x <outwidth> -y <outheight>

Options:
        -i, --input <file>          File to convert
        -o, --output <file>         File output (if blank, same as input. Input will be overwriten.)
        -x, --width <pixels>        Width in pixels if resize is desired
        -y, --heigh <pixels>        Heigh in pixels if resize is desired
        -e, --extension <format>    File extension output. Output file name extension will be used if given.
        -f, --fliph                 Flip image horizontally.
        -v, --flipv                 Flip image vertically.
        -p, --transpose             Transpose image.
        -t, --transverse            Transverse image.
        --r90                       Rotate image 90 degrees.
        --r180                      Rotate image 180 degrees.
        --r270                      Rotate image 270 degrees.
        -h                          This menu.
        --version                   Version.

Examples:
    python3 simpleImageConverter.py -i image.jpg -o image_out.gif -x 100 -y 100
    python3 simpleImageConverter.py -i image.jpg -o image_out.png -x 200  (in this case, y size will be proportional to x)
    python3 simpleImageConverter.py -i image.png -f gif -y 80  (in this case, file output is image.gif)
    python3 simpleImageConverter.py -i image.png -y 350  (in this case, file output is resized image.png)
```

### Supported image formats
bmp, dds, dib, eps, gif, ico, jpeg, jpg, pcx, png, tiff, webp

### To Do
* Make code nicer

### License
[DWTFYWWI](https://github.com/avar/DWTFYWWI)
