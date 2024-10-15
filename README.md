# barcode-cv-project
This project converts a text string into a barcode and decodes it back. The encode function generates a barcode by drawing bars based on letter positions. The decode function reads the barcode, scans the middle row, and decodes the bar widths into characters. The barcode is saved as output.png.

## Features
- **Encode**: Converts a given text string into a barcode image.
- **Decode**: Reads a barcode image and decodes it back to the original text.

## Prerequisites

Before running the script, you need to install the required Python package:
```
pip install opencv-python numpy
```
## How It Works
### Encode
The encode function takes a string and generates a barcode by drawing rectangular bars on a canvas. The width of each bar corresponds to a letter's position in the alphabet. Each character in the string, including spaces, is represented by a specific bar width.

### Decode
The decode function reads a barcode image, scans the middle row for black bars, and decodes the width of the bars back into characters. It supports uppercase letters and spaces.

### Output
The generated barcode image is saved as output.png in the working directory.

## Example Usage
### Encoding a Text to Barcode
```
from barcode_script import encode
encode("Abbas Cheddad")

```
This will generate a barcode for the string "Abbas Cheddad" and save it as output.png.
### Decoding the Barcode
```
from barcode_script import decode
decoded_text = decode('output.png')
print(decoded_text)

```
This will decode the barcode saved in output.png and print the original text.

## Author
Developed by Patteera Lerdtada.
