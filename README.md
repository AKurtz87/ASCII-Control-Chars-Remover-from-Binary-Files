# ASCII-Control-Chars-Remover-from-Binary-Files

This is a Node.js script that reads a binary file and converts its content into ASCII text. It does so by first replacing specific characters (defined in the charsToReplace array) with a space character, then converting the resulting buffer to ASCII text and formatting it with a maximum of 50 characters per line.

The script also generates a random image of ASCII characters using ANSI escape codes to colorize them, which is printed to the console before and after the conversion process.

<img width="592" alt="image" src="https://user-images.githubusercontent.com/91114967/224286838-a8ba0bce-bab7-408e-83ca-b3616fba1ee1.png">

To use this script, you would need to run it from the command line and provide the path to the input binary file as the first argument. The output file will be created in the same directory as the script with the name "asciiFile.txt".

# Requirements

To run this script, you will need:

- Node.js v10 or higher
- A binary file to convert to ASCII

# Usage

To use this script, run the following command from the command line:

> node ascii_remove_control_chars_from_file.js filename

Where inputFilePath is the path to the binary file you want to convert.

The output file will be created in the same directory as the script with the name "asciiFile.txt".
The script will also generate a random image of ASCII characters, which is printed to the console before and after the conversion process.

# Customization

By default, the script removes the control ASCII characters contained in the following array:

const charsToReplace = ["\x00", ...];

# Purpose

The purpose of this Node.js script is to convert binary files to ASCII text and remove control ASCII characters. This allows for the identification of strings of interest for YARA rules.

