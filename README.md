# Case Converter Program 🔄

![Python Version](https://img.shields.io/badge/python-3.6%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

A Python utility that converts PascalCase or CamelCase strings to snake_case, offering an educational insight into basic string manipulation techniques.

## About
This project transforms case-formatted strings into snake_case, promoting consistent coding styles. It serves as a practical tool for beginners exploring Python programming and software design principles.

## Features
- Converts PascalCase and CamelCase strings to snake_case.
- Handles strings without uppercase letters gracefully.
- Removes extraneous leading/trailing underscores.
- Simple and efficient implementation.
- Easily integrated into other Python projects.

## Quick Start

### Installation
Clone the repository:
```bash
git clone https://github.com/fahadelahikhan/Case-Converter-Program.git
cd Case-Converter-Program
```

(Optional) Install dependencies:
```bash
pip install -r requirements.txt
```

### Basic Usage
```python
from case_converter import convert_to_snake_case

input_string = "IAmACamelCaseString"
output_string = convert_to_snake_case(input_string)
print(output_string)  # Expected output: "i_am_a_camel_case_string"
```

## Example
A realistic usage scenario:
```python
input_str = "ConvertThisString"
result = convert_to_snake_case(input_str)
print(f"Converted string: {result}")  # Expected output: "convert_this_string"
```

## How It Works
The function iterates over each character of the input string. If a character is uppercase, it is converted to lowercase and prefixed with an underscore (except for the first character). The final string is then stripped of any leading underscores to produce a proper snake_case output.

## License
Distributed under the [MIT License](LICENSE).

> **Note**: This tool is provided as-is without any warranty. Use it at your own risk.
