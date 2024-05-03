# Steganography
Steganography is the art of hiding information within other data in such a way that it's not apparent to casual observers. Implementing steganography in C involves manipulating bits within files to embed secret messages without altering the visible content.

# How It Works:

This C program offers a simple implementation of steganography. It works by manipulating the least significant bits of pixels in an image file. Each pixel in an image is represented by RGB (Red, Green, Blue) values. By altering the least significant bits of these values, we can embed secret information into the image.

# Encoding:

The user provides the original image file and the message they want to hide.
The program reads the image and converts it into pixel data.
It then converts the message into binary format.
The program embeds the binary message into the least significant bits of the pixel data.
Finally, it saves the modified pixel data as a new image file.

# Decoding:

The user provides the image file containing the hidden message.
The program reads the image and extracts the pixel data.
It then retrieves the least significant bits of each pixel to reconstruct the binary message.
The binary message is converted back into text format, revealing the hidden message.
Instructions:

1. Compilation:

Clone the repository: git clone https://github.com/your_username/steganography.git
Navigate to the project directory: cd steganography
Compile the code: gcc steganography.c -o steganography
2. Usage:

Encoding: ./steganography encode <original_image> <message_file> <output_image>
Decoding: ./steganography decode <image_with_hidden_message>
Example:

Encoding: ./steganography encode original_image.png secret_message.txt encoded_image.png
Decoding: ./steganography decode encoded_image.png
Notes:

Supported image formats: PNG, JPEG.
Make sure the message file is not larger than the available space in the image file.
For better concealment, use high-resolution images with complex patterns.
This program provides a basic introduction to steganography. For more advanced features and robustness, consider exploring additional techniques and algorithms. Feel free to contribute to the project or suggest improvements. Happy coding!
