# Case Converter Program 🐍

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

A simple Python utility for converting PascalCase and CamelCase strings to snake_case. Perfect for developers working with different coding conventions.

## 📜 About
The Case Converter Program helps standardize variable and function naming across different programming styles. It takes strings in PascalCase (where each word is capitalized) or CamelCase (where the first word is lowercase and subsequent words are capitalized) and converts them to snake_case (all lowercase with underscores between words).

## ✨ Features
- Converts both PascalCase and CamelCase to snake_case
- Preserves original characters except for case changes
- Handles strings with numbers correctly
- Simple command-line execution
- Easy to integrate into other Python projects

## 🚀 Quick Start

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/fahadelahikhan/Case-Converter-Program.git
   cd Case-Converter-Program
   ```

2. Run the application:
   ```bash
   python Case Converter Program.py
   ```

### Basic Usage
```python
# Import the conversion function
from case_converter import convert_to_snake_case

# Convert a PascalCase string
pascal_string = "IAmAPascalCasedString"
snake_case = convert_to_snake_case(pascal_string)
print(snake_case)  # Output: i_am_a_pascal_cased_string

# Convert a CamelCase string
camel_string = "iAmACamelCasedString"
snake_case = convert_to_snake_case(camel_string)
print(snake_case)  # Output: i_am_a_camel_cased_string
```

### Example Conversion
```python
# Converting a complex string with numbers
complex_string = "UserID123Generator"
converted = convert_to_snake_case(complex_string)
print(converted)  # Output: user_id123_generator

# Converting a string with mixed cases
mixed_case = "HTTPResponseCode"
converted = convert_to_snake_case(mixed_case)
print(converted)  # Output: http_response_code
```

## 📖 How It Works
The converter works by:
1. Iterating through each character in the input string
2. Checking if a character is uppercase
3. When an uppercase character is found, converting it to lowercase and prefixing with an underscore
4. Joining all characters together and removing any leading or trailing underscores

This approach effectively identifies word boundaries in PascalCase and CamelCase strings and inserts underscores accordingly.

## ⚖️ License
Distributed under the MIT License. See [LICENSE](LICENSE) for details.

---

> **Note**: This is a simple utility for educational and productivity purposes. For more complex naming convention conversions, consider using established libraries with additional features.
